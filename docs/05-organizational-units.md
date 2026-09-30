# 🏢 05 — Organizational Units

## 🐒 CADA MACACO NO SEU GALHO

As Unidades Organizacionais devem ser utilizadas para estruturar o ambiente e aplicar políticas ao escopo adequado.

### Estrutura proposta

```text
PROJETO
│
├── 🏢 TI
├── 🏢 RH
├── 🏢 FINANCEIRO
├── 🏢 COMERCIAL
├── 🏢 DIRETORIA
└── 🏢 FUNCIONARIOS
```

## ⚠️ UO ≠ Grupo

| Elemento | Função principal |
|---|---|
| 🏢 UO | Políticas/configuração |
| 👥 Grupo | Associação/acesso |
| 🗄️ Shared Drive | Armazenamento |
| 👤 Usuário | Identidade |

Um usuário pode estar em uma UO e em vários grupos.

```text
                  👤 Pedro
                     │
            ┌────────┴────────┐
            ▼                 ▼
        🏢 Comercial       👥 TI-Projeto
            │                 │
       políticas         acesso específico
```

## 🎯 Regra

Não usar grupos como substitutos de UOs e não usar UOs como substitutos de grupos de acesso.
