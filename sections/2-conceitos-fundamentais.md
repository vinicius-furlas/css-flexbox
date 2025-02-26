2. **Conceitos Fundamentais**

​	2.1 **O Modelo de Caixa Flexível**

No Flexbox, cada elemento é envolto em uma "caixa flexível" que permite o ajuste dinâmico de tamanho e posicionamento, ou seja, visa organizar os elementos de uma página HTML dentro de seus containers de forma dinâmica

​	2.2 **Elemento Pai (Flex Container) vs. Elementos Filhos (Flex Items)**

O Flex Container **é um componente de layout que ajuda você a projetar e criar layouts de seção na sua página da web**. Você pode usar contêineres flexíveis para agrupar componentes como botões, texto, imagens e outros contêineres, ou seja, um elemento pai. **Os Flex Itens são os filhos diretos do Flex Container**, lembrado que uma tag se torna um flex container a partir do momento que você definir display: flex. É possível que um Flex Item seja também um  Flex Container, basta definir display: flex nele. Assim os filhos desse  item também serão flex itens, ou seja, Elementos Filhos.

​	2.3 **Propriedade `display: flex` e seus efeitos**

O **display**: **flex** funciona de uma maneira diferente dos outros **displays**. Quando colocamos essa **propriedade** em um elemento, esse elemento se torna um **flex** container, a partir daí podemos manipular todos os elementos filhos desse **flex** container com **propriedades** novas.
