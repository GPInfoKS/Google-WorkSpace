# 📚 13 — Lições aprendidas

## 🧠 Principais aprendizados

### 1. Tecnologia não substitui governança

Criar Groups, UOs e Shared Drives não resolve um ambiente desorganizado se não houver critérios de utilização.

### 2. Identidade deve ser individual

Contas genéricas utilizadas por pessoas dificultam rastreabilidade.

### 3. UO e Grupo possuem papéis diferentes

UO é principalmente escopo de política; grupo é principalmente associação e acesso.

### 4. Migração é uma oportunidade de saneamento

Não é recomendável transportar indiscriminadamente todo o legado.

### 5. E-mail precisa de governança

Aliases, grupos, encaminhamentos, catch-all e roteamento devem possuir finalidade documentada.

### 6. O legado precisa permanecer durante a transição

Migrar não significa apagar imediatamente a origem.

### 7. Piloto reduz risco

Uma pequena implantação controlada permite descobrir problemas antes da expansão.

---

## 🏁 Resultado esperado

A organização passa de uma estrutura orientada a:

```text
👤 pessoas
   +
📁 pastas
   +
🔐 permissões individuais
   +
📧 contas genéricas
```

para uma estrutura orientada a:

```text
👤 identidade
      +
🏢 políticas
      +
👥 grupos
      +
🗄️ armazenamento corporativo
      +
🔐 governança
```

---

## 💡 Reflexão

> O objetivo da modernização não é apenas trocar o servidor de arquivos ou migrar para a nuvem.
>
> É construir uma estrutura que continue organizada depois que o projeto terminar.
