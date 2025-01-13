# Precedência e Especificidade de Estilos CSS

Você está trabalhando em um projeto de site e define que todos os botões devem ter um fundo azul. Mais tarde, o designer pede que um botão específico, com a classe `.especial`, tenha um fundo vermelho. Você escreve o CSS, mas, para sua surpresa, o botão continua azul.

O CSS não aplicou o estilo do botão `.especial` como você esperava. Apesar de ter definido a cor de fundo como vermelho, o botão ainda aparece azul. O que é que está acontecendo?

O problema está na especificidade e precedência de estilos. No CSS, regras com maior especificidade têm prioridade sobre outras menos específicas. A especificidade é calculada com base no seletor usado:

- **ID (`#id`)** tem a maior especificidade.
- **Classes (`.classe`)**, pseudo-classes (`:hover`) e atributos têm especificidade intermediária.
- **Elementos (`div, button`)** e pseudo-elementos (`::before`) têm a menor especificidade.

Lembrando que **estilos inline** possuirão sempre a maior especificidade quando usados.

Se um seletor for mais específico, ele prevalece sobre outros, independentemente da ordem em que aparecem no CSS. Para resolver seu problema, você pode aumentar a especificidade do seletor do botão especial:

```
button.especial {
  background-color: red;
}
```

Se ainda assim não funcionar, pode ser que outra regra com maior especificidade ou um `!important` esteja interferindo.

No CSS, quando múltiplas regras se aplicam ao mesmo elemento, a precedência e especificidade decidem qual estilo é aplicado:

1. **Especificidade**: é como uma pontuação dada a cada seletor. Quanto mais específico, mais alta a pontuação, e ele terá prioridade.
2. **Ordem de Aparição**: se dois seletores têm a mesma especificidade, a regra definida por último no CSS será aplicada.
3. **Herança e Cascata**: estilos podem ser herdados de elementos pai e se acumulam conforme você desce na estrutura do documento.

Aqui vai um exemplo de como a especificidade funciona:

```
/* Especificidade baixa */
button {
  color: white;
}

/* Especificidade média */
.especial {
  color: black;
}

/* Especificidade alta */
button.especial {
  color: red;
}
```

Nesse caso, o botão com a classe `.especial` terá o texto na cor vermelha, pois `button.especial` é o seletor mais específico. Entender essas regras de precedência vai te salvar de muita dor de cabeça na hora de estilizar seus sites! Por isso, se você quiser se aprofundar no assunto eu vou deixar este [artigo da plataforma Medium](https://medium.com/emanuelg-blog/entendendo-a-preced%C3%AAncia-de-estilo-em-css-especificidade-heran%C3%A7a-e-efeito-cascata-a437c4929173) sobre especificidade e precedência de estilos no CSS do **Emanuel G de Souza**.

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)