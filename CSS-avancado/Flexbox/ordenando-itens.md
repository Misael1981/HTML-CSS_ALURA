# Ordenando itens

No mundo de desenvolvimento web, a criação de layouts responsivos e bem estruturados é essencial para garantir uma boa experiência do usuário em diferentes dispositivos e tamanhos de tela. O CSS Flexbox é uma ferramenta poderosa para isso, permitindo a criação de layouts flexíveis e alinhados com facilidade. Entre as suas propriedades, `display: flex` e `order` são particularmente importantes para controlar a disposição e a ordem dos elementos dentro de um contêiner flexível. Este texto explora como essas propriedades podem ser utilizadas para estilizar cabeçalhos, criar navegações flexíveis e responsivas, e ajustar layouts com media queries.

Criar layouts responsivos e bem organizados pode ser desafiador, especialmente quando se trata de alinhar elementos de forma precisa e controlar a ordem em que aparecem na tela. Por exemplo, um cabeçalho pode precisar ser centralizado e ter uma largura máxima, uma lista de navegação deve se adaptar a diferentes tamanhos de tela, e um campo de input de pesquisa deve ser estilizado adequadamente. Além disso, a ordem dos elementos pode precisar ser ajustada para diferentes visualizações, o que pode ser complexo sem uma abordagem sistemática.

O Flexbox fornece uma maneira mais eficiente e intuitiva de distribuir espaço e alinhar itens em um contêiner, mesmo quando o tamanho dos itens é desconhecido ou dinâmico.

- `display: flex`: Define o contêiner como um contêiner flexível, ativando as propriedades flexbox nos itens filhos. Os itens dentro do contêiner podem ser alinhados e distribuídos facilmente usando propriedades como `justify-content`, `align-items`, e `flex-direction`.

- `order`: Permite alterar a ordem visual dos itens dentro de um contêiner flexível sem alterar o HTML. https://cursos.alura.com.br/course/css-posicionando-elementos-flexboxItens com um valor de `order` menor aparecem antes dos itens com valores maiores. Isso é útil para ajustar a ordem dos elementos responsivamente.

### Exemplo de código usando `order`:

```
<div class="container">
    <div class="item1">Item 1</div>
    <div class="item2">Item 2</div>
    <div class="item3">Item 3</div>
</div>
```
```
.container {
    display: flex;
}

.item1 { order: 2; }
.item2 { order: 1; }
.item3 { order: 3; }
```

- `.item1` é exibido em segundo lugar.
- `.item2` é exibido em primeiro lugar.
- `.item3` é exibido em terceiro lugar.

Combinando essas propriedades com media queries, você pode criar layouts adaptáveis que mantêm a funcionalidade e a estética em diferentes dispositivos e tamanhos de tela.

### [Menu-CSS: posicionando elementos com Flexbox CSS](menu.md)

