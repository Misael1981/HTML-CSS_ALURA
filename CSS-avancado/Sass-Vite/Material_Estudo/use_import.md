# @use vs @import no Sass

No Sass, a transição do `@import` para o `@use` representa uma melhoria na modularidade e na organização do código. No projeto Serenatto, importamos as partials utilizando o `@use`. Mas que tal compreender as diferenças entre eles?

## `@import`

`@import` é a abordagem clássica para incluir arquivos Sass. Embora funcional, pode levar a problemas como:

- **Duplicação de estilos**: o mesmo arquivo pode ser importado várias vezes, resultando em CSS redundante.
- **Conflitos de nomes**: como todos os estilos são incorporados globalmente, variáveis e mixins podem colidir, causando comportamentos inesperados.

## `@use`

Em contraste, `@use` introduz uma forma mais segura e eficiente de gerenciar dependências:

- **Namespace**: os arquivos são encapsulados dentro de um namespace, evitando conflitos de nomes. Você acessa variáveis e mixins com o formato namespace.variable ou namespace.mixin().
- **Carregamento único**: cada arquivo é carregado apenas uma vez, reduzindo a duplicação no CSS final e melhorando o desempenho.
- **Controle de acesso**: é possível definir variáveis e mixins como públicas ou privadas, o que permite um gerenciamento mais refinado do que é exposto a outros arquivos.

**Então**, embora o `@import` ainda esteja disponível, o `@use` é a abordagem recomendada para criar estilos mais limpos, organizados e sustentáveis.

Para mais detalhes, consulte a documentação oficial do Sass sobre [@import](https://sass-lang.com/documentation/at-rules/import/) e [@use](https://sass-lang.com/documentation/at-rules/use/).

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)