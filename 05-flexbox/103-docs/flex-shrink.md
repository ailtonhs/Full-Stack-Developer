# Flex-shrink

Designs que se adaptam a tamanho menores são ótimos para dispositivos compactos, como celulares. Vamos simular uma tela menor com uma largura de contêiner reduzida
```html
<div class="container">
   <div class="one">1</div>
   <div class="two">2</div>
</div>
```
```css
.one {
 background-color: #FF97A1;
}

.two {
 background-color: #FFC86E;
}

.container {
 border: solid 1px #D37947;
 display: flex;
 width: 250px;

}
```
Os itens flexíveis encolhem quando ão consegue expandir até seu **flex-basis** valor total. Vamos definir **flex-basis** isso 200px para elemento da classe **item**.
```css
.one {
  background-color: #ff97a1;
}

.two {
  background-color: #ffc86e;
}

.item {
  flex-basis: 200px;

}

.container {
  border: solid 1px #d37947;
  display: flex;
  width: 250px;
}
```
Para reduzir o tamanho dos itens flexíveis, usamos a **flex-shrink** propriedade. O valor padrão é **1**.
```css
.one {
  flex-shrink: 1;
  background-color: #FF97A1;
}
```
Se definirmos o valor de flex-shrink como **0**, o item não encolhe de forma alguma. 
```css
.one {
  flex-shrink: 0;
  background-color: #ff97a1;
}
```
Se definirmos ambos os itens como **flex-shrink: 0**, eles transbordarão para fora de seus contêineres.
```css
.one {
  flex-shrink: 0;
  background-color: #ff97a1;
}

.two { 
  flex-shrink: 0;
  background-color: #ffc86e;
}
```
Para que um item flexível encolha mais do que os outros, atribuímos a ele um **flex-shrink** número maior. Fazemos com que o primeiro item encolha mais do que o segundo
```css
.one {
  flex-shrink: 2;
  background-color: #ff97a1;
}

.two { 
  flex-shrink: 1;
  background-color: #ffc86e;
}
```
Podemos definir proporções diferentes para fornecer tamanhos diferentes para cada item flexível. Para tornar cada item menor que o anterior, adicione **1**, **2**, e **3**.
```css
.one {
  flex-shrink: 1;
  background-color: #ff97a1;
}

.two {
  flex-shrink: 2;
  background-color: #ffc86e;
}

.three {
  flex-shrink: 3;
  background-color: #bfdaf9;
}
```