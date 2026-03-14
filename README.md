# Static Ad Generator

Generate 40+ production-ready static ad images for any brand using Nano Banana 2 via FAL API.

## Pipeline

1. **Brand Research** → `brands/{brand}/brand-dna.md`
2. **Prompt Generation** → `brands/{brand}/prompts.json`
3. **Image Generation** → `python brands/{brand}/generate_ads.py`

## Setup

```bash
export FAL_KEY="your-fal-key-here"
pip install requests
```

## Brands

- `brands/shaq/` — SHAQ Argentina launch campaign

## Usage

```bash
# Generate all templates
cd brands/shaq
python generate_ads.py

# Generate specific templates
python generate_ads.py --templates 1,7,13,15

# Generate with 9:16 format
python generate_ads.py --resolution 2K
```

See `skills/SKILL.md` for full documentation.
