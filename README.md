# GitHub Pages Lab

Site estático interativo em português para explorar recursos que podem ser publicados no GitHub Pages.

## Conteúdo
- Editor Markdown com pré-visualização ao vivo (Marked + DOMPurify)
- Blocos de código com realce (Highlight.js)
- Diagramas Mermaid
- Fórmulas matemáticas com MathJax
- Viewport 3D com controles, geometria selecionável e wireframe (Three.js)
- Gráficos (Chart.js)
- Tabela com filtro
- Catálogo pesquisável de recursos
- Exemplos de alertas, checklists, conteúdo expansível, responsividade e animação CSS

## Publicar no GitHub Pages
1. Crie um repositório GitHub.
2. Envie `index.html` e `README.md` para a raiz da branch `main`.
3. No repositório, vá a **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Selecione `main` e `/(root)` e clique em **Save**.
6. Aguarde o deploy e abra a URL exibida na página de configuração do Pages.

## Dependências
As bibliotecas são carregadas por CDN:
- Marked
- DOMPurify
- Highlight.js
- Mermaid
- MathJax
- Three.js
- Chart.js

É necessária conexão com a internet para carregar as bibliotecas externas. Para operação offline, hospede versões locais das bibliotecas, respeitando as respectivas licenças.

## Segurança
A pré-visualização Markdown sanitiza HTML com DOMPurify. Ainda assim, não use este laboratório para renderizar conteúdo não confiável em produção sem revisão. Nunca coloque tokens, senhas ou credenciais no JavaScript público.

## Limites
GitHub Pages hospeda conteúdo estático; não executa backend próprio. Dados e gráficos são exemplos fictícios. O motor 3D renderiza geometria gerada no browser, não depende do visualizador STL nativo do GitHub.
