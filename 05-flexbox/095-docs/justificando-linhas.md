# Justificando linhas e colunas

## Justificando linhas

Para posicionar os itens flexíveis no centro do eixo principal do contêiner, definimos **justify-content** como center.
```html
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
</div>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: center;
}

.item {
    border: 3px solid #457081;
}
```
Se quisermos que os itens fiquem bem espaçados dentro de um contêiner, usamos esse **space-around** valor.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: space-around;
}
```
Para manter espaço entre os itens e posicionar o primeiro e o último item próximo às laterais do recipiente, utilizamos o **space-between** valor.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    justify-content: space-between;
}