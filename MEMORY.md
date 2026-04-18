# MEMORY.md

> Curated long-term memory. Decisions, durable facts, preferences that survive sessions.
> **Update when:** You learn something permanent. Never duplicate from USER.md.

---

## Capabilities

### MiniMax Image Generation
- **Endpoint:** `https://api.minimax.io/v1/image_generation` (chat uses `/anthropic`)
- **Auth:** `source ~/.hermes/.env` → `Authorization: Bearer $MINIMAX_API_KEY`
- **Model:** `image-01`
- **Tip:** English prompts > Portuguese. URLs expire — download immediately.

---

## User Profile
> Full profile in `USER.md`. Only reference keys here.

- Idioma: **pt-BR**
- Projeto: Autivox (OpenClaw Gateway) + monetização SaaS/YouTube faceless
- Nicho: Finance (Nick and Nate Invests style)
- Ver `USER.md` para preferências completas

---

## Project: Autivox

### Missão
Sistema autônomo de monetização → 3k-5k BRL/mês (30d), 10k+ BRL/mês (12m)

### Princípios (do USER.md — não duplicar aqui)
- AUTONOMIA + PROATIVIDADE + IR ATÉ O FIM + 80/20 + FOCO RECEITA
- Ver `skills/soul-principles/` para guia completo

### Regras Críticas
- ❌ **NUNCA** sugerir deploy externo Autivox sem permissão explícita
- ❌ **NUNCA** 2 providers iguais nos primeiros 3 fallbacks
  - Ordem segura: MiniMax → Zai → Codex → Sonnet → Opus → Gemini
- ❌ Pollinations instável (530) → Seedream 4.5 ou GPT-4o
- ✅ Config changes: backup → leia docs → valide → aplique

### Source of Truth
- Scripts YouTube: `openclaw-workspace/prompts/metaprompt_nick.md` é autoridade
- Se correção conflita com metaprompt → NÃO aplique, alerte

---

## Resources
- **Workspace:** `openclaw-workspace/` (projetos, agentes,流水)
- **Skills:** `skills/` (procedimentos, não memória)
- **Daily logs:** `memory/` (contexto efêmero)

---

_Last updated: 2026-04-18_
