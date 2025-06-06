# 📦 Projeto Front-End Base

Este é um template de projeto front-end utilizando **HTML**, **CSS/SASS** e **JavaScript** puro, com uma estrutura de pastas organizada para facilitar a escalabilidade e manutenção.

## 📁 Estrutura de Pastas

/meu-projeto
│
├── 📁 node_modules/      **Instalado automaticamente com npm install**
├── 📁 src/               **Arquivos-fonte principais**
│ ├── 📁 assets/          **Imagens, fontes e ícones**
│ │ ├── 📁 images/
│ │ ├── 📁 fonts/
│ │ └── 📁 icons/
│ │
│ ├── 📁 css/             **CSS compilado (output do SASS)**
│ │ └── main.css
│ │
│ ├── 📁 sass/            **Arquivos SASS organizados**
│ │ ├── 📁 components/    **Botões, cards, formulários, etc.**
│ │ ├── 📁 layout/        **Grid, header, footer, sidebar**
│ │ ├── 📁 pages/         **Estilos específicos por página**
│ │ ├── 📁 themes/        **Suporte a temas (light, dark)**
│ │ ├── 📁 Utilities/     **Mixins, functions e Helpers**
│ │ └── main.scss         **Arquivo que importa todos os outros**
│ │
│ ├── 📁 js/              **Scripts JavaScript**
│ │ ├── 📁 modules/       **Funções reutilizáveis e helpers**
│ │ ├── 📁 pages/         **Scripts específicos por página**
│ │ └── main.js
│ │
│ ├── 📁 components/      **Componentes HTML reutilizáveis (ex: navbar)**
│ │
│ ├── 📁 pages/           **Páginas HTML**
│ │ ├── index.html
│ │ └── contato.html
│ │
│ └── 📁 data/            **Dados simulados (ex: .json para testes)**
│
├── 📁 dist/              **Arquivos finais (prontos para deploy)**
│
├── .gitignore
├── package.json          **Configurações de build/scripts (opcional)**
├── README.md
└── index.html            **Entrada principal ou redirecionamento**


## ✅ Boas Práticas

- **Modularização do SASS**:                  Divida os estilos por responsabilidade e mantenha `main.scss` como centralizador.
- **Separação de componentes vs. páginas**:   Componentes genéricos vão em `sass/components`, estilos específicos em `sass/pages`.
- **JavaScript modular**:                     Use funções reutilizáveis e evite lógica inline no HTML.
- **Build automatizado (opcional)**:          Use `npm` com ferramentas como `sass`, `vite`, `webpack` ou `gulp` para compilar, minificar e servir os arquivos.
- **HTML limpo e organizado**:                Prefira carregar componentes HTML via JS (ex: `fetch`) e mantenha o HTML o mais semântico possível.
- **Pasta `dist/` separada**:                 Use para arquivos finais de produção.
- **Padronização do código**:                 Use `stylelint`, `eslint` e `prettier` para manter qualidade e consistência.