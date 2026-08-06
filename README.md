# Painel RB

Página pessoal com os links que uso no dia a dia, organizados por categoria. Hospedado gratuitamente no GitHub Pages.

🔗 **Site publicado:** `https://seu-usuario.github.io/nome-do-repositorio/`
*(atualize esse link aqui depois de ativar o GitHub Pages)*

## O que tem aqui

Um único arquivo `index.html`, sem dependências externas de build — é só HTML, CSS e JavaScript puro. Funciona direto no navegador, sem precisar instalar nada.

**Categorias atuais:**
- Trabalho
- Pessoal
- Estudo
- Sistema
- Infraestrutura
- Favoritos

Cada uma tem sua própria cor e todos os links mostram o ícone (favicon) do site automaticamente.

## Como editar

Tudo fica dentro da tag `<script>`, no final do `index.html`.

### Adicionar ou remover um link

Procure o array `links` e adicione uma linha seguindo o formato:

```js
{ categoria: "trabalho", nome: "Nome do site", desc: "descrição curta", url: "https://exemplo.com" },
```

O campo `categoria` precisa ser exatamente igual ao `id` de alguma categoria da lista `categorias` (ver abaixo).

### Adicionar uma categoria nova

Procure o array `categorias`, no início do script, e adicione uma linha:

```js
{ id: "nova-categoria", nome: "Nome Exibido", cor: "#hexadecimal" },
```

O `id` é o valor que você vai usar no campo `categoria` dos links. A seção aparece automaticamente na página, sem precisar editar o HTML.

### Onde editar

- Direto pelo site do GitHub: abra o `index.html` no repositório e clique no ícone de lápis (editar).
- Ou edite localmente e suba de novo pelo "Add file → Upload files".

Qualquer alteração salva atualiza o site publicado em poucos segundos, automaticamente.

## Publicação (GitHub Pages)

1. Repositório público no GitHub, com o `index.html` na raiz.
2. Settings → Pages → Deploy from a branch → branch `main`, pasta `/ (root)`.
3. O site fica em `https://seu-usuario.github.io/nome-do-repositorio/`.

## Notas

- Os ícones dos links são buscados automaticamente via favicon do site. Se algum site não tiver favicon, o painel mostra a primeira letra do nome no lugar.
- Atalho de teclado: `/` foca a busca, `Esc` limpa.
