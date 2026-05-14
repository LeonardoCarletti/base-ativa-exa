# Dashboard — Base Ativa de Assinaturas

Dashboard analítico da base ativa de assinaturas · Vertical Segurança · referência maio/2026.

## Deploy

### Vercel (recomendado)
```bash
npm i -g vercel
vercel
```
Ou conecte o repositório direto no [vercel.com](https://vercel.com) — deploy automático em cada push.

### GitHub Pages
Ative em **Settings → Pages → Deploy from branch → main → / (root)**.

## Estrutura
```
dashboard-base-ativa/
├── index.html      # Dashboard completo (self-contained, sem dependências externas)
├── vercel.json     # Configuração de deploy
├── .gitignore
└── README.md
```

## Seções
- **Visão Geral** — KPIs principais mai/26
- **Produto Pai** — visão unificada, exata e evolução 24 meses
- **Por Oferta** — tabela com MoM + distribuição visual
- **Por Parceiro** — base atual, YoY e share TIM Group
- **Evolução Histórica** — série completa 53 meses + fases de crescimento
- **Sinais & Alertas** — pontos de atenção para o time de produto

> Arquivo `index.html` é **100% self-contained** — zero CDN, zero dependências externas.
