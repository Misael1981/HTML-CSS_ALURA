# `flex flow`

Muitos layouts exigem que os elementos sejam organizados de diferentes maneiras conforme o espaço da tela muda. Por exemplo, em dispositivos móveis, você pode querer que os itens sejam empilhados verticalmente, enquanto em telas maiores eles são dispostos em uma única linha. Além disso, quando o espaço horizontal é insuficiente, é comum que os itens se movam para uma nova linha. O problema é que controlar manualmente a direção dos itens e o comportamento de quebra de linha pode ser confuso e levar a um código repetitivo.

A propriedade `flex-flow` resolve esse problema ao permitir que você defina simultaneamente a direção e o comportamento de quebra de linha dos itens flexíveis. Ao combinar `flex-direction` e `flex-wrap`, você pode configurar rapidamente como os itens serão organizados no contêiner, com um código mais enxuto e eficiente.

## 1. `flex-direction`

A propriedade `flex-direction` controla a direção na qual os itens são dispostos dentro do contêiner flexível. Os valores mais comuns incluem:

- `row`: Disposição em linha, da esquerda para a direita (padrão).
- `row-reverse`: Disposição em linha, mas da direita para a esquerda.
- `column`: Disposição em coluna, de cima para baixo.
- `column-reverse`: Disposição em coluna, mas de baixo para cima.

### Exemplo:

```
.container {
  display: flex;
  flex-direction: row; /* Ou column, row-reverse, column-reverse */
}
```

## 2. flex-wrap

A propriedade `flex-wrap` controla se os itens devem ou não quebrar a linha quando o espaço no contêiner não for suficiente. Os valores mais comuns são:

- `nowrap`: Os itens não quebram a linha e permanecem em uma única linha ou coluna (padrão).
- `wrap`: Os itens quebram a linha e fluem para uma nova linha ou coluna conforme necessário.
- `wrap-reverse`: Semelhante ao `wrap`, mas a nova linha ou coluna se forma na direção oposta.

### Exemplo:

```
.container {
  display: flex;
  flex-wrap: wrap; /* Ou nowrap, wrap-reverse */
}
```

## 3. flex-flow

A propriedade `flex-flow` é uma abreviação para combinar `flex-direction` e `flex-wrap` em uma única linha de código. O formato é `flex-flow`: `<flex-direction>` `<flex-wrap>`;.

### Exemplo:

```
.container {
  display: flex;
  flex-flow: row wrap;
}
```

Nesse caso, os itens são dispostos em linha (`row`) e quebram para a próxima linha quando necessário (`wrap`).

### Combinações Úteis

Ao utilizar `flex-flow`, é possível criar comportamentos interessantes, como:

- Dispor itens verticalmente e permitir que eles quebrem para novas colunas se necessário:

```
.container {
  flex-flow: column wrap;
}
```
- Dispor os itens em uma única linha da direita para a esquerda, sem permitir que eles quebrem:

```
.container {
  flex-flow: row-reverse nowrap;
}
```
A propriedade `flex-flow` é uma ferramenta poderosa para simplificar o controle sobre a disposição dos itens flexíveis em um contêiner. Ao combinar `flex-direction` e `flex-wrap`, você pode ajustar facilmente a organização dos itens, seja em linhas ou colunas, e controlar o comportamento quando o espaço é insuficiente. Isso resulta em layouts flexíveis e responsivos com menos código e mais clareza.

### [Menu-CSS: posicionando elementos com Flexbox CSS](menu.md)