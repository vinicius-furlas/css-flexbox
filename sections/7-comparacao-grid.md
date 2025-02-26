# 7. Comparação entre Flexbox e CSS Grid
**7.1 Diferenças entre Flexbox e Grid Layout**

**Flexbox:**

Ideal para layouts unidimensionais (uma linha ou uma coluna). Focado em distribuir espaço e alinhar itens em um único eixo.

**CSS Grid:**

Ideal para layouts bidimensionais (linhas e colunas). Permite criar layouts complexos com controle total sobre linhas e colunas.

Exemplo:
```
/* Flexbox */
.flex-container {
  display: flex;
  justify-content: space-between;
}

/* CSS Grid */
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
```

**7.2 Quando usar Flexbox e quando usar Grid**

**Use Flexbox:**

Para alinhar itens em uma única direção (linha ou coluna).

Para distribuir espaço entre itens de forma dinâmica.

Para criar componentes como menus, barras de navegação ou cards.

**Use CSS Grid:**

Para layouts complexos com linhas e colunas.

Para criar grids de imagens, galerias ou layouts de página inteira.

**7.3 Combinação de Flexbox e Grid para layouts avançados**

Você pode combinar Flexbox e Grid para criar layouts ainda mais poderosos. Por exemplo, use Grid para o layout geral da página e Flexbox para alinhar itens dentro de cada célula do grid.
```
.grid-container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  gap: 10px;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }

.main {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

**7.4 Conversão de layouts Flexbox para Grid e vice-versa**

Às vezes, você pode precisar converter um layout de Flexbox para Grid ou vice-versa. Aqui estão algumas dicas:

**Flexbox para Grid:** Se o layout é unidimensional, mantenha Flexbox. Se for bidimensional, considere Grid.

**Grid para Flexbox:** Se o layout é simples e unidimensional, Flexbox pode ser mais fácil de implementar.


Referências :

https://css-tricks.com/quick-whats-the-difference-between-flexbox-and-grid/
https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_grid_layout/Relationship_of_grid_layout_with_other_layout_methods
https://www.smashingmagazine.com/2018/04/best-practices-grid-layout/

