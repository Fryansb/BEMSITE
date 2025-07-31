<template>
  <div id="app">
    <!-- Header -->
    <div class="container py-5">
      <div class="text-center mb-5">
        <h1 class="display-3 fw-bold hero-title mb-3">BEM Methodology</h1>
        <p class="lead mb-4 opacity-90">Organize seu CSS como um profissional</p>
      </div>

      <!-- Cards Grid -->
      <div class="row g-4">
        <!-- Card 1: BEM Intro -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-info-circle-fill display-4 text-info"></i>
              </div>
              <h5 class="card-title text-white mb-3">Introdução ao BEM</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Block Element Modifier: uma metodologia que nos ajuda a criar componentes reutilizáveis e código compartilhável no front-end.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('bem')">
                  <i class="bi bi-code-slash"></i> Ver Estrutura
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('bemAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>

        <!-- Card 2: HTML -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-file-earmark-code display-4 text-warning"></i>
              </div>
              <h5 class="card-title text-white mb-3">HTML Puro</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Estrutura semântica com nomenclatura BEM para criar uma base sólida e acessível.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('html')">
                  <i class="bi bi-code-slash"></i> Ver Código
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('htmlAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>

        <!-- Card 3: Vue -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-layers-fill display-4 text-success"></i>
              </div>
              <h5 class="card-title text-white mb-3">Vue.js</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Framework progressivo que adota BEM para criar componentes organizados e escaláveis.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('vue')">
                  <i class="bi bi-code-slash"></i> Ver Código
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('vueAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>

        <!-- Card 4: React -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-bootstrap-reboot display-4 text-primary"></i>
              </div>
              <h5 class="card-title text-white mb-3">React</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Biblioteca que se beneficia da metodologia BEM para manter components limpos e reutilizáveis.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('react')">
                  <i class="bi bi-code-slash"></i> Ver Código
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('reactAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>

        <!-- Card 5: Angular -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-gear-fill display-4 text-danger"></i>
              </div>
              <h5 class="card-title text-white mb-3">Angular</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Framework robusto que utiliza BEM para criar aplicações enterprise escaláveis.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('angular')">
                  <i class="bi bi-code-slash"></i> Ver Código
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('angularAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>

        <!-- Card 6: SCSS -->
        <div class="col-md-6 col-lg-4">
          <div class="card h-100">
            <div class="card-body d-flex flex-column text-center">
              <div class="mb-3">
                <i class="bi bi-palette-fill display-4 text-info"></i>
              </div>
              <h5 class="card-title text-white mb-3">SCSS/Sass</h5>
              <p class="card-text flex-grow-1 opacity-90">
                Pré-processador que potencializa BEM com mixins, variáveis e estrutura aninhada.
              </p>
              <div class="mt-auto">
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('scss')">
                  <i class="bi bi-code-slash"></i> Ver Código
                </button>
                <button class="btn btn-outline-light btn-sm me-2 mb-2 btn-code" @click="openModal('scssAbout')">
                  <i class="bi bi-info-circle"></i> Ler Sobre
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Modal Simples para Teste -->
    <div v-if="showModal" class="modal-overlay" @click="closeModal">
      <div class="modal-content-custom" @click.stop>
        <div class="modal-header-custom">
          <h5 class="text-white">{{ currentModal.title }}</h5>
          <button @click="closeModal" class="btn-close-custom">&times;</button>
        </div>
        <div class="modal-body-custom">
          <div v-html="currentModal.content"></div>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <footer class="container-fluid footer-glass mt-5 py-4">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-8">
            <p class="mb-2 text-white opacity-90">
              <i class="bi bi-heart-fill text-danger"></i>
              <strong>BEM Methodology Demo</strong> - Demonstração prática da metodologia CSS BEM em diferentes frameworks
            </p>
            <p class="mb-0 text-white opacity-75">
              Este site demonstra como aplicar a metodologia BEM (Block Element Modifier) em HTML, Vue.js, React, Angular e SCSS, 
              mostrando exemplos práticos de código e explicações detalhadas para cada abordagem. Esta pagina sera implementada no projeto Print(MeAjuda).
            </p>
          </div>
          <div class="col-md-4 text-md-end">
            <div class="mb-2">
              <small class="text-white opacity-75 d-block">Desenvolvido por</small>
              <strong class="text-white">Ryan Vasconcelos</strong>
            </div>
            <div class="d-flex justify-content-md-end gap-3">
              <a href="https://github.com/Fryansb" target="_blank" class="btn btn-outline-light btn-sm">
                <i class="bi bi-github"></i> GitHub
              </a>
              <a href="https://www.linkedin.com/in/ryan-vasconcelos-5b7776260/" target="_blank" class="btn btn-outline-light btn-sm">
                <i class="bi bi-linkedin"></i> LinkedIn
              </a>
            </div>
            <small class="text-white opacity-50 d-block mt-2">
              LinkedIn Learning • 2025
            </small>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue'

const showModal = ref(false)
const activeModal = ref('')

const modals = {
  bem: {
    title: 'Estrutura BEM',
    content: `
      <div class="text-white">
        <h6 class="text-info">📦 Block (Bloco)</h6>
        <pre class="bg-dark text-light p-3 rounded mb-3"><code>.card { }</code></pre>
        
        <h6 class="text-warning">🧩 Element (Elemento)</h6>
        <pre class="bg-dark text-light p-3 rounded mb-3"><code>.card__title { }
.card__content { }
.card__button { }</code></pre>
        
        <h6 class="text-success">🎨 Modifier (Modificador)</h6>
        <pre class="bg-dark text-light p-3 rounded"><code>.card--highlighted { }
.card__button--disabled { }</code></pre>
      </div>
    `
  },
  bemAbout: {
    title: 'Sobre BEM Methodology',
    content: `
      <div class="text-white">
        <h6 class="text-info">🎯 O que é BEM?</h6>
        <p class="mb-3">BEM (Block Element Modifier) é uma metodologia de nomenclatura CSS criada pela Yandex que organiza código de forma previsível e escalável.</p>
        
        <h6 class="text-warning">✨ Principais Benefícios:</h6>
        <ul class="mb-3">
          <li><strong>Clareza:</strong> Nomes descritivos facilitam manutenção</li>
          <li><strong>Modularidade:</strong> Componentes independentes e reutilizáveis</li>
          <li><strong>Escalabilidade:</strong> Ideal para projetos grandes</li>
        </ul>
      </div>
    `
  },
  html: {
    title: 'HTML com BEM',
    content: `
      <pre class="bg-dark text-light p-3 rounded"><code>&lt;div class="card card--featured"&gt;
  &lt;header class="card__header"&gt;
    &lt;h2 class="card__title"&gt;Título do Card&lt;/h2&gt;
  &lt;/header&gt;
  &lt;main class="card__content"&gt;
    &lt;p class="card__description"&gt;Descrição do conteúdo&lt;/p&gt;
  &lt;/main&gt;
  &lt;footer class="card__footer"&gt;
    &lt;button class="card__button card__button--primary"&gt;
      Ação Principal
    &lt;/button&gt;
  &lt;/footer&gt;
&lt;/div&gt;</code></pre>
    `
  },
  htmlAbout: {
    title: 'HTML Semântico com BEM',
    content: `
      <div class="text-white">
        <h6 class="text-warning">📝 HTML Semântico</h6>
        <p class="mb-3">Combinar HTML semântico com BEM cria uma base sólida para aplicações web acessíveis e bem estruturadas.</p>
        
        <h6 class="text-info">🎯 Vantagens:</h6>
        <ul>
          <li>Melhor SEO e acessibilidade</li>
          <li>Código mais legível e manutenível</li>
          <li>Facilita desenvolvimento em equipe</li>
        </ul>
      </div>
    `
  },
  vue: {
    title: 'Vue.js com BEM',
    content: `
      <pre class="bg-dark text-light p-3 rounded"><code>&lt;template&gt;
  &lt;div class="product-card product-card--featured"&gt;
    &lt;h3 class="product-card__title"&gt;{{ product.name }}&lt;/h3&gt;
    &lt;p class="product-card__price"&gt;{{ product.price }}&lt;/p&gt;
    &lt;button 
      @click="addToCart"
      class="product-card__button"
      :class="{ 'product-card__button--loading': isLoading }"
    &gt;
      {{ isLoading ? 'Adicionando...' : 'Adicionar ao Carrinho' }}
    &lt;/button&gt;
  &lt;/div&gt;
&lt;/template&gt;

&lt;script setup&gt;
import { ref } from 'vue'
const isLoading = ref(false)
&lt;/script&gt;</code></pre>
    `
  },
  vueAbout: {
    title: 'Vue.js e BEM',
    content: `
      <div class="text-white">
        <h6 class="text-success">🚀 Vue.js Framework</h6>
        <p class="mb-3">Vue.js é um framework progressivo que se integra perfeitamente com a metodologia BEM para criar aplicações escaláveis.</p>
        
        <h6 class="text-info">💡 Por que BEM + Vue?</h6>
        <ul>
          <li>Componentização natural combina com blocos BEM</li>
          <li>Scoped CSS previne vazamentos de estilo</li>
          <li>Reatividade facilita modificadores dinâmicos</li>
        </ul>
      </div>
    `
  },
  react: {
    title: 'React com BEM',
    content: `
      <pre class="bg-dark text-light p-3 rounded"><code>const ProductCard = ({ product, featured = false }) =&gt; {
  const [isLoading, setIsLoading] = useState(false);
  
  const cardClasses = [
    'product-card',
    featured ? 'product-card--featured' : ''
  ].filter(Boolean).join(' ');
  
  return (
    &lt;div className={cardClasses}&gt;
      &lt;h3 className="product-card__title"&gt;{product.name}&lt;/h3&gt;
      &lt;p className="product-card__price"&gt;{product.price}&lt;/p&gt;
      &lt;button 
        onClick={handleAddToCart}
        className="product-card__button"
      &gt;
        {isLoading ? 'Adicionando...' : 'Adicionar'}
      &lt;/button&gt;
    &lt;/div&gt;
  );
};</code></pre>
    `
  },
  reactAbout: {
    title: 'React e BEM',
    content: `
      <div class="text-white">
        <h6 class="text-primary">⚛️ React Library</h6>
        <p class="mb-3">React + BEM criam uma combinação poderosa para desenvolvimento de interfaces de usuário componentizadas e escaláveis.</p>
        
        <h6 class="text-info">🎯 Vantagens da Combinação:</h6>
        <ul>
          <li>Componentes React = Blocos BEM naturalmente</li>
          <li>Props facilitam modificadores dinâmicos</li>
          <li>CSS-in-JS ou CSS Modules com BEM</li>
        </ul>
      </div>
    `
  },
  angular: {
    title: 'Angular com BEM',
    content: `
      <pre class="bg-dark text-light p-3 rounded"><code>@Component({
  selector: 'app-product-card',
  template: \`
    &lt;div [ngClass]="cardClasses"&gt;
      &lt;h3 class="product-card__title"&gt;{{ product.name }}&lt;/h3&gt;
      &lt;p class="product-card__price"&gt;{{ product.price | currency }}&lt;/p&gt;
      &lt;button 
        (click)="addToCart()"
        [ngClass]="buttonClasses"
      &gt;
        {{ isLoading ? 'Adicionando...' : 'Adicionar ao Carrinho' }}
      &lt;/button&gt;
    &lt;/div&gt;
  \`
})
export class ProductCardComponent {
  @Input() product: any;
  @Input() featured: boolean = false;
}</code></pre>
    `
  },
  angularAbout: {
    title: 'Angular e BEM',
    content: `
      <div class="text-white">
        <h6 class="text-danger">🅰️ Angular Framework</h6>
        <p class="mb-3">Angular oferece ferramentas robustas que se complementam perfeitamente com BEM para aplicações enterprise.</p>
        
        <h6 class="text-info">🏢 Ideal para Enterprise:</h6>
        <ul>
          <li>TypeScript + BEM = código type-safe e bem estruturado</li>
          <li>Angular CLI gera componentes com estrutura BEM</li>
          <li>ViewEncapsulation para escopos de CSS</li>
        </ul>
      </div>
    `
  },
  scss: {
    title: 'SCSS com BEM',
    content: `
      <pre class="bg-dark text-light p-3 rounded"><code>$primary-color: #007bff;
$border-radius: 8px;

.product-card {
  background: white;
  border-radius: $border-radius;
  transition: transform 0.3s ease;
  
  &:hover {
    transform: translateY(-2px);
  }
  
  &--featured {
    border: 2px solid $primary-color;
  }
  
  &__title {
    font-size: 1.25rem;
    color: #333;
  }
  
  &__button {
    background: $primary-color;
    color: white;
    padding: 0.75rem 1rem;
    
    &:hover {
      background: darken($primary-color, 10%);
    }
    
    &--loading {
      opacity: 0.7;
      cursor: not-allowed;
    }
  }
}</code></pre>
    `
  },
  scssAbout: {
    title: 'SCSS/Sass e BEM',
    content: `
      <div class="text-white">
        <h6 class="text-info">🎨 SCSS/Sass Preprocessor</h6>
        <p class="mb-3">SCSS potencializa BEM com recursos avançados como nesting, mixins e variáveis para código CSS mais organizado.</p>
        
        <h6 class="text-warning">🚀 Superpoderes do SCSS + BEM:</h6>
        <ul>
          <li>Nesting natural reflete estrutura BEM</li>
          <li>Variáveis para manter consistência</li>
          <li>Mixins para reutilizar modificadores</li>
          <li>Functions para lógica complexa</li>
        </ul>
      </div>
    `
  }
}

const currentModal = computed(() => {
  return modals[activeModal.value] || { title: '', content: '' }
})

const openModal = (modalType) => {
  activeModal.value = modalType
  showModal.value = true
}

const closeModal = () => {
  showModal.value = false
  activeModal.value = ''
}
</script>

<style scoped>
.modal-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.8);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1050;
}

.modal-content-custom {
  background: rgba(30, 30, 30, 0.95);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 20px;
  max-width: 800px;
  width: 90%;
  max-height: 80vh;
  overflow-y: auto;
}

.modal-header-custom {
  padding: 1.5rem 1.5rem 1rem 1.5rem;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.modal-body-custom {
  padding: 1.5rem;
}

.btn-close-custom {
  background: none;
  border: none;
  color: white;
  font-size: 1.5rem;
  cursor: pointer;
  opacity: 0.7;
}

.btn-close-custom:hover {
  opacity: 1;
}
</style>
