# Funções de ajuste de cor no Sass

No Sass, temos acesso a várias funções úteis para manipular cores de forma mais dinâmica e eficiente. Uma dessas funções é a `color.adjust`, que permite modificar propriedades como saturação, matiz e brilho de uma cor existente, sem a necessidade de criar variações manualmente.

### O que temos na partial de buttons é:

```
//código omitido
&:hover {
  background-color: color.adjust(variables.$accent-color, $lightness: -10%);
  border-color: color.adjust(variables.$accent-color, $lightness: -10%);
}
```

Aqui, usamos a função `color.adjust` do módulo `sass:color` para escurecer a cor definida na variável `$accent-color` em 10% ao passar o mouse sobre o botão. Isso é feito ajustando a propriedade de "lightness" (luminosidade) da cor.

## Por que usar @use '`sass:color`'?

A forma recomendada de acessar funcionalidades como as de manipulação de cor é importando módulos com o `@use`. Ao fazer isso, garantimos um código mais modular e organizado. Nesse caso, usamos o módulo `sass:color` para acessar a função `color.adjust`.

Para mais detalhes, você pode consultar a [documentação oficial do Sass sobre o módulo de cores](https://sass-lang.com/documentation/modules/color/).

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)