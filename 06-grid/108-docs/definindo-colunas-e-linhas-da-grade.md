# Definindo colunas e linhas da grade

## Modelo de grade

Usamos essa **grid-template** propriedade para definir as linhas e colunas da grade em uma única linha.
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
 grid-template: 50px 50px / 150px 150px;
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

Ao usar **grid-template**, os valores à esquerda da barra representam as linhas e os da direita, as colunas.
```css
```css
.grid-container {
 display: grid;
 grid-template: 50px 50px / 80px 80px;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Se quisermos, podemos até misturar unidades diferentes. **50px 50px / 1fr 1fr** Basta adicionar um código para que as colunas se ajustem ao tamanho dos contêineres.
```css
```css
.grid-container {
 display: grid;
 grid-template: 50px 50px / 1fr 1fr;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Podemos misturar diferentes unidades relativas para obter resultados diferentes. Por exemplo, definindo as linhas como **60% auto** e as colunas como **1fr 1fr**
```css
```css
.grid-container {
 display: grid;
 grid-template: 60% auto / 1fr 1fr;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Embora estejamos definindo linhas e colunas, ainda podemos ter mais de uma ou de outra.
```css
```css
.grid-container {
 display: grid;
 grid-template: 1fr 1fr 1fr / 60% auto;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}