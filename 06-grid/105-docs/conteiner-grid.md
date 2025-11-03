# Criando uma grade CSS

## O Contêiner de grade

O CSS Grid é um sistema de layout que nos permite adicionar itens tanto horizontal quanto verticalmente em uma página da web.

Para usar o CSS Grid, primeiro precisamos criar um elemento pai que atuará como um contêiner.
```html
<div class="grid-container">
   <div>1</div>
   <div>2</div>
   <div>3</div>
   <div>4</div>
</div>
```
Em seguida, adicionamos a **grid-item** classe aos elementos dentro do contêiner.
```html
<div class="grid-container">
   <div class="grid-item">1</div>
   <div class="grid-item">2</div>
   <div class="grid-item">3</div>
   <div class="grid-item">4</div>
</div>
```
Para aplicar o CSS Grid ao contêiner, precisamos começar com a **display** propriedade. Em seguida, definimos a **display** propriedade com o valor **grid**.
```css
.grid-container {
    display: grid;
    background-color: #e0f6ff;
    border: 1px dashed #1e96ff;
}

.grid-item {
    background-color: #1e96ff;
    color: #ffffff;
    text-align: center;
    margin: 2px;
}
```
Em seguida, vamos organizar os itens da grade em colunas. Para isso, usaremos a **grid-template-columns** propriedade. Podemos então definir o tamanho de cada coluna separadamente, dependendo do nosso projeto.
```css
.grid-container {
    display: grid;
    grid-template-columns: 50px 50px 120px;
    background-color: #e0f6ff;
    border: 1px dashed #1e96ff;
}

.grid-item {
    background-color: #1e96ff;
    color: #ffffff;
    text-align: center;
    margin: 2px;
}
```