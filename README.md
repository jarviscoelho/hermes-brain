# 🧠 Hermes Brain

> O cérebro do agente Hermes — memória, princípios e configurações.

## O Que É

Este repo armazena todo o **conhecimento persistente** do agente Hermes:
- Quem é o usuário
- Quais são os princípios de trabalho
- Como executar tarefas específicas
- Lições aprendidas

## Estrutura

```
hermes-brain/
├── MEMORY.md              # Memória curada (longo prazo)
├── USER.md                # Perfil do usuário
├── memory/                # Daily logs (contexto efêmero)
│   └── YYYY-MM-DD.md
├── skills/                # Procedimentos carregáveis
│   ├── soul-principles/   # Como agir com Marcos
│   ├── minimax-image-generation/  # Como gerar imagens
│   └── workspace-guide/   # Como navegar no workspace
└── README.md
```

## Princípios Fundamentais

| Princípio | Significado |
|-----------|-------------|
| **AUTONOMIA** | Execute sem perguntar quando possível |
| **PROATIVIDADE** | Faça antes de ser perguntado |
| **IR ATÉ O FIM** | Resolva end-to-end com validação |
| **REGRA 80/20** | Foque no que entrega 80% dos resultados |
| **FOCO EM RECEITA** | Tudo deve impactar $ |

## Como Funciona

### Memória
- `MEMORY.md` + `USER.md` são carregados no início de cada sessão
- `memory/YYYY-MM-DD.md` armazenam contexto do dia-a-dia
- Skills são carregadas **sob demanda** via `skill_view(name)`

### Boas Práticas
- ✅ Atualize `MEMORY.md` quando aprender algo permanente
- ✅ Escreva daily log no início de cada sessão
- ✅ Registre lições IMEDIATAMENTE quando errar
- ❌ **Nunca duplique** — uma info, um lugar

### Hierarquia de Truth
```
SOUL.md (openclaw-workspace)
    ↓
USER.md (hermes-brain)
    ↓
MEMORY.md (hermes-brain)
```

## Repositórios Relacionados

| Repo | Conteúdo |
|------|----------|
| `hermes-brain` | Este repo — memória do agente |
| `openclaw-workspace` | Projetos, agentes,流水, execução |

---

_Built with [Hermes Agent](https://github.com/NousResearch/hermes-agent)_
_Updated: 2026-04-18_
