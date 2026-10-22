---
name: consistent-architecture
description: >-
  Mantém arquitetura consistente: boundaries de módulos, estrutura de pastas,
  naming estável e camadas claras. Use sempre que o usuário pedir arquitetura,
  reorganização de pastas, monorepo, camadas, boundaries, clean architecture,
  “onde colocar este arquivo” ou refatoração estrutural — mesmo sem dizer
  “arquitetura”.
---

# Consistent Architecture

Preserve e reforçe a arquitetura existente. Não invente uma estrutura paralela sem necessidade.

## Regras

- Uma responsabilidade por módulo/pasta.
- Imports só “para dentro” (UI → domínio → infra; nunca o inverso sem porta explícita).
- Naming estável e previsível; não misture convenções no mesmo nível.
- Novos arquivos seguem o mapa existente; se o mapa for inadequado, proponha mudança antes de espalhar arquivos.
- Mudança de boundary → ADR curto (contexto, decisão, consequências) em `docs/adr/` ou pasta equivalente do repo.

## Workflow

1. **Inspecionar** — pastas, entrypoints, padrões de import e naming já usados.
2. **Mapear** — desenhe em poucas linhas: camadas, módulos e dependências permitidas.
3. **Alinhar** — proponha o caminho do novo código no mapa; se conflitar, diga o conflito e peça confirmação.
4. **Só então** criar/mover arquivos.
5. **Documentar** — se a boundary mudou, escreva o ADR leve.

## Checklist

- [ ] Pasta e nome batem com o padrão do repo
- [ ] Nenhuma dependência circular ou “para cima” sem porta
- [ ] Código novo não cria um segundo “estilo” de organização
