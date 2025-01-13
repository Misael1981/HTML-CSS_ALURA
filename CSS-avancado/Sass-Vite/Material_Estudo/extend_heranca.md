#  @extend e herança no Sass

No desenvolvimento de projetos, a repetição de estilos pode se tornar um grande desafio à medida que o código cresce. O Sass oferece soluções para esse problema por meio do uso de `%placeholders` e da diretiva `@extend`. Esses recursos promovem a herança de estilos, permitindo que você crie uma base de estilos reutilizáveis.

`%placeholders` são uma forma de definir estilos que podem ser aplicados a diferentes seletores sem gerar CSS adicional. Eles atuam como modelos de estilo, permitindo que você mantenha seu código organizado e conciso. Ao utilizá-los, você consegue agrupar propriedades comuns e evitar a duplicação, resultando em um arquivo CSS menor e mais fácil de manter.

Já a diretiva `@extend` é o mecanismo que permite aplicar esses `%placeholders` a diferentes classes. Quando um seletor utiliza `@extend`, ele herda todas as propriedades do `%placeholder` correspondente. Isso não apenas reduz a quantidade de código, mas também assegura que qualquer modificação feita no `%placeholder` será automaticamente refletida em todos os seletores que o utilizam. Assim, você mantém a consistência visual em todo o projeto.

Essa abordagem de herança é fundamental para a manutenção do código. Em vez de alterar várias regras CSS em diferentes locais, uma simples atualização no `%placeholder` pode propagar as mudanças automaticamente, facilitando a implementação de novas regras de estilo.

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)