# kanay-modern
# Kanay Modern - Site Moderno com Astro

Site moderno para Kanay baseado no template Odyssey com Astro. Lighthouse 100, performance otimizada e design responsivo.

## 🚀 Quick Start - Setup Local

```bash
# 1. Clonar o Odyssey como base
git clone https://github.com/cris-kracked/odyssey.git kanay-modern
cd kanay-modern

# 2. Remover histórico do Odyssey e reinicializar
rm -rf .git
git init
git add .
git commit -m "Initial commit: Odyssey template for Kanay Modern"

# 3. Adicionar o repositório remoto do kanay-modern
git remote add origin https://github.com/cris-kracked/kanay-modern.git
git branch -M main
git push -u origin main

# 4. Instalar dependências
npm install

# 5. Rodar localmente
npm run dev
```

## 📝 Customização - Kanay

### 1. Cores e Branding
Edite em `src/styles/globals.css`:
- Substitua cores do Odyssey pelas cores do Kanay
- Logo: `public/logo.png`

### 2. Conteúdo
Páginas em `src/pages/`:
- `index.astro` - Hero + Seções principais
- `blog/` - Para publicações

### 3. Componentes
Em `src/components/`:
- Adaptar texto, imagens e dados
- Manter estrutura do Odyssey

## 📋 Conteúdo do Kanay

**Hero:**
- Título: "Sua Riqueza Começa com Conhecimento Financeiro"
- Subtítulo: "Gestão • Consultoria • Educação Financeira"
- Descrição: "Com mais de 10 anos no mercado financeiro..."
- CTAs: WhatsApp + LinkedIn

**Serviços:**
1. Gestão Financeira Empresarial
2. Consultoria de Investimentos
3. Educação Financeira Corporativa

**Sobre:**
- Nome: Cristiano Cosme
- Descrição e experiência
- CTAs de contato

**Contato:**
- WhatsApp: +55 11 98637-7999
- LinkedIn: cristiano-cosme
- Email: contato@kanay.ia.br

## 🎨 Design Tokens

```typescript
// tailwind.config.ts
colors: {
  'primary': '#your-kanay-color',     // Substitua
  'secondary': '#secondary-color',
  'accent': '#accent-color',
}
```

## 📦 Deploy Vercel

```bash
# 1. Conectar com Vercel
vercel

# 2. Ou pelo dashboard: vercel.com
# - Importar repositório kanay-modern
# - Framework: Astro
# - Deploy automático em push
```

## 📊 Performance

- ✅ Lighthouse 100
- ✅ Zero JS desnecessário
- ✅ Imagens otimizadas
- ✅ Font loading performance

## 🔗 Links

- **Template Original**: [Odyssey](https://github.com/cris-kracked/odyssey)
- **Site Atual**: [kanay.ia.br](https://kanay.ia.br)
- **Demo**: (será preenchida após deploy)

## 📝 Próximos Passos

1. ✅ Clone e setup local
2. ✅ Adapte cores e logos
3. ✅ Edite conteúdo das seções
4. ✅ Teste localmente: `npm run dev`
5. ✅ Deploy: `vercel`

---

**Baseado em**: [Odyssey Theme](https://odyssey-theme.sapling.supply/)
**Para**: Kanay - Consultor Financeiro
