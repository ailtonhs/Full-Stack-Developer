# Criando linhas de grade

O CSS Grid nos dá controle sobre as linhas, permitindo ajustar seu tamanho e localização dentro da grade.

Vamas analisar mais detalhadamente como dimensionar as linhas. Usamos a **grid-template-rows** propriedade para definir as linhas da grade.
```html
  <div class="grid-container">
   <div class="grid-item">1</div>
   <div class="grid-item">2</div>
   <div class="grid-item">3</div>
  </div>
  ```
```css
.grid-container {
 display: grid;
 grid-template-rows: 50px 80px 100px;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}

.grid-item {
 background-color: #1E96FF;
 color: #FFFFFF;
 text-align: center;
 padding-top: 10px;
 margin: 2px;
}
```
Para organizar os itens da grade em linhas de tamanho fixo, usamos unidades de pixel. Se houver menos itens na grade do que linhas, teremos linhas vazias.
```css
.grid-container {
 display: grid;
 grid-template-rows: 50px 50px 50px;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Também podemos usar valores percentuais para as linhas, mas isso só funciona se o contêiner tiver um tamanho definido, como **300px** nesse caso.
```css
.grid-container {
 display: grid;
 grid-template-rows: 40% 60%;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Podemos combinar **px** unidades e **fr** unidades juntas, se necessário.
```css
.grid-container {
 display: grid;
 grid-template-rows: 100px 1fr 2fr;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Definir o tamanho da linha **auto** fará com que ela ocupe todo o espaço disponível.
```css
.grid-container {
 display: grid;
 grid-template-rows: auto 30px auto;
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```
Assim como antes, podemos usar a **repeat()** função para escrever menos código **repeat(3, 40px)**.
```css
.grid-container {
 display: grid;
 grid-template-rows: repeat(3, 40px);
 background-color: #E0F6FF;
 border: 1px dashed #1E96FF;
}
```