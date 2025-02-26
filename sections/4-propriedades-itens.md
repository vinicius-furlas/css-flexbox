 4. **Propriedades dos Itens Flexíveis**

      4.1 **`order` – Definição de ordem de exibição**

      A propriedade **order** em css define a ordem de disposição de um item em um contêiner flex ou grid. Os itens em um contêiner são classificados por valor ascendente e, em seguida, pela ordem do código-fonte. Os itens que não recebem um valor explícito recebem o valor padrão de .**`order`** `order``order``0`
    ```
    <div class="container">
    <div class="item" style="order: 3">Item 1</div>
    <div class="item" style="order: 1">Item 2</div>
    <div class="item" style="order: 2">Item 3</div>
    </div>
    ```
    ```
    .container {
     display: flex;
     gap: 10px;
     }

    .item {
     background-color: #f4f4f4;
     padding: 20px;
     border: 1px solid #ccc;
    }
    ```

      4.2 **`flex-grow` – Crescimento proporcional dos itens**

      A propriedade **flex-grow** define o fator de crescimento flexível, que especifica quanto do **espaço livre positivo **do contêiner flexível , se houver, deve ser atribuído ao **tamanho** principal do item flexível .**`flex-grow`** 

      Quando o tamanho principal do flex-container é maior que os tamanhos  principais combinados de seus itens flexíveis, esse espaço livre  positivo pode ser distribuído entre os itens flexíveis, com o  crescimento de cada item sendo seu valor de fator de crescimento como  uma proporção da soma total de todos os fatores de crescimento flexível  dos itens flexíveis.
    ```
    <div class="container">
     <div class="item" style="flex-grow: 1">Item 1</div>
     <div class="item" style="flex-grow: 2">Item 2</div>
     <div class="item" style="flex-grow: 1">Item 3</div>
    </div>
    ```
    ```
    .container {
      display: flex;
      gap: 10px;
    }
    
    .item {
      background-color: #f4f4f4;
      padding: 20px;
      border: 1px solid #ccc;
    }
    ```

      4.3 **`flex-shrink` – Redução proporcional dos itens**

      A propriedade **flex-shrink **define o fator de encolhimento flex de um item flex. Se o tamanho de todos os itens flex for maior que o contêiner flex, os itens flex podem encolher para se ajustar de acordo com seu valor. O espaço livre negativo de cada linha flex é distribuído entre os itens flex da linha que têm um valor maior que .**`flex-shrink`** `flex-shrink``flex-shrink``0`

     ```
     <div class="container">
       <div class="item" style="flex-shrink: 1">Item 1</div>
       <div class="item" style="flex-shrink: 0">Item 2 (Não encolhe)</div>
       <div class="item" style="flex-shrink: 1">Item 3</div>
     </div>
     ```
     ```
     .container {
       display: flex;
       gap: 10px;
       width: 300px; /* Contêiner pequeno para forçar o encolhimento */
     }
     
     .item {
       background-color: #f4f4f4;
       padding: 20px;
       border: 1px solid #ccc;
       width: 150px; /* Largura inicial dos itens */
     }
     ```

      4.4 **`flex-basis` – Tamanho inicial do item**

      A propriedade **flex-basis** define o tamanho principal inicial de um item flexível. Ele define o tamanho da caixa de conteúdo, a menos que seja definido de outra forma com o dimensionamento da caixa.
    ```
    <div class="container">
      <div class="item" style="flex-basis: 100px">Item 1</div>
      <div class="item" style="flex-basis: 200px">Item 2</div>
      <div class="item" style="flex-basis: 50%">Item 3</div>
    </div>
    ```
    ```
    .container {
       display: flex;
       gap: 10px;
     }
     
     .item {
       background-color: #f4f4f4;
       padding: 20px;
       border: 1px solid #ccc;
     }
    ```
      4.5 **`flex` – Atalho para `flex-grow`, `flex-shrink` e `flex-basis`**

      A propriedade flex do CSS, define como um ítem será posicionado para no espaço disponível dentro de seu container.
    ```
    <div class="container">
      <div class="item" style="flex: 1 1 100px">Item 1</div>
      <div class="item" style="flex: 2 1 200px">Item 2</div>
      <div class="item" style="flex: 1 0 50%">Item 3</div>
    </div>
    ```
    ```
    .container {
       display: flex;
       gap: 10px;
     }
     
     .item {
       background-color: #f4f4f4;
       padding: 20px;
       border: 1px solid #ccc;
     }
    ```

      4.6 **`align-self` – Alinhamento individual dos itens**

      A propriedade **CSS**`align-self` alinha itens-flex da linha flex alvo, sobreescrevendo o valor `align-items`. Se alguma dos eixos das margens do dado item está estabelecido como `auto`, então `align-self` é ignorado.
    ```
    <div class="container">
      <div class="item" style="align-self: flex-start">Item 1 (Topo)</div>
      <div class="item" style="align-self: center">Item 2 (Centro)</div>
      <div class="item" style="align-self: flex-end">Item 3 (Base)</div>
    </div>
    ```
    ```
    .container {
       display: flex;
       align-items: stretch; /* Alinhamento padrão */
       height: 200px; /* Altura fixa para visualizar o alinhamento */
       gap: 10px;
     }
     
     .item {
       background-color: #f4f4f4;
       padding: 20px;
       border: 1px solid #ccc;
       width: 100px;
     }
    ```
    
