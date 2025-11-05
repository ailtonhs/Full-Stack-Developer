# Definindo o tamanho de um item da grade

## Layout em grid

Essa **grid-column** propriedade é usada para expandir um item da grade por várias colunas. Vamos definir essa propriedade para cada item da grade.
```html
  <div class="grid-container">
   <div class="grid-item item-1">Item</div>
   <div class="grid-item item-2">Item</div>
  </div>
```
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(3, 1fr);
 grid-template-rows: repeat(3, 1fr);
 background-color: #E0F6FF;
}

.item-1 {
 grid-column: span 2;
}

.item-2 {
grid-column: span 1;
}

.grid-item {
 background-color: #1E96FF;
 color: #FFFFFF;
 padding: 20px;
 margin: 5px;
}
```
Usamos o termo **span** para falar sobre o quanto expandimos um item da grade. Em código, **span 2** significa que estendemos o item da grade por duas colunas.
```css
.item-1 {
 grid-column: span 2;
}

.item-2 {
grid-column: span 1;
}
```
Se quisermos definir o tamanho de um item da grade ao longo das linhas, usamos a **grid-row** propriedade. Vamos definir essa propriedade para o primeiro item da grade.
```css

.item-1 {
 grid-column: span 2;
 
grid-row: span 3;
}

.item-2 {
 grid-column: span 1;
}
```
