# Combinadores CSS

Você está desenvolvendo uma página web e precisa estilizar um menu de navegação. As opções do menu são elementos `<li>` dentro de uma `<ul>`. No entanto, você quer que apenas os links que são filhos diretos dos

- Sejam estilizados de uma forma especial, mas percebe que não dá para usar uma simples classe ou ID para isso.
Você percebe que aplicar um estilo diretamente na `<ul>` afeta todos os links, inclusive aqueles que estão dentro de outras listas (`<ul>`) em outras partes do código. Mas você só quer que os links de primeiro nível (ou seja, os filhos diretos) sejam afetados.

Aqui é onde entram os **combinadores CSS**. Eles permitem que você selecione elementos baseando-se na relação entre eles. Por exemplo, para resolver seu problema, você pode usar o combinador de filho direto (`>`):

```
ul > li > a {
  color: red;
}
```

Com esse código, apenas os links (`<a>`) que são filhos diretos de um `<li>` que, por sua vez, é filho direto do `<ul>`, serão coloridos de vermelho.

Os combinadores CSS permitem que você selecione elementos com base em suas relações no DOM. Os principais combinadores são:

- **Descendente ( )**: seleciona todos os elementos que são descendentes de um outro elemento, por exemplo, `div p` seleciona todos os `<p>` dentro de `<div>`.
- **Filho Direto (`>`)**: seleciona apenas os filhos diretos de um elemento, como `ul > li`.
- **Adjacente (`+`)**: seleciona o elemento que vem imediatamente após um outro elemento, como `h1 + p`.
- **Irmão Geral (`~`)**: seleciona todos os elementos irmãos que seguem um elemento específico, como `h1 ~ p`. Você pode usar um ou mais combinadores para estilizar elementos de forma mais específica no seu código.

- ### [artigo sobre seletores avançados em CSS escrito pelo Vinicius Neves](https://www.alura.com.br/artigos/css-seletores-avancados-aplicacoes-web)


### [Menu - Explorando seletores e utilizando variáveis](../menu.md)