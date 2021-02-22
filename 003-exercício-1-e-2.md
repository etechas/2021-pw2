# Exercícios de Aprendizagem

## Exercício 1

Crie uma classe chamada `ExercicioUm` com o método **main** que declare e atribua três variáveis, uma com o seu `nome`, outra com o seu `sobrenome` e outra com a sua `idade`. Então, declare uma variável com nome `resultado` que una suas variáveis da seguinte forma: "Horácio Augusto da Silveira tem 30 anos".

> Utilize o System.out pra mostrar o que acontece e respeite os espaços!

### Resolução

``` java
public class ExercicioUm {
	
	public static void main(String[] args) {
		
		String nome = "Rogério";
		String sobrenome = "de Morais";
		int idade = 37;
		String resultado = nome + " " + sobrenome + " tem " + idade + " anos";
		System.out.println(resultado);
	}

}
```

## Exercício 2

Crie uma classe chamada `ExercicioDois` com o método **main** e defina a variável `numeroA` com um valor de **30** e defina a variável `numeroB` com um valor de **45**. Em seguida, faça a variável `numeroA` armazenar o valor da variável `numeroB` e vice-versa. Neste procedimento, você precisa criar uma terceira variável chamada de `numeroC` para armazenar o valor da variável `numeroA`.

> Utilize o System.out pra mostrar o que acontece.

### Resolução

``` java
public class ExercicioDois {
	
	public static void main(String[] args) {
		
		int numeroA = 30;
		int numeroB = 45;
		int numeroC = numeroA;
		numeroA = numeroB;
		numeroB = numeroC;
		
		System.out.println("A: " + numeroA);
		System.out.println("B: " + numeroB);
		
	}

}
```
