# 🎯 01 — Contexto e objetivos

## 🐂 DAR NOME AOS BOIS

O primeiro objetivo da reestruturação é corrigir problemas de identidade e organização existentes no ambiente legado.

### Problema

Contas genéricas podem acabar sendo utilizadas como identidade individual:

```text
financeiro@empresa.exemplo
        ↓
      1 pessoa
```

Isso dificulta:

- auditoria;
- responsabilização;
- desligamento;
- transferência de função;
- recuperação de acesso;
- controle de privilégios;
- rastreabilidade.

### Arquitetura proposta

```text
👤 Pessoa
   │
   └── usuario.nominal@empresa.exemplo

🏢 Função departamental
   │
   └── financeiro@empresa.exemplo
             │
             └── 👥 Grupo Financeiro
```

### Objetivo

Separar **identidade pessoal** de **identidade funcional/departamental**.

---

## 🎯 Objetivos específicos

1. Inventariar contas existentes.
2. Identificar contas genéricas.
3. Identificar aliases.
4. Identificar encaminhamentos.
5. Identificar delegações.
6. Identificar dependências externas.
7. Definir contas que devem ser convertidas em grupos, aliases ou mantidas.
8. Planejar desligamentos e transições sem perda de informação.

---

## 🧭 Critérios de decisão

| Situação | Tratamento a avaliar |
|---|---|
| Conta representa uma pessoa | 👤 Usuário nominal |
| Endereço representa departamento | 👥 Grupo |
| Endereço alternativo do mesmo serviço | 🏷️ Alias |
| Conta utilizada por sistema | ⚙️ Conta técnica / integração |
| Endereço histórico utilizado | 🔀 Roteamento controlado |
| Endereço sem uso | 🧹 Descontinuar após validação |
