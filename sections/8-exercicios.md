# 8. Exercícios e Desafios Práticos

**8.1 Criando um layout de cabeçalho e rodapé flexível**
```
<div class="container">
  <header>Header</header>
  <main>Main Content</main>
  <footer>Footer</footer>
</div>
```
```
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header, footer {
  background-color: #333;
  color: white;
  padding: 10px;
  text-align: center;
}

main {
  flex: 1;
  padding: 20px;
}
```

Crie um layout com cabeçalho e rodapé que se ajustem ao tamanho da tela.

**8.2 Criando uma galeria de imagens responsiva**
```
<div class="galeria">
  <img src="image1.jpg" alt="Image 1">
  <img src="image2.jpg" alt="Image 2">
  <img src="image3.jpg" alt="Image 3">
</div>
```

```
.galeria {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.galeria img {
  flex: 1 1 calc(33.333% - 10px);
  max-width: 100%;
  height: auto;
}
```

Crie uma galeria de imagens que se ajuste ao tamanho da tela.

**8.3 Criando um formulário estilizado usando Flexbox**

Crie um formulário com campos alinhados e espaçados.

**8.4 Criando um card de perfil utilizando Flexbox**

Crie um card de perfil com foto, nome e descrição.

**8.5 Desafio: Criando uma página de login usando apenas Flexbox**

Crie uma página de login com campos de entrada e botão de envio.

**8.6 Desafio avançado: Reproduzir um layout de site real com Flexbox**

Escolha um site real e tente reproduzir seu layout usando apenas Flexbox. Isso ajudará a consolidar todos os conceitos aprendidos.
