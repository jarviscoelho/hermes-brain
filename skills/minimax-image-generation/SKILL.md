---
name: minimax-image-generation
description: Generate images using MiniMax image-01 API
triggers:
  - generate image
  - create image
  - MiniMax image
  - gerar imagem
---

## Steps

1. Source the environment: `source ~/.hermes/.env`
2. Make curl request to endpoint: `https://api.minimax.io/v1/image_generation`
3. Required headers:
   - `Authorization: Bearer $MINIMAX_API_KEY`
   - `Content-Type: application/json`
4. Request body (JSON):
   ```json
   {
     "model": "image-01",
     "prompt": "your prompt in English",
     "image_size": "16:9"
   }
   ```
5. Parse response: `response.data.image_urls[0]` contains the image URL
6. Download image with `curl -L` (URLs expire quickly)
7. Deliver image to user via `MEDIA:/path/to/file`

## Notes

- The chat model uses `api.minimax.io/anthropic`, but image generation uses a different endpoint
- English prompts work better than Portuguese
- Image URLs are temporary (Expires in URL params), download promptly
- Response format is URL by default
