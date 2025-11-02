# Itens flexíveis em crescimento

## Flex grow

Para controlar como um item flexível cresce ao longo de seu eixo principal, usamos **flex-grow** uma regra dentro do próprio item flexível.
```html
<div class="container">
  <div class="one">1</div>
  <div class="two">2</div>
</div>
```
```css
.one {
    background-color: #ff97a1;
    flex-grow: 0;
}

.two {
    background-color: #ffc86e;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```
O valor padrão para **flex-grow** é **0**, o que significa que o item não se adapta em tamanho e tem apenas a largura do seu conteúdo.
```css
.one {
    background-color: #ff97a1;
    flex-grow: 0;
}
```
Para fazer o item crescer, definimos **flex-grow** para **1**.
```css
.one {
    background-color: #ff97a1;
    flex-grow: 1;
}
```
Aqui, o primeiro item flexível tem um valor padrão **flex-grow: 1;**, enquanto o segundo tem um valor padrão **0**. Aque com o número maior recebe maior espaço.
```css
.one {
    background-color: #ff97a1;
    flex-grow: 1;
}

.two {
    background-color: #ffc86e;
}
```
Itens de maior **flex-grow** valor ocupam mais espaço no recipiente. Um recipiente menor significa que eles ocupam menos espaço.
```css
.container {
    border: 1px solid #d37947;
    display: flex;
    width: 60%;
}

.one {
    background-color: #ff97a1;
    flex-grow: 1;
}

.two {
    background-color: #ffc86e;
}