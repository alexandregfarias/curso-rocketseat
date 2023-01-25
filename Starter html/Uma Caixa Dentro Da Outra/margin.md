## Margin

Espaços entre os elementos.

- margin-top | margin-right | margin-bottom | margin-left
- values: `<lenght>` | `<percentage>` | `auto`

```css

div {
    /* shorthand */
    margin: 12px 16px 10px 4px; [top, right, bottom, left]
    margin: 12px 16px 0;
    margin: 8px 16px;
    margin: 8px
    margin: top right bottom left
} 

```
* Cuidado com margin collapsing (top se junta ao bottom)