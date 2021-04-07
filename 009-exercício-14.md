# Exercícios de Aprendizagem

## Exercício 12

Alterar a classe `AtividadeAvaliativa<SeuNome>` incluindo os métodos:

-`calcularVelocidadeCarro()` que receba a frequência do veículo e retorne a velocidade
-`calcularLimite20PorcentoEstrada()` que receba o limite de velocidade da estrada e retorne o valor de 20% acima
-`calcularValorMulta()` que receba a frequência do veículo e  o limite de velocidade da estrada e retorne o valor da multa.

> Utilize os métodos acima para não repetir os cálculos.

### Resolução `calcularVelocidadeCarro()`

``` java
public static double calcularVelocidadeCarro(double frequenciaCarro) {
	return 300 * (1 / frequenciaCarro - 1);
}
```

## Resolução `calcularLimite20PorcentoEstrada()`

``` java
public static double calcularLimite20PorcentoEstrada(int velocidadeLimite) {
	return velocidadeLimite * 1.2;
}
```

## Resolução `calcularValorMulta()`

``` java
public static double calcularValorMulta(double frequenciaCarro, int velocidadeLimite) {
	double velocidadeCarro = calcularVelocidadeCarro(frequenciaCarro);
	double limite20PorCento = calcularLimite20PorcentoEstrada(velocidadeLimite);
	if (velocidadeCarro <= velocidadeLimite) {
		return 0.0;
	} else if (velocidadeCarro <= limite20PorCento) {
		return 127.69;
	} else {
		return 574.62;
	}
}
```

## Resolução `main()`

``` java
public static void main(String[] args) {
	double frequenciaCarro = 0.7;
	int velocidadeLimite = 120;
	
	double velocidadeCarro = calcularVelocidadeCarro(frequenciaCarro);
	System.out.println("Velocidade do carro: " + velocidadeCarro + " km/h.");
	
	double multa = calcularValorMulta(frequenciaCarro, velocidadeLimite);
	System.out.println("Multa de: R$ " + multa);
}
```