# flex grow, shrink e basis

Ao trabalhar com layouts responsivos em CSS, o Flexbox é uma das ferramentas mais poderosas e flexíveis para criar interfaces dinâmicas. No entanto, entender como elementos dentro de um contêiner flexível se comportam pode ser desafiador. Propriedades como `flex-grow`, `flex-shrink` e `flex-basis` desempenham papéis essenciais na distribuição do espaço, mas podem ser confusas para muitos desenvolvedores.

Imagine um cenário onde você possui vários itens dentro de um contêiner flexível, e deseja que alguns itens cresçam mais do que outros ou encolham de forma diferente quando o espaço disponível é redimensionado. O Flexbox, por meio das propriedades `flex-grow`, `flex-shrink` e `flex-basis`, oferece uma solução precisa para controlar o comportamento dos elementos. Usando essas propriedades, podemos definir:

- Como os itens crescem quando há espaço extra (`flex-grow`),
- Como encolhem quando há espaço insuficiente (`flex-shrink`),
- E qual será o tamanho base de um item (`flex-basis`).

### 1. flex-grow

A propriedade `flex-grow` define quanto um item pode crescer em relação aos outros quando há espaço extra no contêiner flexível. Se todos os itens tiverem `flex-grow: 1`, eles crescerão igualmente. No entanto, se um item tiver `flex-grow: 2`, ele ocupará o dobro do espaço extra em relação a um item com `flex-grow: 1`.

Exemplo:

```
.item {
  flex-grow: 1;
}
.item-destaque {
  flex-grow: 2;
}
```

Neste caso, o item com `flex-grow: 2` crescerá duas vezes mais do que os outros.

### 2. flex-shrink

A propriedade `flex-shrink` controla como os itens encolhem quando o espaço é reduzido. Um valor maior de `flex-shrink` permite que o item encolha mais do que os outros. Por padrão, a maioria dos itens tem `flex-shrink: 1`, o que significa que encolhem proporcionalmente. Se um item tiver `flex-shrink: 0`, ele não encolherá.

### Exemplo:

```
.item {
  flex-shrink: 1;
}
.item-fixo {
  flex-shrink: 0;
}
```

Aqui, o item com `flex-shrink: 0` permanecerá do mesmo tamanho, mesmo quando o espaço no contêiner for reduzido.

### 3. flex-basis

A propriedade `flex-basis` define o tamanho inicial de um item antes de o espaço restante ser distribuído. Ela pode ser definida como um valor fixo (por exemplo, `200px`) ou como um valor relativo (por exemplo, `auto`).

### Exemplo:

```
.item {
  flex-basis: 100px;
}
```

Neste caso, o item começará com 100px de largura, e depois poderá crescer ou encolher com base nas outras propriedades (`flex-grow` e `flex-shrink`).

Compreender e usar `flex-grow`, `flex-shrink` e `flex-basis` permite criar layouts flexíveis e responsivos com precisão. Ao dominar essas propriedades, você poderá ajustar o comportamento dos seus elementos de forma eficiente, garantindo que seu design funcione bem em qualquer tamanho de tela.

### [Menu-CSS: posicionando elementos com Flexbox CSS](menu.md)