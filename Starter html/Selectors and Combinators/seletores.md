# Seletores

Conecta um elemento HTML com CSS a fim de alterar o elemento.

## Tipos

* ID Selector:
    - Um elemento que tenha um atributo `id`.
    - Cada `id` deve ser único.

    
    ```HTML    
    <h1 id="title"> Sou um Título </h1>  
    ```

    ```CSS
    #title {
        font-size: 12px;
        font-color: red;
    }

    Isso irá mexer com o atributo que tem o id title.       
    ```

    * Class Selector
    - Os elementos que contenham o atributo `class`.
    - Podemos ter uma ou mais classes.

    ```HTML
    <h1 id="title" class="yellow"> Oh your skin oh yeah your skin and bones. Turn into something beautiful... </h1>    
    ```
    ```CSS
    .yellow {
        font-size: 1.5em;
        font-weight: bold;
        font-color: yellow;
    }

    Todos elementos que possuírem a classe yellow receberam os efeitos aplicados do css.
    ```

    
