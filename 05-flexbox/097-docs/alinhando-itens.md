# Alinhando itens flexíveis

Para alinhar os itens ao longo do eixo transversal, usamos a **align-items** propriedade.
```html
<div class="container">
   <div class="item"> 1</div>
   <div class="item"> 2</div>
   <div class="item"> 3</div>
   <div class="item"> 4</div>
</div>
```
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
    align-items: stretch;
}

.item {
    border: 2px solid #457081;
}
```
O valor padrão para itens flexíveis **align-items** é **strech**. Essa configuração faz com que os elementos preencham todo o eixo transversal.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
    align-items: stretch;
}
```
Se **flex-direction** definido como **column**, o **stretch** valor fará com que os itens preencham toda a largura do contêiner, pois o eixo transversal é horizontal.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    flex-direction: column;
    align-items: stretch;
}
```
Se **align-items** definido como **flex-start**, os itens assumem o tamanho do seu conteúdo e ficam no início do eixo transversal.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
    align-items: flex-start;
}
```
configurar **align-items** para **flex-end** empurrar os itens para o final do eixo transversal.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
    align-items: flex-end;
}
```
Para centralizar os itens dentro do contêiner, usamos **center**.
```css
.container {
    border: 2px solid #806868;
    display: flex;
    height: 100px;
    align-items: center;
}
```