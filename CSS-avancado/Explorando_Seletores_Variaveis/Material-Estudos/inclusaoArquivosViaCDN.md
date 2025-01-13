# Normalize CSS - Reset CSS: CDN vs. Arquivos Locais e Desempenho

A escolha entre incluir um reset ou normalizar CSS via CDN ou como arquivos locais pode influenciar o desempenho de sua página. Vamos analisar as diferenças:

## CDN (Content Delivery Network) vs. Arquivos Locais

- ### CDN:

    - #### Vantagens:
        - **Desempenho**: Os arquivos são entregues a partir de servidores distribuídos geograficamente, o que reduz a latência e melhora o tempo de carregamento, especialmente para usuários mais distantes.
        - **Cache**: Os arquivos são frequentemente armazenados em cache em navegadores e servidores intermediários, transmitindo o número de requisições e economizando banda.
        - **Manutenção**: As atualizações são gerenciadas pelo provedor do CDN, o que simplifica a manutenção.

    - #### Desvantagens:

        - **Dependência**: Você depende da disponibilidade e desempenho do serviço do CDN.
        - **Personalização**: Pode ser mais difícil personalizar ou redefinir ou normalizar CSS quando ele está em um CDN.

- ### Arquivos Locais:

    - #### Vantagens:

        - **Controle**: Você tem controle total sobre o arquivo e pode personalizá-lo como quiser.
        - **Disponibilidade: Não depende de serviços externos.

    - #### Desvantagens:

        - **Desempenho**: O arquivo precisa ser carregado do seu servidor, o que pode aumentar o tempo de carregamento, especialmente para usuários com conexões mais lentas.
        - **Manutenção**: Você precisa manter o arquivo atualizado.

### Normalize vs. Reset CSS

- **Redefinir CSS**: Remove quase todos os estilos padrão dos elementos HTML, criando uma base mais limpa para você aplicar seus próprios estilos.
- **Normalize CSS**: Corrige inconsistências entre navegadores e preserva estilos úteis, como listas e tabelas, fornecendo uma base mais sólida e consistente.

### Desempenho

- **Tamanho do Arquivo**: Arquivos menores geralmente carregam mais rápido. Tanto o reset quanto o normalize CSS são arquivos relativamente pequenos, mas a diferença pode ser significativa em projetos maiores.
- **Número de requisições**: Cada arquivo CSS adicional significa uma requisição HTTP a mais, ou que pode afetar o tempo de carregamento.
- **Minificação e Combinação**: Minificar (remover espaços em branco e comentários) e combinar arquivos CSS pode melhorar o desempenho.

### Qual é a escolha?

A melhor opção depende do seu projeto específico:

- **Prioridade em Desempenho**: Utilize um CDN para os arquivos de reset ou normalize CSS e combine-os com outros arquivos CSS para reduzir o número de requisições.
- **Controle e Personalização**: Se você precisa de um controle total sobre os estilos e deseja personalizá-los extensivamente, utilize arquivos locais.
- **Manutenção**: Se você não deseja se preocupar com atualizações, um CDN é uma boa opção.

### Considerações Adicionais:

- **Tamanho do Projeto**: Para projetos pequenos, a diferença de desempenho pode ser mínima.
- **Conexão do usuário**: A velocidade da conexão do usuário também influencia o tempo de carregamento.
- **Outras Otimizações**: Minificar e compactar outros arquivos (HTML, JavaScript, imagens) também contribui para um melhor desempenho.

- [Link para um Normalize CSS - via CDN](https://www.jsdelivr.com/package/npm/normalize.css)

- [Link para um Reset CSS - via CDN](https://www.jsdelivr.com/package/npm/reset)

### Em resumo:

- **CDN**: Geralmente oferece melhor desempenho, mas você perde um pouco de controle.
- **Arquivos Locais**: Oferecem mais controle, mas podem impactar o desempenho.
Normalizar vs. Redefinir: A escolha depende de suas necessidades específicas.

### Recomendação:

Para a maioria dos projetos, usar uma normalização de CSS via CDN é uma boa prática. O Normalize CSS oferece uma base mais sólida e consistente do que o reset CSS, e o CDN melhora o desempenho.

### [Menu - Explorando seletores e utilizando variáveis](../menu.md)