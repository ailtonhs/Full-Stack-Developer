# Justificando linhas e colunas

## Justificando colunas

**justify-content** funciona com **flex-direction: column;**, mas só podemos ver funcionando se o contêiner for mais alto que todos os itens.

**flex-direction: column;** significa que o eixo principal do contêiner é vertical, **justify-content: center** justificando assim os itens verticalmente desta vez.
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
    border: 2px solid lightgray;
    height: 200px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.item {
    border: 3px solid #457081;
}
```
Se quiser que os itens fiquem bem espaçados verticalmente dentro de um contêiner, usamos esse **space-around** valor.
```css
.container {
    border: 2px solid lightgray;
    height: 200px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}
```
Para manter espaço entre os itens e posicionar o primeiro e o último item próximo às laterais do recipiente, utilizamos **space-between**.
```css
.container {
    border: 2px solid lightgray;
    height: 200px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
```
