# Flex-wrap

Para impedir que os elementos ultrapassem os limites do contêiner, usamos a **flex-wrap** propriedade.
```html
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
    <div class="item">5</div>
    <div class="item">6</div>
</div>
```
```css
.container {
    border: 3px solid #806868;
    width: 200px;
    display: flex;
    flex-wrap: nowrap;
}

.item {
    border: 3px solid #457081;
    margin: 20px;
}
```
O valor padrão para **flex-wrap** é **nowrap**. Isso significa que, se os objetos não puderem mais diminuir de tamanho dentro do contêiner, eles transbordarão para fora dele.
```css
.container {
    border: 3px solid #806868;
    width: 200px;
    display: flex;
    flex-wrap: nowrap;
}
```
Costumávamos **flex-wrap: wrap;** fazer com que os itens começassem em uma nova linha quando não cabiam mais.
```css
.container {
    border: 3px solid #806868;
    width: 200px;
    display: flex;
    flex-wrap: wrap;
}
```
Se quisermos que os itens que não cabem vão para o topo do recipiente em vez do fundo, usamos **wrap-reverse**.
```css
.container {
    border: 3px solid #806868;
    width: 200px;
    display: flex;
    flex-wrap: wrap-reverse;
}
```
Assim como antes, **flex-wrap** funciona tanto para colunas quanto para linhas. 
```css
.container {
    border: 3px solid #806868;
    width: 200px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap-reverse;
}
```
