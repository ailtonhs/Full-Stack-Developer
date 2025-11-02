# Definir o tamanho inicial do item

Para alterar o tamanho dos itens flexíveis ao longo do eixo principal, usamos a **flex-basis** propriedade.
```html
<div class="container">
    <div class="item one">1</div>
    <div class="item two">2</div>
</div>
```
```css
.one {
    flex-basis: auto;
    background-color: #ff97a1;
}

.two {
    background-color: #ffc86e;
}

.container {
    display: flex;
    border: 1px solid #d37947;
}

.item {
    text-align: center;
}
```
Todos os itens flexíveis têm **flex-basis** a largura definida **auto** como padrão. Quando usamos **auto**, os itens têm apenas a largura do seu conteúdo.
```css
.one {
    flex-basis: auto;
    background-color: #ff97a1;
}
```
**flex-basis** é uma propriedade de item flexível. Propriedades de item flexível funcionam apenas dentro de regras de item flexível e não funcionam dentro de regras de contêiner flexível.
```css
.one {
    flex-basis: auto;
    background-color: #ff97a1;
}

.container {
    display: flex;
}
```
Podemos definir o tamanho dos itens com valores em pixels, como **100px**.
```css
.one {
    flex-basis: 100px;
    background-color: #ff97a1;
}
```
Se quisermos definir o tamanho dos itens flexíveis em porcentagem, podemos.
```css
.one {
    flex-basis: 50%;
    background-color: #ff97a1;
}
```
**flex-basis** está vinculado ao eixo principal e se adapta com base nele **flex-direction**. Se tivermos colunas, **flex-basis** define a altura do item.
```css
.one {
    flex-basis: 100px;
    background-color: #ff97a1;
}

.container {
    border: 1px solid #d37947;
    display: flex;
    flex-direction: column;  
}
```
**flex-basis** é o tamanho inicial dos itens flexíveis. Eles ainda adaptam seu tamanho para caber no recipiente. Aqui, o item encolhe para se ajustar.
```css
.one {
    flex-basis: 200px;
    background-color: #ff97a1;
}

.two {
    background-color: #ffc86e;
}

.container {
    border: 1px solid #d37947;
    display: flex;
    width: 150px;
}