---
name: minimax-image-generation
description: Generate images using MiniMax image-01 API
triggers:
  - generate image
  - create image
  - MiniMax image
  - gerar imagem
  - criar imagem
---

# MiniMax Image Generation

## Quick Reference

```
ENDPOINT=https://api.minimax.io/v1/image_generation
AUTH=source ~/.hermes/.env
MODEL=image-01
```

## Steps

1. `source ~/.hermes/.env`
2. Curl request:
```bash
curl -s -X POST "https://api.minimax.io/v1/image_generation" \
  -H "Authorization: Bearer $MINIMAX_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"model": "image-01", "prompt": "English prompt here", "image_size": "16:9"}'
```
3. Parse: `response.data.image_urls[0]`
4. Download: `curl -L <url> -o /tmp/image.jpg`
5. Deliver: `MEDIA:/tmp/image.jpg`

## Tips
- English prompts > Portuguese
- URLs expire — download immediately
- Sizes: `16:9`, `1:1`, `9:16`, `4:3`

## Common Errors
- `530` → Pollinations error, try again or use Seedream
- `401` → Missing or invalid API key, run `source ~/.hermes/.env`
- `1004` → Auth error, check API key is correct
