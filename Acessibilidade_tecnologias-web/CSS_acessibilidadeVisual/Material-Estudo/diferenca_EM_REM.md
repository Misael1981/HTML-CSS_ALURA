# Entendendo a diferença entre EM e REM

As unidades de medida definem tamanhos e espaçamentos entre elementos na tela, certo?

Portanto, elas são essenciais na acessibilidade e design: conforme expliquei, não é recomendado utilizar pixels (px) em tamanhos de fonte.

Em CSS, temos mais duas unidades de medida: “REM” e “EM”. Ambas se relacionam com o dimensionamento de elementos na página, porém apresentam diferenças significativas.

Vamos ver mais.

## Como cada uma funciona?

### "`em`":

A unidade "em", em CSS, é uma medida relativa ao tamanho da fonte do elemento pai.

Isso significa que um valor de "1em" corresponde ao tamanho da fonte do elemento pai. Se você definir um elemento com tamanho de fonte de "2em", ele será o dobro do tamanho da fonte do elemento pai. No entanto, essa relação é cumulativa: se você aninhar elementos com tamanhos de fonte em "em", o tamanho da fonte será multiplicado pelo tamanho do elemento pai imediatamente acima na hierarquia.

### Definindo tamanho de fontes com “em”:

```
//CSS

body {
  font-size: 16px; /* Tamanho da fonte padrão na maioria dos navegadores */
}

p {
  font-size: 2em; /* Tamanho da fonte do parágrafo será 2 vezes a fonte padrão do navegador, que nesse caso é 32px */
}
```

### Definindo espaçamentos com “em”:

```
//CSS
article {
  font-size: 18px; /* Tamanho da fonte do artigo */
  line-height: 1.5em; /* Espaçamento de linha será 1.5 vezes a fonte do artigo */
}
```

### "`REM`":

A unidade "REM" em CSS é utilizada para definir medidas; é relativa ao tamanho da fonte do elemento raiz. Isso proporciona uma abordagem global e previsível, permitindo que as alterações no tamanho da fonte do elemento raiz afetem uniformemente todos os elementos na página, simplificando a manutenção e garantindo consistência no design.

### Definindo tamanho de fontes com “REM”:

```
//CSS

html {
  font-size: 16px;  /* Tamanho da fonte do elemento raiz */
}

body {
font-size: 2rem;  /* Tamanho de fonte será 2 vezes a fonte do elemento raiz, nesse caso sendo 32px. */
}
```

### Definindo espaçamentos com “REM”:

```
//CSS

html {
  font-size: 16px; /* Tamanho da fonte do elemento raiz */
}

section {
  margin: 1rem; /* Margem será 16 pixels, independentemente do tamanho da fonte do elemento pai */
}
```

A escolha entre "EM" e "REM" depende das necessidades específicas do seu projeto. Ambas as unidades são usadas de forma complementar para criar designs acessíveis e responsivos.

Caso queira conhecer mais sobre unidades de medida, aconselho a leitura desse “[Guia de Unidades](https://www.alura.com.br/artigos/guia-de-unidades-no-css)”, escrito pelo instrutor Paulo Scalercio.

### [Voltar ao Menu - CSS: ajustando a acessibilidade visual em um projeto](../menu.md)
