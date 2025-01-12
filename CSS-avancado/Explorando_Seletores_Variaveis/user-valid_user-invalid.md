# :user-valid e :user-invalid

A um tempo atrás, se você quisesse estilizar campos de formulários de forma a dar um feedback sobre as informações neles serem válidas ou não, você provavelmente usaria `:valid` e `:invalid` para aplicar esses estilos.

O problema é que esses seletores poderiam aplicar estilos antes mesmo do usuário interagir com o formulário, e isso provavelmente geraria uma experiência negativa ao mostrar mensagens de erro antes deles acontecerem.

E como resolver este impasse? É aqui que entram os seletores `:user-valid` e `:user-invalid`. Eles são semelhantes a `:valid` e `:invalid`, mas só aplicam o estilo após o usuário ter interagido com o campo, proporcionando uma melhor experiência.

### Exemplo:

```
input:user-valid {  border-color: green;}input:user-invalid {  border-color: red;}
```

Com esses novos seletores, não é mais necessário escrever um código com estado para acompanhar as entradas alteradas por um usuário. Os estilos são aplicados somente após a interação do usuário. Se o estado do campo era válido antes do usuário interagir, esses estilos só irão mudar quando o usuário mudar o foco para outro elemento. O mesmo vale para o user-invalid.

Estes seletores são relativamente novos e vale a pena checar a compatibilidade deles com navegadores mais antigos. Se você quiser se aprofundar nesses novos seletores, vou deixar um [artigo muito legal do blog web.dev mostrando o uso e permitindo que você interaja em tempo real com elementos com esses seletores](https://web.dev/articles/user-valid-and-user-invalid-pseudo-classes?hl=pt-br).

### [Menu - Explorando seletores e utilizando variáveis](./menu.md)