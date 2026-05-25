# 📊 EXA Analytics Dashboard

Dashboard analítico unificado com Base Ativa + Indicadores NET (Transacional)

**Versão:** 2.0  
**Data de atualização:** 25/mai/2026  
**Mês de referência:** maio/2026

---

## 🚀 Deploy na Vercel

### Opção 1: Via CLI
```bash
# Instalar Vercel CLI (se ainda não tem)
npm i -g vercel

# Deploy
cd caminho/do/projeto
vercel --prod
```

### Opção 2: Via GitHub
1. Faça commit dos arquivos:
   ```bash
   git add .
   git commit -m "feat: atualiza dashboard com dados mai/2026"
   git push
   ```

2. No Vercel:
   - Conecte seu repositório
   - Deploy automático acontece

### Opção 3: Drag & Drop
1. Acesse [vercel.com/new](https://vercel.com/new)
2. Arraste esta pasta
3. Deploy instantâneo

---

## 📊 Dados Atualizados

### Base Ativa (maio/2026)
- **Segurança:** 469,2M assinaturas (21 parceiros · 8 ofertas)
- **Seguros:** 204K assinaturas (3 parceiros · 3 ofertas)
- **Conteúdo:** 2,42B assinaturas (16 parceiros · 6 ofertas)
- **Mulheres Positivas:** 49,6M assinaturas (3 parceiros · 1 oferta)
- **TOTAL:** ~2,94B assinaturas

### Indicadores NET (Transacional maio/2026)
- **Segurança:** CREATE 51,5M | CANCEL 42,7M | NET 8,8M | CHURN 82,91%
- **Seguros:** CREATE 46,7K | CANCEL 3,5K | NET 43,2K | CHURN 7,59% ✅
- **Conteúdo:** CREATE 253,3M | CANCEL 174,1M | NET 79,2M | CHURN 68,72%
- **Mulheres Positivas:** CREATE 3,8M | CANCEL 2,0M | NET 1,8M | CHURN 52,53%

---

## 📁 Estrutura do Projeto

```
/
├── index.html              ← Dashboard principal (601 KB)
├── vercel.json             ← Configuração Vercel
└── README.md               ← Este arquivo
```

---

## 🎯 Funcionalidades

### Base Ativa
- ✅ Overview com KPIs principais
- ✅ Análise por Produto Pai
- ✅ Análise por Oferta
- ✅ Análise por Parceiro
- ✅ Evolução Histórica (53 meses para Segurança)
- ✅ Sinais & Alertas

### Indicadores NET (Transacional)
- ✅ 6 KPIs consolidados (CREATE, CANCEL, RENEW, SUSPEND, NET, CHURN)
- ✅ NET por Oferta (tabela completa com CHURN)
- ✅ TOP 10 Parceiros por CREATE
- ✅ TOP 10 Parceiros por CANCEL
- ✅ Todos os Parceiros (consolidado)
- ✅ Análise por Plano

### Fórmulas Implementadas
```
CHURN (%) = CANCEL ÷ CREATE × 100
NET FLOW  = CREATE - CANCEL
```

---

## 🎨 Características

- ✅ **Self-contained:** Zero CDN, zero dependências externas
- ✅ **Responsivo:** Mobile + Desktop
- ✅ **4 Verticais:** Segurança, Seguros, Conteúdo, Mulheres Positivas
- ✅ **Dual View:** Base Ativa + Transacional (toggle)
- ✅ **Navegação:** Sidebar com scroll smooth
- ✅ **Cores semânticas:** Verde/Amarelo/Vermelho por threshold
- ✅ **Tabelas scrollable:** Overflow horizontal/vertical quando necessário

---

## 📈 Insights Críticos

### 🔴 ALERTAS
- **Segurança CHURN 82,91%** — Taxa muito alta, requer ação
- **Concentração TIM** — 98,8% da base de Segurança

### 🟢 OPORTUNIDADES
- **Seguros CHURN 7,59%** — Melhor vertical, modelo a replicar
- **Conteúdo** — 82,3% da base total (~2,42B)

---

## 🔄 Como Atualizar os Dados

### 1. Atualizar Base Ativa
Substitua os CSVs e rode:
```bash
python atualizar_base_ativa.py
```

### 2. Atualizar Transacional
Substitua os CSVs e rode:
```bash
cd /mnt/skills/user/dashboard-indicadores-net
python run_all.py --html index.html
```

### 3. Deploy
```bash
vercel --prod
```

---

## 📞 Suporte

- **Skill:** `/mnt/skills/user/dashboard-indicadores-net/`
- **Docs:** Ver SKILL.md, README.md, EXAMPLES.md na skill

---

## 📊 Histórico de Versões

### v2.0 (25/mai/2026)
- ✅ Base Ativa atualizada (maio/2026)
- ✅ Dados Transacionais atualizados (24-25/mai/2026)
- ✅ Indicadores NET integrados
- ✅ 4 verticais completas
- ✅ Total: ~2,94B assinaturas

### v1.0 (Original)
- Base Ativa inicial
- Gráficos estáticos

---

**Status:** ✅ Pronto para Produção  
**Deploy:** Vercel (recomendado)  
**Tecnologias:** HTML5 · CSS3 · JavaScript Vanilla  
**Tamanho:** 601 KB (otimizado)
