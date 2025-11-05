# Grid Gaps

Por padrão, os itens da grade não têm espaço entre si. Vamos aprender a maneira correta de adicionar espaços entre os itens da grade.

Para criar espaços entre os itens da grade, usamos **gaps**. As gaps são diferentes das margens, que adicionam espaço em todos os lados de um item.

Para criar espaçamento iguais entre as linhas da grade, usamos a **row-gap** propriedade.
```html
 <div class="grid-container">
   <div class="grid-item">1</div>
   <div class="grid-item">2</div>
   <div class="grid-item">3</div>
   <div class="grid-item">4</div>
   <div class="grid-item">5</div>
   <div class="grid-item">6</div>
  </div>
  ```
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(2, auto);
 background-color: #E0F6FF;
 row-gap: 5px;
}

.grid-item {
 background-color: #1E96FF;
 color: #FFFFFF;
 text-align: center;
 padding: 15px;
}
```
Se quisermos espaçamento igual entre as colunas, usamos a **column-gap** propriedade.
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(4, auto);
 background-color: #E0F6FF;
 column-gap: 5px;
}
```
Para adicionar espaços entre linhas e colunas, usamos a **gap** abreviação. **gap: 5px 10px** significa que adicionamos espaços **5px** entre linhas e **10px** entre colunas.
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(2, auto);
 gap: 5px 10px;
 background-color: #E0F6FF;
}
```
Para criar espaçamento iguais entre linhas e colunas, definimos **gap** epenas um valor. Por exemplo, **gap: 10px** criar espaçamentos iguais na grade para linhas e colunas.
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(2, auto);
 background-color: #E0F6FF;
 gap: 10px;
}
```