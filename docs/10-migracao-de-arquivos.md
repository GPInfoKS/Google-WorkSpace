# 🚚 10 — Migração de arquivos

## 🏚️ VAMOS VER O QUE TEM NESSE PORÃO

A migração não deve ser tratada como simples cópia de dados.

### Princípio central

> **Nenhum arquivo deve ser migrado simplesmente porque existe.**

Antes da transferência, avaliar:

- propósito;
- responsável;
- utilização;
- sensibilidade;
- permissões;
- duplicidade;
- necessidade de retenção;
- compatibilidade;
- destino.

---

## 🔄 Fluxo

```mermaid
flowchart LR
    A["🔎 Inventário"] --> B["🧹 Classificação"]
    B --> C["👤 Validação com departamento"]
    C --> D["🗂️ Destino"]
    D --> E["🧪 Piloto"]
    E --> F["✅ Validação"]
    F --> G["🚚 Lote"]
    G --> H["🔎 Homologação"]
    H --> I["🔄 Transição"]
    I --> J["🧓 Legado"]
```

## 🧹 Classificação

| Categoria | Ação |
|---|---|
| 🟢 Ativo | Migrar |
| 🔵 Histórico | Migrar/arquivar |
| 🟡 Temporário | Validar |
| 🟠 Duplicado | Consolidar |
| 🔴 Obsoleto | Validar descarte |
| 🔒 Sensível | Migrar com acesso restrito |

## ⚠️ Regras

- Manter servidor legado durante a transição.
- Definir rollback.
- Validar integridade.
- Validar permissões.
- Validar abertura dos arquivos.
- Validar com responsável do departamento.
- Não excluir dados apenas porque foram migrados.

## 📋 Homologação

| Teste | Resultado |
|---|---|
| Arquivo abre | ⬜ |
| Arquivo íntegro | ⬜ |
| Usuário correto acessa | ⬜ |
| Usuário sem acesso não acessa | ⬜ |
| Estrutura correta | ⬜ |
| Nome/path compatível | ⬜ |
| Responsável validou | ⬜ |
