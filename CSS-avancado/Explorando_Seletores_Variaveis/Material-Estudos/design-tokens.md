# Design Tokens

Ao criar um site, muitas vezes você precisa reutilizar as mesmas cores, fontes, espaçamentos, e outros elementos de design em diferentes partes do projeto. Manter tudo isso consistente é um desafio, especialmente quando o projeto cresce e novas páginas ou componentes são adicionados.

Conforme você vai desenvolvendo, percebe que ter que lembrar de cada cor, tamanho de fonte, ou espaçamento específico para cada parte do site é uma tarefa muito difícil. Além disso, quando o designer decide mudar a cor principal do site, você tem que caçar e substituir manualmente essas cores em diversos arquivos e linhas de código. É aí que você deve ter ferramentas para se salvar em situações como essa.

Aqui entram o que chamamos de **Design Tokens** (pode ser traduzido como elementos de design). Eles são como variáveis que guardam valores de design, como cores, fontes, tamanhos, etc. Em vez de codificar diretamente uma cor ou tamanho em seu CSS, você cria um token que guarda esse valor. Assim, se você precisar mudar algo, altera apenas o token, e o resto do site é atualizado automaticamente.

Exemplo de como isso pode ser feito em CSS usando variáveis:

```
:root {
  --cor-primaria: #3498db;
  --espacamento-padrao: 16px;
}

body {
  color: var(--cor-primaria);
  padding: var(--espacamento-padrao);
}
```

Se, mais tarde, você precisar mudar a cor principal, basta alterar `--cor-primaria`, e todos os lugares onde ela é usada serão atualizados de uma vez.

**Design tokens** são uma prática de desenvolvimento que centraliza e padroniza os valores de design de um projeto. Eles ajudam a manter a consistência e facilitam a manutenção e a escalabilidade do código. Os tokens podem ser usados para cores, espaçamentos, fontes, bordas, e qualquer outro valor repetido no design. Algumas das vantagens de usar essa estratégia são:

- **Centralização**: tudo em um só lugar. Você altera o valor de um token, e essa mudança reflete em todo o projeto.
- **Consistência**: reduz o risco de inconsistências no design, já que você usa os mesmos tokens em todo o código.
- **Manutenção**: facilita a atualização do design ao longo do tempo, tornando o processo mais ágil e menos propenso a erros.

Nas etapas iniciais do projeto é interessante avaliar se o seu projeto dispõe de um guia de estilos e se ele pode ser transformado em tokens de design. Fazendo isso você está adotando boas práticas desde o início do desenvolvimento, evitando futuros problemas com seu código, adotando práticas que grandes empresas de tecnologia utilizam em seus sistemas de design.

- ### [Quer se aprofundar no assunto? Confere este artigo do Carlos Henrique Filho na plataforma do Medium falando sobre tokens de design.](https://brasil.uxdesign.cc/o-que-s%C3%A3o-design-tokens-cd408431727d)

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)