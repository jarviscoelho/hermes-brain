---
name: workspace-guide
description: Como navegar e usar o openclaw-workspace
triggers:
  - workspace
  - openclaw
  - onde encontrar
  - arquivos
---

# Workspace Guide

## Repositórios
- **hermes-brain** (este): `~/.hermes/memories/` — memória do agente
- **openclaw-workspace:** `/root/.hermes/hermes-agent/openclaw-workspace/` — projetos e流水

## Estrutura openclaw-workspace

```
openclaw-workspace/
├── MEMORY.md              # Memórias consolidadas
├── USER.md                # Perfil do usuário
├── SOUL.md                # Identidade Stark (principais)
├── CRITICAL_LEARNINGS.md  # Erros nunca repetir
├── agents/                # Agentes swarm (Alfred, Loki, etc)
├── memory/
│   ├── YYYY-MM-DD.md     # Daily logs
│   ├── lessons.md         # Lições aprendidas
│   └── corrections/       # Correções registradas
├── prompts/
│   └── metaprompt_nick.md # Source of truth para scripts
├── apps/
│   └── yt-automator/      # Pipeline de videos
└── docs/                  # Documentação
```

## Arquivos Importantes
| Arquivo | Uso |
|---------|-----|
| `SOUL.md` | Princípios e identidade do sistema |
| `metaprompt_nick.md` | Como gerar scripts YouTube |
| `lessons.md` | Erros técnicos e lições |
| `agents/*/SOUL.md` | Personalidade de cada agente |

## Regras
- Workspace repo: nunca fazer commit de `.env` ou credenciais
- Daily logs: escrever no início de cada sessão
- Lições: registrar IMEDIATAMENTE quando aprender algo novo

## Contexto Atual (2026-04-18)
- Autivox: OpenClaw Gateway modo local
- YouTube: 0 subs, 0 videos publicados
- VPS: 69.62.93.146 (Tailscale: 100.124.139.118)
- Canonical backend: `http://127.0.0.1:8020`
