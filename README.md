# 🚀 Meu Blog Pessoal com Quarto

Bem-vindo ao repositório do meu blog pessoal! Este projeto foi desenvolvido utilizando o framework Quarto e é publicado automaticamente na web através do GitHub Pages.

O blog está no ar e pode ser acessado em:
https://digasx.github.io/blog-digasx/

# ✨ Sobre o Blog

Neste espaço, eu escrevo sobre tecnologia, programação, estudos e hobbies. O objetivo é compartilhar conhecimento e documentar meus aprendizados.

# 🔧 Tecnologias Utilizadas

- [Quarto](https://quarto.org/): A ferramenta principal para transformar arquivos Markdown em um site estático completo. Permite a inclusão de código executável (Python, R, etc.), equações LaTeX e muito mais.

- [GitHub Pages](https://pages.github.com/): Plataforma de hospedagem gratuita da Microsoft/GitHub, perfeita para sites estáticos.

- [GitHub Actions](https://github.com/features/actions): Automação que faz o "build" (renderização) do site e o publica no GitHub Pages toda vez que uma alteração é enviada para o repositório.

- Markdown: A linguagem de marcação simples e intuitiva usada para escrever todos os posts e páginas.

# 💻 Como Executar Localmente

Se você quiser testar o blog em sua máquina local ou fazer modificações, siga os passos abaixo.

Pré-requisitos:

- Você precisa ter o [Quarto CLI](https://quarto.org/docs/get-started/) instalado na sua máquina.

## Passos:

1. Clone o repositório:


`git clone https://github.com/digasx/blog-digasx.git`

`cd blog-digasx`

2. Inicie o servidor de preview:

O Quarto possui um servidor local com live-reload (atualiza o navegador automaticamente quando você salva um arquivo). Para iniciá-lo, execute:


`quarto preview`

# ✍️ Como Adicionar um Novo Post

O fluxo para criar um novo post é muito simples:

1. Navegue até o diretório `posts/` (ou o nome que você deu à pasta de postagens).

2. Crie uma nova pasta com um nome descritivo para o seu post (ex: `meu-primeiro-post`).

3. Dentro dessa nova pasta, crie um arquivo `index.qmd`.

4. Escreva o conteúdo do seu post neste arquivo usando Markdown. Não se esqueça de adicionar o cabeçalho YAML no início do arquivo:

    ```yaml
    ---
    title: "O Título do Seu Post"
    author: "Seu Nome"
    date: "2025-09-25" # Use o formato AAAA-MM-DD
    categories: [Tecnologia, Quarto] # Categorias para organização
    image: "imagem_capa.png" # Opcional: imagem de capa
    ---
    O conteúdo do seu post começa aqui...
    ```


5. Após commitar e enviar (`git push`) suas alterações para o branch principal (`main` ou `master`), a GitHub Action será acionada automaticamente para publicar o novo post.

# 📁 Estrutura do Projeto

```
.
├── .github/workflows/   # Contém a automação (GitHub Action) para publicação
├── _quarto.yml          # Arquivo principal de configuração do site (menus, tema, etc.)
├── index.qmd            # A página inicial (Home) do blog
├── about.qmd            # A página "Sobre"
├── posts/               # Diretório onde todos os posts do blog são armazenados
│   ├── meu-primeiro-post/
│   │   ├── index.qmd
│   │   └── imagem.png
│   └── ...
├── styles.css           # Arquivo para customizações de estilo (CSS)
└── README.md            # Este arquivo :)
```