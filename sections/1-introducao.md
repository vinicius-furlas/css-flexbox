# 1. Introdução ao CSS Flexbox

🔹 **1.1 O que é Flexbox?**
    Por muito tempo, as únicas  ferramentas disponíveis para criar leiautes em CSS e posicionar  elementos com boa compatibilidade entre browsers eram float e position.  Porém, essas ferramentas possuem algumas limitações muito frustrantes,  especialmente no que diz respeito à responsividade. Algumas tarefas que  consideramos básicas em um leiaute, como centralização vertical de um  elemento-filho com relação a um elemento-pai ou fazer com que  elementos-filhos ocupem a mesma quantidade de espaço, ou colunas terem o mesmo tamanho independente da quantidade de conteúdo interno, eram  impossíveis ou muito difíceis de serem manejadas com floats ou position, ao menos de forma prática e flexível. A ferramenta Flexbox (de Flexible Box) foi criada para tornar essas tarefas mais simples e funcionais: os filhos de um elemento com Flexbox podem se posicionar em qualquer  direção e pode ter dimensões flexíveis para se adaptar.

🔹 **1.2 Quando usar Flexbox?**
    CSS Flexible Box Layout é um módulo do CSS que define um layout  multicoluna otimizado para o design de interfaces de usuário, para isso  busca lidar com o layout dos itens de maneira unidimensional. No modelo  de layout do Flexbox, os filhos de um contêiner flex podem ser dispostos em qualquer direção, e podem "flexibilizar" seus tamanhos, crescendo  para preencher o espaço vazio ou diminuindo para evitar o  transbordamento do elemento pai. O alinhamento horizontal e vertical dos filhos podem ser facilmente manipulados.

🔹 **1.3 Diferença entre Flexbox e outras técnicas de layout (Float, Grid, Inline-Block)**
    **Float:**
O que é floatPropriedade essencialmente "flutua" um elemento à esquerda ou à direita do seu recipiente.
Também remove esse elemento do fluxo normal do documento. Por exemplo, se você floatUma imagem que tem uma legenda, sua legenda acabará enchendo o  espaço ao redor da imagem. A imagem é removida do fluxo normal do  documento
    **Grid:** 
o CSS Grid é projetado especificamente para  layouts bidimensionais, onde você trabalha com linhas e colunas  simultaneamente. Assim, o CSS Grid permite designs de layout mais  complexos.
Um exemplo do uso do grid é:
Layouts de grade : CSS  Grid é ideal para criar layouts de páginas da web intrincados, como um  layout de revista ou blog de página inteira, onde você precisa gerenciar linhas e colunas. Você pode colocar itens em uma estrutura de grade com controle preciso sobre como eles abrangem várias linhas e colunas
    **Inline-Block: **
Primeiro vamos imaginar o seguinte cenário: você tem um parágrafo e que no meio  do seu texto existe uma imagem. Como fazer com que o texto contorne sua  imagem e mantenha um espaçamento entre o texto e a imagem? Se usarmos  display block teremos margens mas criaremos uma nova linha e ocuparemos  100% de largura, mas se usarmos inline teremos o elemento na mesma linha mas sem margem… é aí que o inline-block junta as 2 características.
Com o inline-block você terá o comportamento de um elemento inline, porém  permitindo que altere as margens, altura, largura e padding do seu  elemento assim como um elemento do tipo block. Simples, não é mesmo ?


**Referências:**

https://www.alura.com.br/artigos/css-guia-do-flexbox?srsltid=AfmBOorLJZbvFAo_-Wu3ntl8WnZhZ-XlU1mQK5T7BSqC9NDkWA4VfRVI
https://dev.to/ethanmgustafson/css-float-flexbox-14fg
https://zerotomastery-io.translate.goog/blog/css-grid-vs-flexbox/?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=pt&_x_tr_pto=tc
[https://vitor-franca.medium.com/inline-block-e-inline-block-voc%C3%AA-sabe-a-diferen%C3%A7a-entre-eles-c9f22bfda082](https://vitor-franca.medium.com/inline-block-e-inline-block-você-sabe-a-diferença-entre-eles-c9f22bfda082)
https://www.w3schools.com/cssref/css3_pr_align-items.php
