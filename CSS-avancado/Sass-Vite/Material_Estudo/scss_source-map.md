# SCSS e source map

Durante a compilação manual de SCSS para CSS, notamos a criação de um arquivo .css.map, chamado source map. Este arquivo serve para mapear o código CSS compilado de volta para o código SCSS original, facilitando o processo de debug, especialmente quando trabalhamos com pré-processadores como o SCSS.

Quando você compila SCSS manualmente, precisa executar comandos separados e lidar com os arquivos .map, além de garantir que a compilação aconteça toda vez que o SCSS for alterado.

No entanto, ao usar ferramentas como o Vite, o processo de geração e uso dos source maps é automatizado. Isso significa que você não precisa configurar manualmente a criação desses arquivos ou gerenciá-los durante o desenvolvimento. O Vite compila o SCSS para CSS em tempo real, isso simplifica o fluxo de trabalho e reduz a necessidade de ajustes manuais.

### [Voltar ao menu - SASS com Vite: otimizando e modularizando seu CSS](../menu.md)