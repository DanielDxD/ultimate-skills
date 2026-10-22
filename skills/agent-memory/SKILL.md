---
name: agent-memory
description: >-
  Memória persistente da IA no projeto: lê e atualiza decisões, preferências e
  contexto em arquivos. Use sempre que o usuário pedir para lembrar, gravar
  decisão, “como decidimos”, preferências do projeto, ou em tarefas longas que
  dependam de contexto acumulado.
---

# Agent Memory

Contexto importante vive em arquivos do repo — não só no chat.

## Onde guardar

Default: `docs/agent-memory/`

| Arquivo | Conteúdo |
|---------|----------|
| `decisions.md` | Decisões e porquês (data + resumo) |
| `preferences.md` | Preferências do usuário/projeto (stack, tom, UI) |
| `context.md` | Resumo atual do produto e estado |

Se a pasta não existir, crie-a ao gravar a primeira memória.

## Workflow

1. **No início** de tarefas longas ou ambíguas: ler os arquivos de memória existentes.
2. **Usar** o que estiver documentado; citar a fonte (“em preferences.md…”).
3. **Atualizar** após decisões relevantes, preferências novas ou mudança de contexto do produto.
4. **Não inventar** memória ausente — se não estiver no arquivo, pergunte ou registre como nova.

## Formato de decisão

```markdown
## YYYY-MM-DD — <título>
- **Decisão:** …
- **Por quê:** …
- **Consequências:** …
```

## Regras

- Memória é do projeto, versionável com o git.
- Não gravar segredos (tokens, chaves, senhas).
- Entradas curtas e pesquisáveis; evite dumps de conversa inteira.
