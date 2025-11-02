# itens flexíveis em crescimento

## Flex grow avançado

Podemos definir **flex-grow** o tamanho de todos os itens dentro de um contêiner flexível. Se definirmos o **1** tamanho de todos eles para crescer igualmente e preencherão o contêiner.
```html
<div class="container">
  <div class="one">1</div>
  <div class="two">2</div>
  <div class="three">3</div>
</div>
```
```css
.one {
    flex-grow: 1;
    background-color: #ff97a1;
}

.two {
    flex-grow: 1;
    background-color: #ffc86e;
}

.three {
    flex-grow: 1;
    background-color: #bfdaf9;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```
Os valores que definirmos **flex-grow** são proporções. Se definirmos **flex-grow** o mesmo número para todos os itens, eles permanecerão com o mesmo tamanho.
```css
.one {
    flex-grow: 100;
    background-color: #ff97a1;
}

.two {
    flex-grow: 100;
    background-color: #ffc86e;
}

.three {
    flex-grow: 100;
    background-color: #bfdaf9;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```
Se quisermos aumentar o tamanho do primeiro item flexível, atribuímos a ele um **flex-grow** valor maior do que aos outros dois itens.
```css
.one {
    flex-grow: 2;
    background-color: #ff97a1;
}

.two {
    flex-grow: 1;
    background-color: #ffc86e;
}

.three {
    flex-grow: 1;
    background-color: #bfdaf9;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```
Quanto maior o número, maior a proporção do espaço vazio do contêiner que destinamos a um item flexível.
```css
.one {
    flex-grow: 20;
    background-color: #ff97a1;
}

.two {
    flex-grow: 1;
    background-color: #ffc86e;
}

.three {
    flex-grow: 1;
    background-color: #bfdaf9;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```
Podemos definir proporções diferentes para fornecer tamanhos diferentes para cada item flexível.
```css
.one {
    flex-grow: 1;
    background-color: #ff97a1;
}

.two {
    flex-grow: 2;
    background-color: #ffc86e;
}

.three {
    flex-grow: 3;
    background-color: #bfdaf9;
}

.container {
    border: 1px solid #d37947;
    display: flex;
}
```