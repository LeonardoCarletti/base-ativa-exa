# 📊 Dashboard EXA Analytics — Versão Unificada com INDICADORES NET

## ✅ Arquivo Único Pronto para Deploy

**`index.html`** — Dashboard completo com todas as seções existentes + nova seção INDICADORES NET

---

## 🎯 O que foi adicionado

### 1. Nova seção "INDICADORES NET" em cada vertical

Adicionada **dentro do sub-panel Transacional** de cada uma das 4 verticais:
- 🔵 Segurança → `#seg-indicadores-net`
- 🟢 Seguros → `#segu-indicadores-net`
- 🟡 Conteúdo → `#cont-indicadores-net`
- 🩷 Mulheres Positivas → `#mp-indicadores-net`

### 2. Conteúdo de cada seção INDICADORES NET

```
┌─ Banner explicativo (Cálculo de CHURN e NET)
│
├─ 6 KPIs Consolidados
│  ├─ CREATE Total
│  ├─ CANCEL Total
│  ├─ RENEW Total
│  ├─ SUSPEND Total
│  ├─ NET (CREATE − CANCEL)
│  └─ CHURN Rate (%)
│
├─ 📊 INDICADORES NET · POR OFERTA
│  └─ Tabela: Oferta | CREATE | CANCEL | RENEW | SUSPEND | NET | CHURN %
│     (Top 20 ofertas ordenadas por NET decrescente)
│
├─ 📊 INDICADORES NET · POR PARCEIRO
│  ├─ 🟢 TOP 10 Parceiros · CREATE
│  ├─ 🔴 TOP 10 Parceiros · CANCEL
│  └─ 📋 Todos os Parceiros · Consolidado (scrollable)
│
└─ 📊 INDICADORES NET · POR PLANO
   └─ Tabela com Top 30 planos (scrollable)
```

### 3. Sidebar atualizada

Cada vertical agora tem link **"📊 Indicadores NET"** no menu lateral, ao final das seções.

### 4. Navegação inteligente

Ao clicar em "📊 Indicadores NET" na sidebar:
- Se estiver na aba "Base Ativa", o sistema **automaticamente** alterna para "Transacional"
- Faz scroll suave até a seção

---

## 📊 Fórmulas Documentadas

Cada seção exibe explicitamente as fórmulas no topo:

```
📊 Cálculo de CHURN: CHURN (%) = CANCEL ÷ CREATE × 100
📊 Cálculo de NET:   NET = CREATE − CANCEL
```

E na tabela de Ofertas há repetição do cálculo no rodapé para reforço visual.

---

## 🎨 Estilo Mantido

- ✅ Mesma paleta de cores por vertical (seg/segu/cont/mp)
- ✅ Mesmas classes CSS já existentes (.t-kpi, .card, .dt, .al, etc.)
- ✅ Mesma fonte (IBM Plex Sans/Mono)
- ✅ Mesma estrutura de hierarquia visual (s-tag, s-title, s-sub, ct, cs)
- ✅ Cores semânticas em CHURN (verde < 30% / amarelo 30-70% / vermelho > 70%)
- ✅ Cores semânticas em NET (verde positivo / vermelho negativo)
- ✅ Tabelas responsivas com overflow-x e scroll quando necessário

---

## 📈 Dados Consolidados (por vertical)

### 🔵 Segurança
- **CREATE**: 49,82M | **CANCEL**: 41,04M | **NET**: 8,78M
- **CHURN Rate**: 82,38% ⚠️
- 7 ofertas · 20 parceiros · 57 planos

### 🟢 Seguros
- **CREATE**: 44,5K | **CANCEL**: 3,5K | **NET**: 41K
- **CHURN Rate**: 7,89% ✅ (Melhor performance!)
- 3 ofertas · 3 parceiros · 8 planos

### 🟡 Conteúdo
- **CREATE**: 245,0M | **CANCEL**: 168,4M | **NET**: 76,6M
- **CHURN Rate**: 68,74%
- 6 ofertas · 16 parceiros · 15 planos

### 🩷 Mulheres Positivas
- **CREATE**: 3,6M | **CANCEL**: 1,9M | **NET**: 1,7M
- **CHURN Rate**: 52,70%
- 1 oferta · 3 parceiros · 2 planos

---

## 🚀 Como fazer o Deploy

### Vercel (recomendado)
```bash
# Copiar para seu projeto
cp index.html /caminho/do/seu/projeto/

# Deploy
cd /caminho/do/seu/projeto/
vercel --prod
```

### GitHub
```bash
# Substituir o arquivo
cp index.html /caminho/do/repositorio/

# Commit
cd /caminho/do/repositorio/
git add index.html
git commit -m "feat: adiciona seção INDICADORES NET com CHURN e NET por vertical"
git push
```

### Local (teste)
Basta abrir `index.html` no navegador.

---

## ✅ Garantias

- ✅ **Zero remoção**: Tudo que existia no dashboard original foi mantido
- ✅ **Auto-contido**: Sem CDN, sem dependências externas (mesmo do original)
- ✅ **Mesma estrutura**: HTML balanceado igual ao original
- ✅ **Compatível**: Funciona com Vercel, GitHub Pages, Netlify, qualquer servidor estático
- ✅ **Responsivo**: Tabelas com scroll horizontal quando necessário
- ✅ **Performance**: HTML estático, carrega instantâneo

---

## 📦 Outros arquivos no /mnt/user-data/outputs/

Mantidos do processamento anterior caso queira reutilizar:

- `indicadores_net.json` — Dados estruturados em JSON
- `NET_*_ofertas.csv`, `NET_*_parceiros.csv`, `NET_*_planos.csv` — Dados em CSV para BI
- `html_net_*.html` — Snippets HTML isolados por vertical

---

**Data:** 15/05/2026  
**Versão:** Dashboard EXA Analytics v2 — com INDICADORES NET integrado  
**Período de dados:** jan/2022 a mai/2026  
