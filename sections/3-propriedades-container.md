# 3. Propriedades do Contêiner Flexível

   3.1 **`flex-direction` – Direção dos elementos**

   A propriedade flex-direction **permite alterar a direção na qual os elementos flex serão exibidos ao longo do eixo principal**. Definindo a propriedade flex-direction como row-reverse (linha reversa) ainda teremos os elementos dispostos em uma linha, entretanto, as  linhas inicial e final serão trocadas.
   ```
   <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
   </div>
   ```
   ```
   .container {
     display: flex;
     flex-direction: row; 
     gap: 10px;
   }
   
   .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
   }
   ```
   3.2 **`flex-wrap` – Quebra de linha dos itens**

   Define se os itens devem quebrar ou não a linha. **Por padrão eles não quebram linha**, isso faz com que os flex itens sejam compactados além do limite do conteúdo.
   ```
      <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
     <div class="item">Item 4</div>
     <div class="item">Item 5</div>
   </div>
   ```
   3.3 **`flex-flow` – Atalho para `flex-direction` e `flex-wrap`**

   **O flex-flow é um atalho para as propriedades flex-direction e flex-wrap**. Você não verá muito o seu uso, pois geralmente quando mudamos o  flex-direction para column, mantemos o padrão do flex-wrap que é nowrap. E quando mudamos o flex-wrap para wrap, mantemos o padrão do  flex-direction que é row. Já o [CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS) **`flex-wrap`** define se os itens flexíveis são forçados a ficarem na mesma linha ou  se podem ser quebradas em varias linhas. Se o argumento for valido, ele  define a direção em que as linhas são empilhadas.
   ```
   <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
     <div class="item">Item 4</div>
     <div class="item">Item 5</div>
   </div>
   ```
   ```
   .container {
     display: flex;
     flex-flow: row wrap;
     gap: 10px;
     width: 300px; 
   }
   
   .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
     width: 100px; 
   }
   ```

   3.4 **`justify-content` – Alinhamento horizontal dos itens**

   Justify-content controla o alinhamento de todos os itens no eixo principal. A propriedade justify-content controla o alinhamento das colunas da grade. Ela é definida no contêiner da grade . Ela não se aplica ou controla o alinhamento dos itens da grade.
   ```
   <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
   </div>
   ```
   ```
   .container {
     display: flex;
     justify-content: center; 
     gap: 10px;
   }
   
   .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
   }
   ```

   3.5 **`align-items` – Alinhamento vertical dos itens**

   A propriedade align-items especifica o alinhamento padrão para itens dentro de um flexbox ou contêiner de grade.Em um contêiner flexbox, os itens do flexbox são alinhados no eixo cruzado, que é vertical por padrão (oposto à direção flexível).Em um contêiner de grade, os itens da grade são alinhados na direção do bloco. Para páginas em inglês, a direção do bloco é para baixo e a direção embutida é da esquerda para a direita.Para que esta propriedade tenha algum efeito de alinhamento, os itens precisam de espaço disponível ao seu redor na direção apropriada.

   Para que esta propriedade tenha algum efeito de alinhamento, os itens precisam de espaço disponível ao seu redor na direção apropriada.
   ```
   <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
   </div>
   ```
   ```
   .container {
     display: flex;
     align-items: center; 
     height: 200px;
     gap: 10px;
   }
   
   .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
     width: 100px;
   }
   ```

   3.6 **`align-content` – Alinhamento em múltiplas linhas**

   A propriedade CSS align-content define a distribuição de espaço entre e ao redor dos itens de conteúdo ao longo do eixo cruzado de um flexbox ou do eixo de bloco de um elemento em nível de bloco ou grade.
   ```
   <div class="container">
     <div class="item">Item 1</div>
     <div class="item">Item 2</div>
     <div class="item">Item 3</div>
     <div class="item">Item 4</div>
     <div class="item">Item 5</div>
   </div>
   ```
   ```
   .container {
     display: flex;
     flex-wrap: wrap;
     align-content: space-between; 
     height: 200px;
     gap: 10px;
   }
   
   .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
     width: 100px;
   }
   ```

Referências:

https://www.w3schools.com/cssref/css3_pr_flex-direction.php
https://www.w3schools.com/cssref/css3_pr_flex-flow.php
https://www.w3schools.com/cssref/css3_pr_align-items.php
