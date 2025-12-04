# Kanay Modern - Guia de Implementação Passo a Passo

## 🚀 Método Rápido (Recomendado)

Este é o caminho mais rápido para transformar o Kanay no template Odyssey moderno.

### Passo 1: Clone o Odyssey Localmente

```bash
# No seu terminal, na pasta C:\COMUM (ou seu diretório de desenvolvimento)
git clone https://github.com/cris-kracked/odyssey.git kanay-modern
cd kanay-modern
```

### Passo 2: Remova o Git do Odyssey e Reinicialize

```bash
# Remove o histórico do Odyssey
rm -rf .git

# Reinicializa como novo repositório
git init
git add .
git commit -m "Initial commit: Odyssey template for Kanay Modern"
```

### Passo 3: Conecte ao Repositório kanay-modern

```bash
# Adiciona o repositório remoto
git remote add origin https://github.com/cris-kracked/kanay-modern.git

# Muda a branch para main
git branch -M main

# Faz o push inicial
git push -u origin main
```

### Passo 4: Instale as Dependências

```bash
npm install
```

### Passo 5: Verifique que tudo funciona

```bash
npm run dev
# Deve abrir em http://localhost:3000 ou http://localhost:4321
```

---

## 🎨 Customização do Kanay

### 1. Adapte as Cores (Design Tokens)

**Arquivo**: `src/styles/globals.css` ou `tailwind.config.ts`

```css
/* Substituía as cores do Odyssey pelas do Kanay */
--color-primary: #your-kanay-brand-color;
--color-secondary: #your-secondary;
--color-accent: #your-accent;
```

### 2. Logo

**Arquivo**: `public/logo.png` (ou `public/logo-dark.png`)

Substituía as imagens do Odyssey pela logo do Kanay.

### 3. Atualize a Página Principal

**Arquivo**: `src/pages/index.astro`

Edite os seguintes componentes:

#### Hero Section
```astro
<Hero
  title="Sua Riqueza Começa com Conhecimento Financeiro"
  subTitle="Gestão • Consultoria • Educação Financeira"
  description="Com mais de 10 anos no mercado financeiro, ajudo empresas e pessoas a conquistarem estabilidade e crescimento through estrategias financeiras comprovadas."
/>
```

#### Seção de Serviços

Adapte com os 3 serviços do Kanay:

1. **Gestão Financeira Empresarial**
   - Ícone: 💼 ou uma imagem
   - Descrição: "Planejamento financeiro estratégico, controle de fluxo de caixa..."

2. **Consultoria de Investimentos**
   - Ícone: 📊 ou uma imagem
   - Descrição: "Análise de mercado, diversificação de portfólio..."

3. **Educação Financeira Corporativa**
   - Ícone: 🎓 ou uma imagem
   - Descrição: "Treinamentos e workshops para colaboradores..."

#### Seção Sobre

```astro
<section>
  <h2>Sobre Cristiano Cosme</h2>
  <p>Profissional com expertise em análise financeira, certificado e apaixonado por educação financeira. Com mais de 10 anos no mercado, já ajudei centenas de empresas e pessoas.</p>
</section>
```

#### Seção de Contato

```astro
<ContactForm
  email="contato@kanay.ia.br"
  phone="+55 11 98637-7999"
  linkedin="https://www.linkedin.com/in/cristiano-cosme/"
/>
```

### 4. Atualize os Metadados

**Arquivo**: `src/config.ts`

```typescript
export const SITE_TITLE = "Kanay - Consultor Financeiro";
export const SITE_DESCRIPTION = "Gestão, Consultoria e Educação Financeira";
export const SITE_URL = "https://kanay-modern.vercel.app";
```

### 5. Ajuste o astro.config.mjs

```javascript
export default defineConfig({
  site: 'https://kanay-modern.vercel.app',
  integrations: [
    image(),
    sitemap(),
    robotsTxt(),
  ],
});
```

---

## 🧹 Teste Localmente

```bash
# Rode o servidor de desenvolvimento
npm run dev

# Ou faa o build para produção
npm run build
npm run preview
```

---

## 📤 Deploy na Vercel

### Opção 1: Via CLI (Recomendado)

```bash
vercel
# Responda as perguntas do wizard
# Framework: Astro
# Build Command: npm run build
# Output Directory: dist
```

### Opção 2: Via Dashboard

1. Vá para https://vercel.com
2. Clique em "New Project"
3. Selecione o repositório `kanay-modern`
4. Vercel detectará Astro automaticamente
5. Configure as variáveis de ambiente (se necessário)
6. Clique em "Deploy"

---

## 📝 Estrutura de Pastas

```
kanay-modern/
├── src/
│   ├── pages/
│   │   ├── index.astro          # Página principal
│   │   └── blog/                # Blog (opcional)
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Services.astro
│   │   ├── About.astro
│   │   └── Contact.astro
│   ├── styles/
│   │   └── globals.css          # Estilos globais
│   └── config.ts                # Configurações
├── public/
│   ├── logo.png                 # Logo do Kanay
│   └── images/                  # Imagens
├── astro.config.mjs             # Configuração Astro
├── tailwind.config.ts           # Tailwind CSS
├── package.json
└── README.md
```

---

## ✅ Checklist Final

- [ ] Clone do Odyssey concluído
- [ ] Repositório conectado a `kanay-modern`
- [ ] Depências instaladas (`npm install`)
- [ ] Cores customizadas
- [ ] Logo atualizada
- [ ] Conteúdo do Kanay adicionado
- [ ] Página testada localmente (`npm run dev`)
- [ ] Deploy na Vercel realizado
- [ ] URL de produção configurada
- [ ] Domínio custom apontando para Vercel (opcional)

---

## 📞 Suporte

Se tiver dúvidas:
- Veja o README.md
- Verifique a documentação do [Odyssey](https://odyssey-theme.sapling.supply/)
- Verifique a documentação do [Astro](https://docs.astro.build)

---

**Bom trabalho! 🚀**
