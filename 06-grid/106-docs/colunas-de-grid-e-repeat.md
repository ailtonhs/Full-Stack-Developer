# Criando colunas de grade

## Colunas de grade e repetição

Vamos aprender como definir o tamanho e o número de colunas da grade.

Para definir colunas de grade com tamanho fixo, usamos pixels.
```html
  <div class="grid-container">
   <div class="grid-item">1</div>
   <div class="grid-item">2</div>
   <div class="grid-item">3</div>
  </div>
  ```
```css
.grid-container {
 display: grid;
 grid-template-columns: 100px 50px 100px;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}

.grid-item {
 background-color: #1E96FF;
 color: #FFFFFF;
 text-align: center;
 margin: 2px;
 padding: 10px;
}
```
Os itens da grade são exibidos com base no número de colunas. Se houver mais itens do que colunas, os itens extras serão movidos para a próxima linha.
```html
  <div class="grid-container">
   <div class="grid-item">1</div>
   <div class="grid-item">2</div>
   <div class="grid-item">3</div>
   <div class="grid-item">4</div>
  </div>
  ```
  ```css
  .grid-container {
 display: grid;
 grid-template-columns: 50px 50px 50px;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Vamos analizar os valores que se adaptam ao tamanho da tela. Definir uma coluna como **auto** fará com que os itens da grade ocupe o máximo de espaço possível.
```css
.grid-container {
 display: grid;
 grid-template-columns: 50px auto auto;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
A grid possui uma unidade de medida especial chamada **fr**, abreviação de **unidade fracionária**. **fr** ela distribui o espaço disponível do contêiner em frações.
```css
.grid-container {
 display: grid;
 grid-template-columns: 1fr 2fr 1fr;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Se combinamos **fr** com outra unidades como **px**, o espaço restante após adicionar o **px** item é o que será distribuído em frações.
```css
.grid-container {
 display: grid;
 grid-template-columns: 50px 1fr 1fr;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
O Grid possui um atalho para definir colunas rapidamente, e esse atalho é a **reapet()** função. Por exemplo, **repeat(3, 1fr)** significa 3 colunas de **1fr** cada tipo.
```css
.grid-container {
 display: grid;
 grid-template-columns: repeat(3, 1fr);
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```

