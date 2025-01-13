# Enésimo Seletor

Imagina que você está criando uma galeria de imagens e quer que a primeira imagem de cada linha seja maior que as outras. Além disso, você deseja destacar todos os itens pares de uma lista de artigos, alternando a cor de fundo. Fazer isso manualmente, estilizando cada item individualmente, seria uma dor de cabeça.

Para ter as funcionalidades que você quer, você precisa ***aplicar estilos específicos a elementos que seguem uma certa ordem ou padrão***, como "todos os itens pares", "o terceiro item", ou "cada quarto item". Fazer isso de forma manual não é uma boa ideia, especialmente se os elementos mudarem de posição ou se novos itens forem adicionados.

Para fugir dessa complexidade de fazer tudo manual, o css dispões de pseudo-classes chamadas de “enésimo seletor” (aqueles que começam com `:nth-`).

### Alguns dos enésimos seletores mais usados são:

- `:nth-child(n)`: seleciona o enésimo filho, onde “n” pode ser um número, uma palavra-chave (como odd ou even), ou uma expressão (como 2n+1);

- `:nth-of-type(n)`: semelhante ao `:nth-child`, mas considera apenas elementos do mesmo tipo;

- `:nth-last-child(n)`: funciona como o `:nth-child`, mas começa a contagem de trás para frente;

- `:nth-last-of-type(n)`: combina as características de `:nth-of-type` e `:nth-last-child`;

### Exemplos práticos:

#### 1 - Para destacar todos os itens pares de uma lista (`<li>`):

```
li:nth-child(even) {
  background-color: #f2f2f2;
}
```

#### 2 - Para deixar a primeira imagem de cada linha maior:

```
.gallery img:nth-child(4n+1) {
  width: 150%;
}
```

#### 3 - Para aplicar um estilo ao último item de uma lista:

```
li:nth-last-child(1) {
  font-weight: bold;
}
```

Os “enésimos seletores” do CSS são poderosos recursos que permitem aplicar **estilos com base na posição de um elemento dentro de sua estrutura de pai**. Isso é útil para criar padrões visuais dinâmicos e responsivos, mantendo o HTML limpo e o CSS organizado.

Ficou curioso sobre a existência desses seletores? Dá uma olhada na [documentação aqui neste link](https://www.w3schools.com/cssref/css_selectors.php) e veja se descobre um novo.

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)