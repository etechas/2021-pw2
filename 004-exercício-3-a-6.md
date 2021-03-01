# Exercícios de Aprendizagem

## Exercício 3

Crie uma classe chamada `ExercicioTres` com o método **main** que verifique se o usuário já tem idade mínima para adquirir carta de habilitação. Para isso, teremos uma variável `nome` que guarda um valor do tipo **String** e uma variável `idade` que guarda um valor do tipo inteiro.

O sistema deve cumprimentar o usuário independente da idade. Por exemplo:

- Caso o usuário tenha idade mínima para dirigir, exiba:
"Olá, **NOME_DO_USUARIO_AQUI**"
"Você passou no nosso teste e já pode dirigir!"

- Caso o usuário não tenha a idade mínima para dirigir, exiba somente o cumprimento:
"Olá, **NOME_DO_USUARIO_AQUI**"

### Resolução

``` java
public class ExercicioTres {
	
	public static void main(String[] args) {
		String nome = "Rogério";
		int idade = 37;
		
		System.out.println("Olá, " + nome);
		if (idade >= 18) {
			System.out.println("Você passou no nosso teste e já pode dirigir!");
		}		
	}

}

```

## Exercício 4

Crie uma classe chamada `ExercicioQuatro` com o método **main** que ajude um petshop a dizer se o bichinho de estimação está com o peso ideal. Para isso, eles deixaram as informações usadas para fazer essa classificação:

 - Abaixo de 4kg = Abaixo do peso
 - Maior que 10kg = Acima do peso
 - Se tiver entre esses dois valores = Peso normal.

> Utilizeo o **ELSE IF** e crie o código para suprir essa necessidade e exiba as mensagens de acordo com a lista acima!

### Resolução

``` java
public class ExercicioQuatro {
	
	public static void main(String[] args) {
		double peso = 4.5;
		if (peso < 4) {
			System.out.println("Abaixo do peso");
		} else if (peso > 10) {
			System.out.println("Acima do peso");
		} else {
			System.out.println("Peso normal");
		}
	}

}

```

## Exercício 5

Crie uma classe chamada `ExercicioCinco` que ajude os usuários a saber se podem ir ao banco. Sabemos que o banco está aberto em todos os os dias da semana, exceto em finais-de-semana. Caso o usuário possa ir ao banco, exiba a seguinte mensagem: "Você pode ir ao banco", caso contrário, "O banco está fechado, tente outro dia"

Para esse exercício, leve em consideração as seguintes informações:

- Dias da semana pro sistema: segunda, terca, quarta, quinta, sexta, sabado e domingo.
- Você terá a seguinte variável no código: `diaSemana`
- Use na condição do if o operador && para juntar as condições lógicas junto ao operador diferente de(!=).

### Resolução

``` java
public class ExercicioCinco {
	
	public static void main(String[] args) {
		String diaSemana = "domingo";
		if (diaSemana.equalsIgnoreCase("sabado") || diaSemana.equalsIgnoreCase("domingo")) {
			System.out.println("O banco está fechado, tente outro dia");
		} else {
			System.out.println("Você pode ir ao banco");
		}
	}

}
```

## Exercício 6

Crie uma classe chamada `ExercicioSeis` com o método **main** que declare um número inteiro e informe se é um número da sorte. Podemos dizer que é um número da sorte se o número:

- é positivo

- é um múltiplo de 2 ou 3

- não é 15


### Resolução

``` java
public class ExercicioSeis {
	
	public static void main(String[] args) {
		int numero = 23;
		if (numero > 0 && (numero % 2 == 0 || numero % 3 == 0) && numero != 15) {
			System.out.println(numero + " é um número da sorte");
		} else {
			System.out.println(numero + " não é um número da sorte");
		}
	}

}

```
