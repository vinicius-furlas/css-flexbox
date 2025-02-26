# 6. Flexbox e Responsividade

## 6.1 Uso de `flex-wrap` para adaptação em telas menores
A propriedade flex-wrap permite que os itens quebrem para a próxima linha quando o espaço é insuficiente, garantindo que o layout se ajuste a telas menores.
```
.container {
  display: flex;
  flex-wrap: wrap;
}
```

## 6.2 Combinando Flexbox com Media Queries
Media Queries permitem ajustar o layout para diferentes tamanhos de tela. Combinado com Flexbox, você pode criar designs totalmente responsivos.

```
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

## 6.3 Melhorando a usabilidade em dispositivos móveis
A usabilidade em dispositivos móveis é essencial para garantir que seu site seja acessível e funcional em telas menores. Com Flexbox, você pode criar layouts que se adaptam automaticamente ao tamanho da tela, melhorando a experiência do usuário. Como por exemplo:
```
@media (max-width: 600px) {
  .container {
    flex-direction: column;
    gap: 10px;
  }
}
```

## 6.4 Criando layouts flexíveis sem necessidade de Media Queries
Com Flexbox, você pode criar layouts que se ajustam automaticamente ao espaço disponível, reduzindo a necessidade de Media Queries. Isso é possível usando propriedades como flex-grow, flex-shrink e flex-basis.
```
.item {
  background-color: #f4f4f4;
  padding: 20px;
  border: 1px solid #ccc;
  flex: 1 1 auto; /* Itens crescem e encolhem conforme o espaço */
}
```

## 6.5 Testando responsividade com ferramentas do navegador
As ferramentas de desenvolvedor (DevTools) dos navegadores são essenciais para testar e ajustar a responsividade do seu layout. Elas permitem simular diferentes tamanhos de tela, inspecionar elementos e depurar problemas.



