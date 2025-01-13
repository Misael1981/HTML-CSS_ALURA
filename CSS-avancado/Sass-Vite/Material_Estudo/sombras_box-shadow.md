# xplorando as sombras com box-shadow

No CSS, a **propriedade box-shadow** oferece uma grande flexibilidade na criação de sombras para elementos. E há também algumas configurações que podem ampliar ainda mais o seu uso.

#### O valor de box-shadow é composto por até seis parâmetros:

- **Deslocamento horizontal (offset-x)**: define o quanto a sombra será movida na direção horizontal.
- **Deslocamento vertical (offset-y)**: define o quanto a sombra será movida na direção vertical.
- **Raio de desfoque (blur-radius)**: controla o quanto a sombra será borrada. Quanto maior o valor, mais difusa será a sombra.
- **Raio de propagação (spread-radius)**: define o quanto a sombra irá crescer ou diminuir. Valores positivos expandem a sombra, enquanto negativos a contraem.
- **Cor (color)**: a cor da sombra, que pode ser sólida ou com opacidade (usando rgba ou hsla).
- **Inset**: palavra-chave opcional que inverte a sombra, criando um efeito de sombra interna.

A estrutura geral é a seguinte:

```
box-shadow: offset-x offset-y blur-radius spread-radius color;
```

## Aplicações

**Sombra múltipla**: é possível adicionar várias sombras em um único elemento, separando cada sombra com uma vírgula. 

### Exemplo:

```
box-shadow: 2px 4px 6px rgba(0, 0, 0, 0.5), -3px -3px 8px rgba(255, 255, 255, 0.3);
```

**Sombras internas**: usando o valor inset, você pode criar sombras que são aplicadas dentro do elemento, ao invés de fora. Isso é útil para criar profundidade em campos de formulário ou simular um efeito de "rebaixamento". 

### Exemplo:

```
box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.5);
```

Para explorar mais exemplos e entender melhor os diferentes usos da propriedade box-shadow, você pode consultar a [documentação oficial no MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS/box-shadow), que oferece uma visão aprofundada sobre a sintaxe, parâmetros e melhores práticas.

Além disso, para ver o efeito visual de box-shadow em tempo real, você pode utilizar uma ferramenta interativa como o [CSS Box-Shadow Generator](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_backgrounds_and_borders/Box-shadow_generator). Essa ferramenta permite ajustar os valores de deslocamento, desfoque, propagação e cor da sombra, ajudando a visualizar diferentes estilos e aplicar o código diretamente no seu projeto.

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)