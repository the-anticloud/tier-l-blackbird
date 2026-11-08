# Deploy Guide — L_BLACKBIRD
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, PAX 27B, RF analysis, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, PAX 27B, RF analysis tools (local captures only), AIOSS_FORMAT.

## Environment
8GB RAM. GPU for PAX analysis. RF captures from authorized test environment.

## AIOSS Integration
```bash
aioss init --module L_BLACKBIRD --output ./l_blackbird.aioss
aioss append --chain ./l_blackbird.aioss --payload ./output.bin --module L_BLACKBIRD
aioss verify --chain ./l_blackbird.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_BLACKBIRD",
    aioss_chain="./L_BLACKBIRD.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_BLACKBIRD.aioss --verbose
python -m L_BLACKBIRD.tests.smoke
```
