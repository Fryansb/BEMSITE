# BEM Methodology Demo Site

Um site demonstrativo da metodologia BEM (Block Element Modifier) desenvolvido com Vue.js 3 e Vite, apresentando exemplos práticos em diferentes frameworks.

## 🚀 Tecnologias Utilizadas

- **Vue.js 3** - Framework JavaScript progressivo
- **Vite** - Build tool moderna e rápida
- **Bootstrap 5** - Framework CSS para estilização
- **Bootstrap Icons** - Conjunto completo de ícones
- **CSS3** - Estilos personalizados com glassmorphism

## 📋 Funcionalidades

- ✅ Demonstração interativa da metodologia BEM
- ✅ Exemplos de código para HTML, Vue.js, React, Angular e SCSS
- ✅ Interface responsiva com design moderno
- ✅ Modais interativos com explicações detalhadas
- ✅ Efeitos visuais com glassmorphism e gradientes
- ✅ Otimizado para deploy na Vercel

## 🎯 Sobre BEM

**BEM (Block Element Modifier)** é uma metodologia de nomenclatura CSS que ajuda a:

- 📦 **Block (Bloco)**: Componente independente e reutilizável
- 🧩 **Element (Elemento)**: Parte de um bloco que não pode existir sozinha
- 🎨 **Modifier (Modificador)**: Variação de um bloco ou elemento

### Exemplo de Nomenclatura BEM:

```css
/* Block */
.card { }

/* Elements */
.card__title { }
.card__content { }
.card__button { }

/* Modifiers */
.card--featured { }
.card__button--disabled { }
```

## 🛠️ Como Executar

### Pré-requisitos
- Node.js (versão 16 ou superior)
- npm ou yarn

### Instalação e Execução

```bash
# Clonar o repositório
git clone <url-do-repositorio>
cd BEMLINKEDINSITE

# Instalar dependências
npm install

# Executar em modo de desenvolvimento
npm run dev

# Build para produção
npm run build

# Preview da build de produção
npm run preview
```

## 📁 Estrutura do Projeto

```
BEMLINKEDINSITE/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   │   └── vue.svg
│   ├── components/
│   │   └── HelloWorld.vue (removido)
│   ├── App.vue
│   ├── main.js
│   └── style.css
├── .github/
│   └── copilot-instructions.md
├── package.json
├── vite.config.js
├── vercel.json
└── README.md
```

## 🌐 Deploy na Vercel

O projeto está configurado para deploy automático na Vercel:

1. **Conecte seu repositório** na Vercel
2. **Configure as variáveis** (se necessário)
3. **Deploy automático** acontece a cada push

### Configuração do Vercel (vercel.json):
- Build Command: `npm run build`
- Output Directory: `dist`
- Framework: `vite`

## 📚 Exemplos Incluídos

O site demonstra BEM em diferentes contextos:

1. **HTML Puro** - Estrutura semântica básica
2. **Vue.js** - Componentes reativos com Composition API
3. **React** - Componentes funcionais com hooks
4. **Angular** - Componentes com TypeScript
5. **SCSS** - Pré-processador com nesting BEM

## 🎨 Design System

- **Cores**: Gradiente azul/roxo com glassmorphism
- **Tipografia**: Segoe UI, system fonts
- **Ícones**: Bootstrap Icons
- **Layout**: Bootstrap Grid System
- **Animações**: Transições suaves CSS

## 👨‍💻 Desenvolvido por

**Ryan Vasconcelos**
- [GitHub](https://github.com/Fryansb)
- [LinkedIn](https://www.linkedin.com/in/ryan-vasconcelos-5b7776260/)

---

**LinkedIn Learning • 2025**

> Este projeto será implementado no projeto Print(MeAjuda) como demonstração da metodologia BEM.
#   B E M S I T E 
 
 