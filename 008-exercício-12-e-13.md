# Exercícios de Aprendizagem

## Exercício 12

Crie o método `cartaoDeVisita` na classe `MinhasFuncoes` que gere um cartão de visita com os parâmetros nome, sobrenome e profissão, retornando a concatenação dessas informações.

### Exemplo

`Nome:` Beatriz

`Sobrenome:` Soares

`Profissão:` Programadora

`Cartão de visita esperado:` "Beatriz Soares - Programadora"

### Resolução

``` java
public static String cartaoDeVisita(String nome, String sobrenome, String profissao) {
	return nome + " " + sobrenome + " - " + profissao;
}
```

## Exercício 13

Os engenheiros de uma montadora estão projetando o computador de bordo de um carro. Eles precisam de um método que possa calcular a autonomia atual do automóvel, em outras palavras, quantos quilômetros ele consegue andar com a quantidade de combustível atual. A autonomia pode ser obtida multiplicando a quantidade de combustível pelo rendimento. 

Escreva o método `autonomia` que recebe os parâmetros de quantidade de combustível e rendimento e retorna a autonomia do automóvel.

### Resolução

``` java
public static double autonomia(double quantidadeDeCombustivel, int rendimento){
	return rendimento * quantidadeDeCombustivel;
}
```