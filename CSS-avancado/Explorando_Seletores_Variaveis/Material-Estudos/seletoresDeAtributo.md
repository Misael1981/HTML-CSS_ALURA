# Seletores de Atributo

Como aplicar estilos CSS a elementos com base em seus atributos HTML? Você precisa de uma maneira de selecionar elementos específicos sem adicionar classes extras ou IDs.

Os `seletores de atributo` permitem que você aplique estilos diretamente aos elementos com base nos atributos que eles possuem. Vamos explorar os principais seletores de atributos e ver como cada um pode ser utilizado.

**1 - `[attribute]`**: seleciona todos os elementos que possuem o atributo especificado, independentemente do valor.

Exemplo: Aplicar um estilo a todos os links que possuem o atributo `target`:

```
a[target] {
          color: blue;
}
```

**2 - `[attribute=value]`**: seleciona todos os elementos cujo atributo tenha exatamente o valor especificado.

Exemplo: Aplicar um estilo apenas aos links que abrem em uma nova aba:

```
a[target="_blank"] {
  color: red;
}
```

**3 - `[attribute~=value]`**: seleciona todos os elementos cujo atributo contém uma lista de valores separados por espaços, e um desses valores é exatamente o especificado.

Exemplo: Estilizar elementos que tenham a classe `featured` em uma lista de classes:

```
div[class~="featured"] {
  border: 2px solid gold;
}
```

**4 - `[attribute|=value]`**: seleciona todos os elementos cujo atributo tem um valor que começa com o valor especificado seguido de um hífen (-) ou é exatamente igual ao valor.

Exemplo: Aplicar estilos a elementos com atributos de idioma começando com en (como en ou en-US):

```
[lang|="en"] {
  font-style: italic;
}
```

**5 - `[attribute^=value]`**: seleciona todos os elementos cujo valor do atributo começa com o valor especificado.

Exemplo: Estilizar todos os links que começam com "https":

```
a[href^="https"] {
  font-weight: bold;
}
```

**6 - `[attribute$=value]`**: seleciona todos os elementos cujo valor do atributo termina com o valor especificado.

Exemplo: Aplicar estilos a todas as imagens que têm uma extensão `.png`:

```
img[src$=".png"] {
  border-radius: 8px;
}
```

**7 - `[attribute*=value]`**: seleciona todos os elementos cujo valor do atributo contém a string especificada em qualquer posição.

Exemplo: Estilizar botões com atributos de nome que contenham a palavra "submit":

```
input[name*="submit"] {
  background-color: green;
}
```

Esses seletores te dão mais poderes e liberdade na hora de estilizar elementos específicos.

Se você quiser mergulhar em outros tipos de seletores acesse este [link da documentação](https://www.w3schools.com/cssref/css_selectors.php#gsc.tab=0&gsc.q=user-valid).

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)