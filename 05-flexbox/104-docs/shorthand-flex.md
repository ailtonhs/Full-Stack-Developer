# Shorthand flex

Vamos aprender como combinar **flex-grow**, **flex-shrink**, e **flex-basis** em uma única propriedade para criar resultados interessantes.

Até agora, aprendemos que, por padrão, os itens flexíveis são definidos como **flex-grow: 0;**, **flex-shrink: 1;** e **flex-basis: auto;**.
```html
 <div class="container">
  <div class="one">1</div>
  <div class="two">2</div>
 </div>
 ```
 ```css
 .one {
  flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto;
  background-color: #ff97a1;
}

.two {
  background-color: #ffc86e;
}

.container {
  border: solid 1px #d37947;
  display: flex;
}
```
Em vez de escrever sempre as 3 propriedades, podemos usar a **flex** forma abreviada.
```css
.one {
 flex: 0 1 auto;
 background-color: #ff97a1;
}
```
Ao usar **flex** abreviações, o primeiro valor é sempre **flex-grow**, seguido por **flex-shrink**, e **flex-basis**. O código **0 1 auto**, os valores padrão.
```css
.one {
 flex: 0 1 auto;
 background-color: #ff97a1;
}
```
Podemos definir **flex** valores diferentes para cada item flexível e obter designs diferentes com base no tamanho da tela.