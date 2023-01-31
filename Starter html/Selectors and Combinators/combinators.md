# Combinators

Trabalham para buscar e combinar seletores a fim de aplicar uma estilização.

## Descendant combinator

* Identificado por um espaço entre os seletores.
* Busca um elemento dentro de outro.

```HTML
<body>

<article>
    <h2>Um Título</h2>
</article>

<article> 
    <h2>Outro Título</h2>
</article>

</body>
```

```CSS
body article h2 {
    color: red;
}
Neste caso, tanto o "Um título" como o "Outro Título" ficarão com a cor vermelha. Isso acontece, pois o CSS vai buscar todos os elementos <h2>, que estiverem dentro de um <article> que estiverem dentro de um <body>.
```

## Child Combinator
* identificado pelo sinal `>` entre dois seletores.
* Seleciona somente o elemento que é filho direto do pai
* Elementos depois do filho direto serão desconsiderados.
```CSS
body > ul > li
```
```HTML
<body>
    <ul>
        <li>Item 1</li>
        <ul>
            <li>Item 2</li>
        </ul>
        </ul>

</body>
```

```CSS
body > ul > li {
    color: blue;
}
```

## Adjacent sibling combinator

* Identificado pelo sinal de `+` entre dois seletores
* Seleciona somente o elemento do lado direito que é irmão direto na hierarquia.

```HTML
<h1>
Título   
</h1>

<p>Esse é um parágrafo</p>
<p>Esse é outro parágrafo</p>
<button>Um botão</button>
<button>Outro botão</button>
```

```CSS
h1 + p { 
    color: red;
}
Apenas o primeiro p será afetado. Pois ele é o irmão direto na hierarquia.
```

```CSS
button + button { 
    margin-left: 32px;    
}
```

## General sibling combinator

* Identificado pelo sinal `~` entre dois seletores
* Seleciona todos os elementos irmãos

```CSS
h1 ~ p {
    color: red;
}
Todos os p que estiverem ao lado do h1.
```