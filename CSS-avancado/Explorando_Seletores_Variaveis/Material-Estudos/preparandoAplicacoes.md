# Por que declarar `width`e `height`com 100% no `body`? Uma explicação interessante

## Entendendo o`body`

O elemento `<body>` em HTML representa o conteúdo visível de uma página. É o container principal para todo o texto, imagens, links e outros elementos. Ao definir `width` e `height` como 100% neste elemento, estamos basicamente dizendo:

- **Largura**: O conteúdo da página deve ocupar 100% da largura disponível na janela de visualização (área visível do navegador).
- **Altura**: O conteúdo da página deve ocupar 100% da altura disponível na janela de visualização.

## Por que fazemos isso?

1. ### Layout Responsivo:

    - **Adaptação a Diferentes Telas**: Ao definir essas propriedades como 100%, o conteúdo se ajusta automaticamente a diferentes tamanhos de tela, garantindo uma experiência consistente para o usuário, seja em um desktop, tablet ou celular.
    - **Evita Barras de Rolagem Horizontal**: A largura de 100% ajuda a prevenir a indesejada barra de rolagem horizontal, que pode prejudicar a experiência do usuário.

2. ### Base para Outros Elementos:

    - **Elementos Filhos**: O `body`serve como referência para a largura e altura de outros elementos dentro da página. Se você definir um elemento interno com `width`: 50%, ele ocupará 50% da largura total da página.
    - **Posicionamento Absoluto**: Ao definir `width`e `height`no `body`, você estabelece um ponto de referência para elementos posicionados de forma absoluta.

3. ### Normalização do CSS:

    - **Removedor de estilos padrão**: muitos navegadores aplicam estilos padrão aos elementos HTML, incluindo margens e espaçamentos. Ao definir `width`e `height`como 100%, você está "zerando" esses estilos e começando com uma base mais limpa para aplicar seus próprios estilos.

## Considerações Adicionais:

- ### Altura do `body`:

    - **Conteúdo Dinâmico**: Se o conteúdo da sua página variar em altura, defina `height: 100%` que `body`não pode ser suficiente para preencher toda a tela. Nesses casos, você pode usar unidades como vh(altura da janela de visualização) para garantir que o conteúdo sempre ocupe toda a altura disponível.
    - **Elemento Pai**: Lembre-se que a altura de um elemento é relativa à altura de seu elemento pai. Se o elemento pai não tiver uma altura definida, a altura do elemento filho também não terá efeito.

- ### Largura do `body`:

- `width`: 100%: Geralmente é suficiente para garantir que o conteúdo ocupe toda a largura da janela de visualização.
- `box-sizing: border-box`;: Essa propriedade CSS pode ser útil para evitar problemas com o design de largura, especialmente quando você está trabalhando com elementos que possuem bordas ou preenchimento.

### Exemplo:

```
html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### Em Resumo:

Declarar widthe heightcomo 100% não bodyé uma prática comum em CSS, pois fornece uma base sólida para construir layouts responsivos e flexíveis. Ao entender os fundamentos por trás dessa técnica, você estará melhor preparado para criar páginas web modernas e adaptáveis.

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)