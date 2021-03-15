# Exercícios de Aprendizagem

## Exercício 7

Crie uma classe chamada `MinhasFuncoes` e escreva o método `triplo()` que pega um número como parâmetro e multiplica por 3.

### Resolução

``` java
public int triplo(int num) {
	return num * 3;
}
```

## Exercício 8

Escreva, na mesma classe `MinhasFuncoes`, o método `metade()` que receba um número como parâmetro e retorna sua metade.

### Resolução

``` java
public int metade(int num) {
	return num / 2;
}
```

## Exercício 9

Declare, também, o método `triploDaSoma()` que soma dois parâmetros e retornar o triplo do resultado. Para fazer isso, você já conta com o método `triplo()`.

### Resolução

``` java
public int triploDaSoma(int num1, int num2) {
	int resultado = num1 + num2;
	return num * 3;
}
```

## Exercício 10

Crie o método `tamanhoNomeCompleto` na classe `MinhasFuncoes` que receba um nome e um sobrenome como parâmetros e devolverá o tamanho total, contando um espaço extra para separar ambos.
> tamanhoNomeCompleto("Son", "Goku")
> devolve 8

### Resolução

``` java
public static int tamanhoNomeCompleto(String nome, String sobrenome) {
	String nomeCompleto = nome + " " + sobrenome;
	return nomeCompleto.length();
}
```

## Exercício 11

Crie o método `main` na classe `MinhasFuncoes` e exiba o resultado dos métodos `triplo()`, `metade()`, `triploDaSoma()` e `tamanhoNomeCompleto`.

### Resolução

``` java
public static void main(String[] args) {
		
	int resultadoTriplo = triplo(3);
	int resultadoMetade = metade(6);
	int resultadoTriploDaSoma = triploDaSoma(4, 6);
	int resultadoTamanhoNomeCompleto = tamanhoNomeCompleto("Rogério", "Morais");
		
	System.out.println("Triplo: " + resultadoTriplo);
	System.out.println("Metade: " + resultadoMetade);
	System.out.println("Triplo da soma: " + resultadoTriploDaSoma);
	System.out.println("Tamanho nome completo: " + resultadoTamanhoNomeCompleto);
	
}
```