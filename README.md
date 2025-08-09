# VidFlow

Uma plataforma de vídeos responsiva inspirada no YouTube, desenvolvida como projeto de estudo em desenvolvimento Front-end.

## 📋 Sobre o Projeto

VidFlow é uma aplicação web que simula uma plataforma de compartilhamento de vídeos, com interface moderna e responsiva. O projeto demonstra competências em HTML5, CSS3 e JavaScript, incluindo consumo de APIs, manipulação do DOM e design responsivo.

## 🚀 Funcionalidades

- **Catálogo de Vídeos**: Exibição dinâmica de vídeos organizados em grid responsivo
- **Sistema de Busca**: Filtro em tempo real por título dos vídeos
- **Filtros por Categoria**: Navegação por categorias como Programação, Mobile, Data Science, etc.
- **Design Responsivo**: Interface adaptável para desktop, tablet e mobile
- **Modo Claro/Escuro**: Toggle para alternar entre temas
- **Menu Lateral**: Navegação intuitiva com ícones e labels

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e acessível
- **CSS3**: Estilização avançada com Flexbox, Grid e Media Queries
- **JavaScript ES6+**: Manipulação do DOM, consumo de API e interatividade
- **Fetch API**: Requisições assíncronas para carregar dados dos vídeos
- **JSON**: Estrutura de dados para armazenamento das informações dos vídeos

## 📁 Estrutura do Projeto

```
vidflow/
├── index.html
├── script.js
├── css/
│   ├── estilos.css
│   ├── flexbox.css
│   └── reset.css
├── img/
│   ├── topbar/
│   ├── sidebar/
│   └── VidFlow--Logo-light-mode.png
└── videos.json
```

## 🎯 Principais Implementações

### 1. Consumo de API
```javascript
async function buscarEMostrarVideos() {
  try {
    const buscaAPI = await fetch("http://localhost:3000/videos");
    const videos = await buscaAPI.json();
    // Processamento dos dados...
  } catch (error) {
    // Tratamento de erros
  }
}
```

### 2. Sistema de Filtros
- **Por Texto**: Filtro em tempo real através da barra de pesquisa
- **Por Categoria**: Filtros predefinidos para diferentes tipos de conteúdo

### 3. Design Responsivo
- **Mobile-first**: Desenvolvimento iniciado para dispositivos móveis
- **Breakpoints**: 834px, 1156px e 1440px para diferentes layouts
- **Grid System**: Layout flexível para os cards de vídeos

## 🎨 Design System

### Paleta de Cores
```css
--azul-profundo: #01080e;
--azul-escuro: #041832;
--azul-medio: #144480;
--azul-destaque-light: #1875e9;
--cinza-escuro: #222222;
--cinza-claro: #f2f2f2;
--branco: #ffffff;
```

### Tipografia
- **Família**: Roboto, Arial, Helvetica, sans-serif
- **Tamanhos**: 14px (base), 16px (elementos de destaque)

## 🔧 Como Executar

1. Clone o repositório
```bash
git clone [url-do-repositorio]
```

2. Instale um servidor local (ex: json-server para servir o JSON)
```bash
npm install -g json-server
json-server --watch videos.json --port 3000
```

3. Abra o `index.html` no navegador ou sirva através de um servidor local

## 📱 Responsividade

### Mobile (até 834px)
- Menu inferior fixo
- Layout single-column
- Barra de pesquisa oculta

### Tablet (834px - 1440px)
- Menu lateral compacto
- Grid de vídeos adaptativo
- Barra de pesquisa visível

### Desktop (1440px+)
- Menu lateral expandido
- Grid otimizado para telas grandes
- Todas as funcionalidades visíveis

## 🎓 Conceitos Aplicados

- **API REST**: Consumo de dados através de requisições HTTP
- **Async/Await**: Programação assíncrona moderna
- **Event Listeners**: Gerenciamento de eventos do usuário
- **DOM Manipulation**: Criação dinâmica de elementos
- **Error Handling**: Tratamento de erros e casos excepcionais
- **CSS Grid e Flexbox**: Layouts modernos e flexíveis
- **Media Queries**: Adaptação para diferentes dispositivos


## 👨‍💻 Autor

**Mauricio Grass de Bronstein**

Desenvolvedor Front-end em formação, focado em criar experiências web modernas e responsivas utilizando as melhores práticas de desenvolvimento.

---

Este projeto demonstra competências essenciais em desenvolvimento Front-end e serve como base sólida para projetos mais complexos. A aplicação combina design moderno com código limpo e funcionalidades robustas.
