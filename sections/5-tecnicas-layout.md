# 5. Técnicas e Padrões de Layout com Flexbox

## 5.1 Criando um layout de coluna responsivo:

Um layout de coluna responsivo é ideal para organizar conteúdo verticalmente, como em páginas de blog ou painéis de administração. Com Flexbox, você pode criar colunas que se ajustam automaticamente ao tamanho da tela.

```
.container {
  display: flex;
  flex-direction: column;
  gap: 10px; /* Espaçamento entre os itens */
}
```

 
​	**5.2 Criando um layout de linha responsivo**

Um layout de linha é perfeito para menus de navegação, galerias de imagens ou qualquer conteúdo que precise ser organizado horizontalmente. Com Flexbox, você pode garantir que os itens se ajustem ao espaço disponível.

```
.container {
  display: flex;
  flex-direction: row;
  gap: 10px; /* Espaçamento entre os itens */
}

.item {
  background-color: #f4f4f4;
  padding: 20px;
  border: 1px solid #ccc;
  flex: 1; /* Distribui o espaço igualmente */
}
```

​	5.3 Centralizando elementos com Flexbox

Centralizar elementos vertical e horizontalmente é uma das tarefas mais comuns no desenvolvimento web. Com Flexbox, isso se torna extremamente simples.

```
.container {
  display: flex;
  justify-content: center; /* Centraliza horizontalmente */
  align-items: center; /* Centraliza verticalmente */
  height: 100vh; /* Altura total da tela */
}
```

​	5.4 Criando um menu de navegação flexível

Um menu de navegação flexível é essencial para sites responsivos. Com Flexbox, você pode criar menus que se ajustam ao tamanho da tela e reorganizam os itens automaticamente.

```
.menu {
  display: flex;
  justify-content: space-around; /* Distribui os itens igualmente */
  background-color: #333;
  padding: 10px;
}
```
​	5.5 Criando um grid de cards com Flexbox

Um grid de cards é perfeito para exibir produtos, posts de blog ou qualquer conteúdo em formato de cartão. Com Flexbox, você pode criar um layout responsivo e organizado.
```
.grid {
  display: flex;
  flex-wrap: wrap;
  gap: 10px; /* Espaçamento entre os cards */
}

.card {
  background-color: #f4f4f4;
  padding: 20px;
  border: 1px solid #ccc;
  flex: 1 1 calc(33.333% - 20px); /* 3 colunas com espaçamento */
  box-sizing: border-box;
}
```

**Referências:**

https://css-tricks.com/snippets/css/a-guide-to-flexbox/
