# Trabalhando com fontes

Tipografia transmite mensagem.
- Negrito
- Tamanho
- estilo
- Documentação: https://www.w3.org/TR/css-fonts-3
---

## Propriedades básicas de Fontes:

- font-family
- font-weight
- font-style
- font-size

## Font Family

- Tipo de fonte de um elemento
- Lista de fontes e ordem de prioridade
- inclui *fallback* [ algo que vai ser colocado no lugar caso o caminho da fonte não seja correto ].

```CSS
p {
    font-family: "Times New Roman", "Times", serif;
}
```
O caminho ideal é que haja a Times New Roman, se não tiver use a Times, se não tiver, então apresente alguma font serifada.

## Font Weight

- Peso da fonte


```CSS
p {
    font-weight: bold;
}
```

## Font Style

- O estilo da fonte

```CSS
p {
    font-style: italic;
}
```

## Font Size

- O tamanho da fonte

```CSS
    font-size: 12px;
```

## Web Fonts

- Fontes do sistema são as fontes que estão instaladas na sua máquina, mas que não necessariamente estarão instaladas na máquina do seu cliente.
- Fontes web são fontes fornecidas na web para importarmos para nossa aplicação. Exemplo: Google Fonts 

```HTML
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
</head>
```

Regra CSS para especificar a fonte exemplo. Cada fonte tem sua regra CSS.
```CSS
p {
    font-family: 'Roboto', sans-serif;
}
```

