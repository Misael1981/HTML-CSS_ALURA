# CSS: o que é, como usar no HTML e um Guia para iniciar

<img src="./img/css.webp">

## Introdução

Olá, pessoa incrível! Hoje vamos abordar um tema que considero fundamental para qualquer pessoa que esteja na área de **desenvolvimento web**, ou até mesmo para aquelas que estão pensando em entrar nesse maravilhoso mundo. Vamos falar de CSS — Cascading Style Sheets. Prepare-se para mergulhar nessa aventura!

## O que é CSS?

Olá, pessoa incrível! Hoje vamos embarcar em uma aventura empolgante inspirada na lendária personagem Indiana Jones! Imagine que você é uma pessoa arqueóloga apaixonada por descobertas históricas e tesouros antigos. Assim como Indiana Jones, você está em busca de conhecimento e aventuras emocionantes. No entanto, em vez de explorar templos e ruínas antigas, a sua missão é desvendar os segredos do **CSS (Cascading Style Sheets)** — e dominar essa linguagem poderosa.

<img src="./img/indiana-jones.webp">

Assim como Indiana Jones enfrentava obstáculos desafiadores em suas expedições, você também enfrenta dificuldades em dominar o CSS. Você sabe que o CSS é essencial para criar belos e atraentes sites, mas sente-se perdido no meio de seletores, propriedades e valores. Você precisa desvendar esses mistérios e encontrar uma forma de aplicar corretamente o CSS em seus projetos.

Nesta jornada cheia de emoção e aventura, vamos seguir os passos de Indiana Jones e explorar os segredos ocultos do CSS. Assim como ele usava sua inteligência, habilidades, e ferramentas para superar desafios, decifrar hieróglifos e símbolos enigmáticos, você aprenderá sobre seletores, regras de estilo e blocos de declaração, vou te dar um gostinho, vamos a um exemplo:

```
seletor {
  propriedade: valor;
}
```

Veja que temos o **seletor**, que define a qual **elemento HTML** o estilo será aplicado, seguido por um **bloco de declarações** (dentro das chaves {}). Dentro desse bloco, temos a **propriedade** que queremos alterar e o **valor** dessa propriedade. Simples, não é mesmo?

O **CSS** permitirá que você **controle a aparência e o estilo dos elementos de um site**, assim como Indiana Jones desvendava enigmas e encontrava tesouros valiosos. Prepare-se para embarcar nessa aventura empolgante e descobrir os segredos do CSS! Não perca os próximos capítulos no universo do CSS!

## Importância do CSS no desenvolvimento web

Da mesma maneira que Indiana Jones precisa de seu chicote para se aventurar pelas cavernas escuras e resolver enigmas, nós, desenvolvedores web, precisamos do CSS para criar sites atraentes e funcionais. Por quê? Vamos explorar juntos.

<img src="./img/indiana-jones.webp">

Sem o CSS, nossos sites seriam como um mapa sem legendas — tecnicamente útil, mas incrivelmente difícil de entender. Um bom design não é apenas sobre tornar um site bonito, mas também melhorar a experiência do usuário. O CSS nos permite fazer isso, proporcionando uma **experiência de usuário** suave e agradável.

Você se lembra daquela cena em "Indiana Jones e a Última Cruzada" em que Indy escolhe o cálice certo entre tantos outros brilhantes, mas enganosos? Pois bem, o CSS é esse cálice humilde, mas valioso que torna tudo possível. Pode não ter o brilho imediato de outras tecnologias, mas sem ele, nossos sites seriam muito menos atraentes e eficazes.

Além disso, o CSS é essencial para a criação de **sites responsivos**. Com o aumento do uso de dispositivos móveis para acessar a web, é cada vez mais importante que nossos sites se adaptem a diferentes tamanhos de tela. Com o CSS, podemos garantir que nossos sites sejam tão bonitos e funcionais em um smartphone quanto em um desktop.

Por último, mas não menos importante, o CSS tem um papel crucial na acessibilidade na web. Ele nos permite criar sites que são acessíveis a todas as pessoas, independentemente de suas habilidades ou das tecnologias assistivas que possam estar usando.

Portanto, a importância do CSS no desenvolvimento web é indiscutível. Ele é a ponte de corda que nos permite cruzar o precipício do design funcional, a chave que nos ajuda a decifrar o enigma da experiência do usuário. Como Indy, devemos valorizar essa ferramenta e aproveitar ao máximo o seu potencial.

## Vantagens do uso do CSS

O CSS oferece uma variedade de vantagens que podem transformar a aparência e o funcionamento dos sites. Com o CSS, é possível:

1. **Personalizar** totalmente o visual do site;
2. Garantir a **eficiência** e **reutilização** de código;
3. Criar **sites responsivos**;
4. Melhorar a **acessibilidade**; e
5. Facilitar a **manutenção** do projeto.

## 1- Personalização à vontade

Com o CSS, você tem controle total sobre o visual do site. É possível definir cores, fontes, espaçamentos e muito mais, permitindo uma personalização completa para atender às suas preferências.

## 2- Eficiência e reutilização de código

O CSS permite escrever regras que podem ser aplicadas em vários elementos do site, evitando a repetição de estilos específicos. Isso resulta em menos código para escrever e manter, tornando o processo mais eficiente.

## 3- Site responsivo

Com as media queries do CSS, é possível adaptar o design do site de acordo com as características do dispositivo do usuário. Isso garante que o site seja visualmente atraente e funcional em diferentes tamanhos de tela, como smartphones, tablets e computadores.

## 4- Melhora a acessibilidade

O CSS desempenha um papel importante na criação de sites acessíveis. É possível ajustar o contraste das cores, o tamanho das fontes e outras características visuais para tornar o site mais acessível para usuários com deficiências visuais ou outras necessidades especiais.

## 5- Manutenção facilitada

Separar o design (CSS) do conteúdo (HTML) torna a manutenção do site mais fácil. Alterações no design podem ser feitas sem afetar o código HTML, simplificando o processo de manutenção e reduzindo a possibilidade de erros.

Assim como Indiana Jones desvendava segredos e encontrava tesouros valiosos, o CSS é uma ferramenta essencial para desvendar o **potencial visual e funcional dos sites**. Aproveite todas as vantagens do CSS e transforme suas criações web em verdadeiras jóias da internet!

## História do CSS

Compartilhar histórias é sempre uma aventura incrível. Assim como em qualquer grande saga, a trajetória do CSS também tem seu início, altos e baixos, e momentos marcantes. Então, prepare-se para embarcar nessa jornada ao passado!

## Surgimento do CSS

Em uma época muito distante, mais precisamente em **1994**, um engenheiro chamado Håkon Wium Lie propôs algo novo: uma **linguagem de estilização** que poderia resolver o caos visual do HTML da época. Ele imaginou uma maneira mais prática de implementar e controlar estilos visuais para páginas web. E foi assim que, em parceria com o W3C (World Wide Web Consortium), surgiu o CSS — Cascading Style Sheets.

## Versões do CSS

Assim como o tempo não para, o CSS também não ficou estagnado. A sua evolução veio em ondas, chamadas de níveis em vez de versões.

- **CSS1**: foi a primeira versão oficial, publicada em **1996**. Foi um grande passo à frente, já que permitiu aos desenvolvedores separar o conteúdo do design em seus sites pela primeira vez;

- **CSS2**: lançado em **1998**, trouxe novas funcionalidades como suporte para media types, que permitia a criação de estilos diferentes para impressão e visualização na tela, por exemplo;

- **CSS3**: aqui, as coisas ficaram um pouco mais complicadas. Em vez de lançar uma nova versão completa, o CSS3 foi dividido em **módulos menores**, cada um **lidando com diferentes aspectos do CSS**. Entre os avanços notáveis estão os efeitos de animação, transições e transformações, além do adorável flexbox.

## Principais marcos e avanços na evolução do CSS

Nessa longa trajetória, tivemos muitos marcos importantes. Dentre eles, podemos destacar:

- **Seletores Avançados**: introduzidos com o CSS3, eles deram aos desenvolvedores muito mais controle sobre quais elementos do DOM deveriam ser estilizados;

- **Media Queries**: essa é uma das principais ferramentas que permitem a criação de sites responsivos. As Media Queries permitem que você aplique estilos diferentes dependendo das características do dispositivo do usuário;

- **Flexbox e Grid**: ambos trouxeram uma revolução no design de layouts para a web, tornando muito mais fácil criar designs complexos e responsivos;

- **Variáveis CSS**: permitiram a definição de valores reutilizáveis ​​em todo o seu CSS, o que facilita muito a manutenção do código.

A viagem pela história do CSS é fascinante, não é mesmo? Agora que você já conhece um pouco mais sobre sua origem e evolução, está pronto para aprender mais.

## Estrutura e Sintaxe do CSS

Se a Web fosse uma grande aventura, o CSS seria nosso mapa. E, para navegar nesse mapa, precisamos entender a sua estrutura e a sua sintaxe. Afinal, você não quer se perder em um labirinto de código, não é mesmo?

### 1- Anatomia de uma regra CSS

Vamos começar pelo básico. Uma regra CSS é composta por:

- Um seletor; e
- Um bloco de declaração.

O **seletor** indica a quem a regra se aplica, e o **bloco de declaração** contém uma ou mais declarações que são aplicadas ao elemento selecionado.

Uma **declaração**, por sua vez, é composta por uma **propriedade** e um **valor**, separados por dois pontos. Ficaria assim:

```
seletor {
  propriedade: valor;
}
```
Bem simples, né? Agora vamos olhar mais de perto para cada parte desta regra.

### 2- Seletores CSS

Os seletores são como os nossos detetives. Eles vão à procura dos elementos que correspondem ao padrão que definimos. Existem vários tipos de seletores em CSS, mas aqui estão alguns dos mais usados:

- **Tipo**: selecione elementos pelo nome do elemento, como p, div, h1, etc;
- **Classe**: selecione elementos pela classe, usando um ponto (.) seguido do nome da classe;
- **ID**: selecione elementos pelo ID, usando uma hashtag (#) seguida do nome do ID.

### 3- Propriedades CSS

As propriedades são como os superpoderes dos elementos. Elas **controlam** tudo, desde a cor do texto até o tamanho da borda, passando pela fonte e o espaçamento. O CSS possui centenas de propriedades diferentes, o que proporciona um nível incrível de controle sobre a aparência de uma página web.

### 4- Valores e unidades no CSS

Cada propriedade tem um **conjunto específico de valores** que pode aceitar. Alguns são bastante simples, como auto ou none. Outros podem ser números, cores ou mesmo uma string de texto.

Muitos valores numéricos em CSS são acompanhados por uma **unidade de medida**. Por exemplo, você pode definir a largura de uma div em pixels (`px`), porcentagem (`%`), ems (`em`), ou várias outras unidades. Cada uma tem suas próprias características e usos.

## Box Model e Layout

Se você já teve que empacotar presentes, sabe que é preciso ter um bom entendimento de como as caixas funcionam para conseguir um bom resultado. Da mesma maneira, entender o modelo de caixa (Box Model) é fundamental para trabalhar com CSS. Vamos explorar esse universo agora.

### 1- Conceito de Box Model

No CSS, **cada elemento é considerado como uma caixa retangular**. Essa caixa é descrita por um modelo conhecido como Box Model, que é dividido em **quatro áreas**:

- Conteúdo (`content`);
- Preenchimento (`padding`);
- Borda (`border`); e
- Margem (`margin`).

Juntas, essas áreas definem como os elementos se relacionam entre si e como eles ocupam espaço na página.

### 2- Margem, borda e preenchimento (margin, border, padding)

Agora, vamos desempacotar cada parte do Box Model:

- **Margem (margin)**: é o espaço ao redor da caixa. Pense nela como um buffer que separa o elemento dos outros ao seu redor;

- **Borda (border)**: é a linha que envolve o preenchimento e o conteúdo;

- **Preenchimento (padding)**: é o espaço entre a borda e o conteúdo. Ele é como uma almofada que protege o conteúdo da borda;

### 3- Posicionamento de elementos

O posicionamento de elementos em CSS pode parecer uma versão de Tetris às vezes, onde estamos tentando encaixar diferentes blocos em um espaço limitado. Temos **várias propriedades para controlar o posicionamento**, incluindo:

- `position`;
- `top`;
- `right`;
- `bottom`;
- `left`; e
- `z-index`.

Com elas, você pode mover elementos para cima e para baixo, esquerda e direita, e até mesmo controlar o que fica na frente e o que fica atrás.

### 4- Layouts responsivos com CSS

Vamos pensar na responsividade como uma característica de um camaleão, adaptando-se ao ambiente. No caso do CSS, o ambiente são os diferentes tamanhos de tela e dispositivos. Usando media queries, podemos alterar estilos com base no tamanho da tela, criando uma **experiência que se adapta ao dispositivo do usuário**.

```
@media (max-width: 600px) {
  div {
    width: 100%;
  }
}
```

Entender o Box Model e o layout é como ter um mapa do tesouro que guia a localização e o posicionamento dos elementos na nossa página. E é incrível ver como o CSS nos dá o poder de transformar a Web de acordo com nossa vontade.

## Estilização de Texto e Tipografia

Você sabe quando entra em uma loja e o vendedor imediatamente reconhece que você procura algo único, que fala sobre quem você é? Assim funciona a estilização de texto e tipografia em CSS: elas definem a personalidade e a aparência do seu conteúdo escrito, criando uma experiência de leitura única.

### 1. Propriedades de texto

CSS nos oferece uma paleta cheia de opções para **moldar nosso texto**. Temos propriedades como:

- `color` para alterar a cor;
- `text-decoration` para **adicionar ou remover sublinhados**; e
- Até mesmo `text-transform` para alterar a capitalização do texto.

É como se estivéssemos em uma loja de chapéus, escolhendo a melhor peça para expressar nossa personalidade.

### 2. Fontes e tipografia

As fontes são para o nosso texto o que a trilha sonora é para um filme, elas estabelecem o tom, acentuam o clima e acrescentam uma camada extra de significado para a nossa mensagem. No CSS, podemos manipular a fonte de nosso texto com algumas propriedades específicas:

- `font-family`;
- `font-size`;
- `font-weight`; e
- `font-style`.

Além das fontes padrão que todos os navegadores conhecem, também temos a capacidade de usar qualquer fonte que quisermos em nossos projetos web. Tal qual Indiana Jones em busca de relíquias antigas, podemos vasculhar a internet em busca da fonte perfeita para nossa aventura web. E quando a encontramos, podemos trazê-la para nosso site com a ajuda do `@font-face`.

O `@font-face` é uma regra especial que nos permite **importar fontes de arquivos externos** para o nosso CSS. Ele precisa de algumas informações para funcionar corretamente, como:

- O nome da fonte (`font-family`);
- O caminho para o arquivo da fonte (`src`); e
- Outros parâmetros opcionais como `font-weight` e `font-style`.

```
@font-face {
  font-family: 'MinhaFontePersonalizada';
  src: url('MinhaFontePersonalizada.woff2') format('woff2'),
       url('MinhaFontePersonalizada.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
```

Depois que a fonte é declarada com `@font-face`, ela pode ser usada em todo o nosso CSS, como qualquer outra fonte.

```
h1 {
  font-family: 'MinhaFontePersonalizada', Arial, sans-serif;
}
```

Agora, com a capacidade de manipular e importar fontes, você possui um dos mais poderosos instrumentos na sinfonia que é o CSS. Cada palavra, cada frase, cada parágrafo podem agora dançar ao ritmo da sua música.

### 3. Efeitos de texto

Os efeitos de texto no CSS são como os acessórios que adicionamos ao nosso look. Com `text-shadow`, podemos **adicionar sombras** ao nosso texto, ou com `text-overflow`, podemos **controlar como o texto será exibido** quando ultrapassar o limite de sua caixa. É o toque final que dá um brilho extra ao nosso trabalho.

### 4. Espaçamento e alinhamento de texto

Finalmente, temos o espaçamento e alinhamento, que são como a postura e a maneira como nos apresentamos. Com `line-height`, `text-align`, `letter-spacing` e `word-spacing`, podemos **controlar a distribuição** e a **organização** do nosso texto, criando uma leitura confortável e agradável.

## Cores e Gradientes

As cores no CSS são como os efeitos especiais em um filme. Elas adicionam vida, criam atmosfera e podem até mesmo contar uma história. Então, como podemos pintar nossa tela digital?

### 1. Especificação de cores no CSS

Existem várias maneiras de especificar cores no CSS. Podemos usar **nomes de cores predefinidos**, como 'red' para vermelho, 'blue' para azul e assim por diante. Também podemos usar **códigos** hexadecimais, RGB, RGBA, HSL e HSLA.


```
p {
  color: red; /* nome da cor */
}

h1 {
  color: #ff0000; /* hexadecimal */
}

div {
  color: rgb(255, 0, 0); /* RGB */
}

span {
  color: rgba(255, 0, 0, 0.5); /* RGBA, com transparência */
}

header {
  color: hsl(0, 100%, 50%); /* HSL */
}

footer {
  color: hsla(0, 100%, 50%, 0.5); /* HSLA, com transparência */
}
```

### 2. Uso de cores sólidas

O uso de cores sólidas no CSS é bastante simples. Para aplicar uma cor a um elemento, basta usar a propriedade **color** para a cor do texto ou a propriedade **background-color** para a cor de fundo.

### 3. Gradientes lineares e radiais

O CSS também permite a criação de gradientes, que são **transições suaves entre duas ou mais cores**. Existem dois tipos de gradientes que podemos criar:

- Lineares; e
- Radiais.

Para criar um gradiente linear, usamos a função `linear-gradient()`.

### 4. Transparência e opacidade

A transparência pode ser especificada no CSS usando o formato **RGBA** ou **HSLA** para cores, ou a propriedade `opacity`. A propriedade `opacity` aplica uma transparência ao elemento inteiro, incluindo todo o seu conteúdo.

Assim como um pintor tem um arco-íris de cores à sua disposição, também temos um espectro ilimitado de cores à nossa disposição no CSS. Com as cores e gradientes, podemos criar designs vibrantes, dramáticos ou sutis, e transmitir o tom exato que queremos para nossa aplicação.

### [Menu CSS avançado](menu.md)











