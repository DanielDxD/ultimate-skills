---
name: brand-kit
description: >-
  Brand kit e criação de logo via /brand-kit: identidade visual, wordmark,
  símbolo, favicon e paleta de cores sugerida pela persona. Use quando o usuário
  invocar /brand-kit ou pedir logo, logotipo, marca, brand kit, identidade
  visual, símbolo, favicon ou paleta de marca.
---

# Brand Kit

Comando típico: `/brand-kit crie uma logo…`. Persona e público-alvo guiam a paleta e o conceito do logo.

## Workflow

1. **Perguntar o que faltar** — persona/público-alvo é **obrigatório**, além de: nome da marca, indústria, personalidade, símbolo vs wordmark, usos (app, site, impresso). Em dúvida, pergunte sempre.
2. **Sugerir paleta pela persona** — leia [references/persona-palettes.md](references/persona-palettes.md). Entregue hex + papéis semânticos (`bg`, `surface`, `fg`, `muted`, `accent`, `accent-fg`) + **uma frase** ligando as cores à persona. Peça confirmação antes de travar tokens.
3. **Propor 2–3 direções de logo** em texto (conceito + porquê), alinhadas à paleta.
4. **Gerar arte** com a ferramenta de imagem do Cursor (`GenerateImage` ou fluxo disponível), incluindo a paleta acordada no prompt.
5. **Entregar** variantes (claro/escuro se fizer sentido), notas de uso (espaço livre, tamanho mínimo, não distorcer) e tokens de cor prontos para o projeto.

## Regras

- Não invente paleta sem explicar o vínculo com a persona.
- Não trave cores sem confirmação do usuário.
- Não embuta arquivos de fonte na skill. Tan Waverly / Godger / Asfar Serif só como sugestão de pair se o projeto já tiver licença/arquivos.
- Não copie marcas existentes; conceito original.

## Entregáveis mínimos

- Paleta nomeada (4–6 cores) + papéis semânticos
- Conceito(s) de logo + arte gerada
- Notas de uso + tokens CSS sugeridos
