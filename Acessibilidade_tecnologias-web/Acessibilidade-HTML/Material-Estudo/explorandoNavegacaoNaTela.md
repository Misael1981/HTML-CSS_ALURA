# Explorando Navegação na Tela

Você começou a testar a navegação pelo teclado no projeto, e conferiu como a tag de âncora `<a></a>` auxilia dando interatividade para um elemento, pois quando ela é clicada, pode levar para alguma outra página ou link através do atributo `href=””`.

E você sabia que é possível redirecionar a pessoa que tiver utilizando a página para outra área da mesma página com essa tag?

Vou mostrar pra você utilizando o projeto como exemplo!

Se ao clicar na opção “Contato” no cabeçalho, a tela pode descer automaticamente para a área do formulário de contato mais abaixo:

<img src="../../img/acessibilidade-HTML-01.gif">

E como aplicar esse efeito?

Você primeiro precisa inserir um ID no elemento que deseja ter o foco após o clique. Nesse caso sendo o formulário como exemplo:

```
 <form action="." id="contato-formulario" class="container__contato--form">

///código do formulário oculto

</form>
```

E após isso, passar esse id para o caminho do atributo `href` da tag de âncora:

```
 <li class="cabecalho__lista-item"><a href="#contato-formulario">Contato</a></li>
```

Você pode testar com as outras opções do menu, encaminhando para outras áreas da página, lembrando que o valor de ID é sempre único e não deve ser repetido em um mesmo arquivo HTML.

### [Menu - Acessibilidade no HTML: escrevendo códigos semânticos para inclusão](../menu.md)
