# Explorando mais sobre o @content

No Sass, o `@content` oferece flexibilidade e poder na criação de mixins e regras dinâmicas de CSS. Vamos explorar com mais detalhes como o `@content` funciona?

O `@content` é uma funcionalidade especial em Sass que permite passar blocos de código CSS diretamente para dentro de um mixin. Ele age como um "placeholder" para o conteúdo que será injetado quando o mixin for chamado. Isso é útil quando você quer que um mixin aplique diferentes estilos ou media queries sem precisar repetir o código.

Ao incluir um mixin com `@content`, você pode passar blocos de CSS personalizados, que serão inseridos onde o `@content` estiver no mixin. Veja o exemplo:

```
@mixin media-query($breakpoint) {
  @media (max-width: $breakpoint) {
    @content;
  }
}

.container {
  background-color: blue;

  @include media-query(768px) {
    background-color: red;
  }
}
```

Aqui, o `@content` injetará o `background-color: red` dentro da media query para telas de até 768px de largura, o que facilita a aplicação de diferentes regras para breakpoints específicos.

### E quais vantagens do @content podemos destacar?

- **Modularidade**: ao invés de escrever media queries em múltiplos lugares, o `@content` permite centralizar a lógica, melhorando a manutenção.
- **Reutilização**: você pode usar o mesmo mixin para diferentes seletores, obedecendo à boa prática “DRY” (Don't Repeat Yourself - Não se repita!).

Se você quiser se aprofundar nessa funcionalidade e explorar mais exemplos de uso, consulte a [documentação oficial do Sass sobre content blocks](https://sass-lang.com/documentation/at-rules/mixin/#content-blocks).

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)