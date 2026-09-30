# 🏗️ 03 — Arquitetura alvo

## Visão

```mermaid
flowchart TB
    GW["☁️ Google Workspace"]

    GW --> ID["👤 Identidade"]
    GW --> OU["🏢 UOs"]
    GW --> GR["👥 Groups"]
    GW --> GM["📧 Gmail"]
    GW --> SD["🗄️ Shared Drives"]
    GW --> EP["💻 Endpoints"]
    GW --> SEC["🔐 Segurança"]

    OU --> O1["TI"]
    OU --> O2["RH"]
    OU --> O3["Financeiro"]
    OU --> O4["Comercial"]
    OU --> O5["Diretoria"]

    GR --> G1["ti@" ]
    GR --> G2["rh@" ]
    GR --> G3["financeiro@" ]
    GR --> G4["comercial@" ]
    GR --> G5["diretoria@" ]

    SD --> S1["PRODETECH - GERAL"]
    SD --> S2["PRODETECH - TI"]
    SD --> S3["PRODETECH - RH"]
    SD --> S4["PRODETECH - FINANCEIRO"]
    SD --> S5["PRODETECH - COMERCIAL"]
    SD --> S6["PRODETECH - DIRETORIA"]
```

## 🧩 Princípios

### 1. Identidade individual

Cada colaborador possui uma identidade própria.

### 2. Políticas por escopo

UOs representam principalmente o escopo de políticas e configurações.

### 3. Acesso por grupo

Grupos representam necessidades de acesso e colaboração.

### 4. Armazenamento por equipe

Shared Drives representam espaços corporativos persistentes.

### 5. Migração gradual

O legado permanece disponível durante as fases de validação e transição.

---

## 🔄 Modelo de decisão

```text
Necessidade
   │
   ├── É identidade? ───────► 👤 Usuário
   │
   ├── É política? ─────────► 🏢 UO
   │
   ├── É acesso? ───────────► 👥 Grupo
   │
   ├── É armazenamento? ────► 🗄️ Shared Drive
   │
   └── É comunicação? ──────► 📧 Gmail / Group / Routing
```
