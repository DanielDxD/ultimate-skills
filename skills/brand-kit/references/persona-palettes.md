# Paletas por persona

Sugira 4–6 cores nomeadas com papéis: `bg`, `surface`, `fg`, `muted`, `accent`, `accent-fg`. Ajuste saturação/luminosidade ao brief; a tabela é direção, não receita fechada.

| Persona / indústria | Direção de cor | Accent típico | Evitar |
|---------------------|----------------|---------------|--------|
| Tech / B2B / confiança | Neutros frios + azul | Azul médio `#2563EB` → `#1D4ED8` | Roxo genérico “AI default” |
| Fintech / segurança | Escuro + verde ou azul sóbrio | Verde institucional `#0F766E` | Neon agressivo |
| Wellness / saúde / natureza | Off-white + verdes/terra | Verde `#2F6F5e` / terra `#A67C52` | Preto puro dominante |
| Luxury / moda / editorial | Neutros + preto/creme | Ouro suave `#C2A878` ou preto `#111110` | Cores candy |
| Food / restaurant | Quente, apetite | Terracota `#C45C26` / vinho `#7B2D26` | Azul clínico |
| Kids / educação infantil | Saturados controlados + creme | Coral `#E85D4C` / amarelo `#E8B84A` | Contraste baixo |
| Criativo / agência / portfólio | Alto contraste, 1 accent ousado | Accent do brief (1 só) | Multicolor sem hierarquia |
| Sustentabilidade / ESG | Terra + verde musgo | Musgo `#4A5D23` | Plástico brilhante |
| Nightlife / entretenimento | Escuro + 1 neon contido | Magenta/ciano pontual | Neon em tudo |
| Jurídico / consultoria | Navy + cinza quente | Navy `#1E3A5F` | Cores infantis |

## Como apresentar

```markdown
## Paleta sugerida (persona: <…>)
- **Por quê:** <1 frase>
- bg: #…
- surface: #…
- fg: #…
- muted: #…
- accent: #…
- accent-fg: #…
Confirma esta paleta ou ajustamos?
```

## Tokens CSS sugeridos

```css
:root {
  --color-bg: …;
  --color-surface: …;
  --color-fg: …;
  --color-muted: …;
  --color-accent: …;
  --color-accent-fg: …;
}
```
