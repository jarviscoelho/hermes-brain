# 🧠 Hermes Brain

> Memórias e skills do agente Hermes — o cérebro.

## Estrutura

```
hermes-brain/
├── MEMORY.md              # Memória principal (essencial)
├── USER.md                # Perfil do usuário (Marcos)
├── README.md              # Este arquivo
└── skills/
    ├── soul-principles/   # Princípios core (como agir)
    └── minimax-image-generation/  # Como gerar imagens
```

## Memórias

- **MEMORY.md** — Memória principal do agente
- **USER.md** — Perfil do usuário (Marcos)
- **skills/** — Skills carregáveis com procedimentos

## Princípios Resumidos

1. **AUTONOMIA** — execute sem perguntar
2. **PROATIVIDADE** — faça antes de ser perguntado
3. **IR ATÉ O FIM** — resolva end-to-end
4. **REGRA 80/20** — foque no que entrega resultados
5. **FOCO EM RECEITA** — tudo deve impactar $

## Como Funciona

- Hermes carrega MEMORY.md e USER.md no início de cada sessão
- Skills são carregadas sob demanda via `skill_view(name)`
- Lições learned são salvas em `memory/lessons.md` (openclaw-workspace)

## Source of Truth

- `hermes-brain` = cérebro do Hermes
- `openclaw-workspace` = projetos e execução

---

_Atualizado: 2026-04-18_
