# Boas Práticas com Tabindex

Elementos que possuem foco devem ser os que têm interação de fato na página, como inputs, botões e links. Esses elementos possuem o atributo `tabindex` com valor 0, que permite o foco.

É possível alterar a ordem de foco, como no exemplo abaixo:

```
<ul class="cabecalho__nav--lista">
    <li tabindex=”2” class="cabecalho__lista-item"><a href="#">Espaço</a></li>
    <li tabindex=”1” class="cabecalho__lista-item"><a href="#">Serviços</a></li>
    <li tabindex=”0” class="cabecalho__lista-item"><a href="#">Contato</a></li>
</ul>
```

No exemplo acima, o foco pela navegação com tabindex será nesta ordem: “Contato” em primeiro lugar, “Serviços” em segundo e “Espaço” em terceiro. Ou seja, quanto mais próximo de 0, maior será a prioridade, e quanto maior o valor, menor será a prioridade. Já valores negativos podem ser aplicados para retirar o foco do elemento.

Entretanto, existe uma série de boas práticas para a acessibilidade que a **WCAG Web Content Accessibility Guidelines** nos orienta! Existe até uma [sessão específica falando sobre o uso do atributo tabindex](https://www.w3.org/WAI/ARIA/apg/practices/keyboard-interface/) que traz algumas dicas muito interessantes! Partiu conhecer?

- Foco de tela discernível e previsível. Apesar do tabindex permitir aplicar a ordem que você quiser, o ideal é que todos os elementos com foco tenham o mesmo valor, pois isso faz com que eles sejam selecionados de acordo com a ordem no HTML. E no que isso ajuda na acessibilidade? Imagina uma página onde a navegação pelo teclado não segue uma ordem padrão, indo para o final da página e depois para o topo e vice versa, isso seria ruim para a usabilidade, não é mesmo? Por exemplo, pessoas do espectro autista podem ficar confusas ao utilizar uma página, ou até mesmo uma pessoa cega pode não saber em que área da página está no momento.
- Para que uma página web seja acessível, todos os elementos interativos devem ser operáveis através do teclado. Dessa forma, uma pessoa que não pode utilizar o mouse terá a habilidade de selecionar elementos interativos que quiser, sejam links, botões ou campos de formulário.
- Visibilidade do indicador de foco: Os usuários precisam ser capazes de distinguir facilmente o indicador de foco do teclado de outros recursos do design visual. Assim como um usuário de mouse pode movê-lo para ajudar a encontrar o ponteiro do mouse, um usuário de teclado pode pressionar uma tecla de navegação para observar o movimento. Por exemplo, um botão com foco terá uma borda que indicará o foco. A WCAG indica que utilize os estilos padrão de foco dos navegadores, mas caso queira adaptar para um projeto específico, leve em consideração o uso de contraste de cores acessível.
- Não defina o foco inicial quando a página for carregada, exceto nos casos em que:
  - A página oferece uma função única e primária que quase todos os usuários empregam imediatamente após o carregamento da página.
  - É provável que qualquer usuário use a página com frequência.

As orientações da WCAG são sempre a melhor fonte para aplicar acessibilidade em projetos Web, por isso estamos seguindo este parâmetro no decorrer do curso!

### [Menu - Acessibilidade no HTML: escrevendo códigos semânticos para inclusão](../menu.md)
