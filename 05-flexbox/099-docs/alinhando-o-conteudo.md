# Alinhando o conteúdo

Para controlar o espaço ao redor das linhas de itens que se repetem, usamos a **align-content** propriedade. Isso afeta as linhas ao longo do eixo transversal.
```html
 <div class="container">
   <div class="item">1</div>
   <div class="item">2</div>
   <div class="item">3</div>
   <div class="item">4</div>
   <div class="item">5</div>
   <div class="item">6</div>
   <div class="item">7</div>
   <div class="item">8</div>
   <div class="item">9</div>
  </div>
  ```
  ```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: flex-start;
  }

.item {
   background-color: #FF97A1;
   width: 20%;
   margin: 1px;
}
```
O valor padrão para **align-content** é **stretch**, o que faz com que as linhas de itens flexíveis se estiquem no eixo transversal.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: stretch;
  }
  ```
Para que as linhas quebradas comecem de cima para baixo, definimos **align-content** como **flex-start**.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: flex-start;
  }
  ```
**align-content: flex-end;** empurra todas as linhas para o final do contêiner.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: flex-end;
  }
  ```
**align-content: center;** agrupa todas as linhas no centro do eixo transversal.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: center;
  }
  ```
Para adicionar espaço entre as linhas ao longo do eixo transversal, podemos usar o **space-around** valor.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: space-around;
  }
  ```
Para adicionar espaço entre as linhas, mas remover o espaço próximo às bordas, usamos **space-between**.
```css
.container {
    border: solid 2px #806868;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    align-content: space-between;
  }