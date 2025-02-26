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


## 6.4 Criando layouts flexíveis sem necessidade de Media Queries


## 6.5 Testando responsividade com ferramentas do navegador


