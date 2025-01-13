# rgumentos variáveis no Sass

No Sass, é possível criar Mixins que aceitam um número indefinido de argumentos utilizando o conceito de argumentos variáveis. Para isso, usamos três pontos (`...`) após o nome de um parâmetro, o que permite passar múltiplos valores. No exemplo, usamos `$properties...`, mas esse nome é arbitrário – você pode escolher qualquer nome que faça sentido no seu código, como `$args...` ou `$transitions...`.

Quando você passa várias propriedades, como `border-color` e `box-shadow`, o Mixin aplica transições em todas essas propriedades simultaneamente, utilizando a mesma duração e curva de animação (easing). Isso evita a repetição de código, já que o Sass processa todos os parâmetros passados.

A grande vantagem de usar argumentos variáveis é que você pode aplicar a transição em uma única propriedade ou em várias, sem precisar alterar o Mixin. Essa flexibilidade permite reutilizar o mesmo Mixin em diferentes cenários com apenas pequenas variações nos argumentos.

Ao centralizar as transições em um Mixin, você facilita a manutenção do código. Se precisar alterar o tempo de transição ou a curva de animação, por exemplo, basta ajustar a variável variables.$transition-duration em um único lugar, e essa mudança será refletida em todos os lugares onde o Mixin foi aplicado.

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)