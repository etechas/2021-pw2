# Métodos de Classe

Um método é um **bloco de código** que podemos invocar quantas vezes forem necessárias, permitindo **agrupar o código** que vamos **utilizar muitas vezes**.

## Estrutura de um método

### Modificador de Acesso

Usamos a palavra `public` para informar ao Java que podemos utilizar o método em outro lugar.

![Modificador de Acesso {w=62}](imagens/006-metodos-de-classe/modificador-acesso.png)

### Tipo do resultado

Definimos o `tipo` de retorno do resultado do processo que estamos fazendo dentro do método.

![Tipo do resultado {w=62}](imagens/006-metodos-de-classe/tipo-resultado.png)

### Nome

Definimos um `nome` para nos referirmos ao nosso método quando quisermos invocá-lo.

![Nome {w=62}](imagens/006-metodos-de-classe/nome.png)

### Parâmetros

Escrevemos os parênteses e, dentro deles, os parâmetros da função separados por vírgulas.

![Parâmetros {w=62}](imagens/006-metodos-de-classe/parametros.png)

Dentro de nosso método, podemos acessar os parâmetros como se fossem variáveis.

![Parâmetros {w=62}](imagens/006-metodos-de-classe/uso-parametros.png)

### Corpo

Entre as chaves de abertura e fechamento escrevemos o código que queremos que seja executado toda vez que invocamos o método.

![Corpo {w=62}](imagens/006-metodos-de-classe/corpo.png)

### Retorno

Para retornar ao exterior o resultado do processamento que estamos fazendo dentro do método, usamos a palavra reservada `return` seguida do que quisermos devolver.

![Palavra reservada RETURN {w=62}](imagens/006-metodos-de-classe/palavra-reservada-return.png)

## Exemplo de Método

Com os métodos, podemos fazer muitas coisas, mas vamos começar com algo fácil. Veja esse exemplo onde o método a seguir dobra o valor do número que passamos para ele:

```java
public int dobrar(int num) {
   return num * 2;
}
```
