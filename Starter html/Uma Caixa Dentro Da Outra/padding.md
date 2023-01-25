## Padding

Preenchimento interno da caixa

-padding-top/right/bottom/left

-values `<lenght>` | `<percentage>` | `auto`

```css 
/*shorthand*/
padding: 12px 16px 10px 4px; [top, right, bottom, left]
padding: 12px 16px 10px; [top, right&&left, bottom]
padding: 12px 8px; [top&&bottom, left&&right]
padding: 12px; [top&&bottom&&left&&right]
```

* O padding poderá causar diferença na largura de um elemento por conta do box-sizing.