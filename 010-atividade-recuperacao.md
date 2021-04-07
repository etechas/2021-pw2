# Atividade de Recuperação

## SABESP

A Sabesp cobra um valor base de consumo de água multiplicando-se o consumo mensal (em m³) por uma tarifa dada pelas tabelas abaixo.

> SOCIAL Residencial

| Consumo (m³)  | Tarifa (R$)                |
|---------------|----------------------------|
|  0 a 10       | 9,18 p/ mês (taxa mínima)  |
| 11 a 20       | 1,58 / m³                  |
| 21 a 30       | 5,61 / m³                  |
| 31 a 50       | 8,00 / m³                  |
| Acima de 50   | 8,84 / m³                  |




> NORMAL Residencial

| Consumo (m³)  | Tarifa (R$)                |
|---------------|----------------------------|
|  0 a 10       | 27,07 p/ mês (taxa mínima) |
| 11 a 20       |  4,24 / m³                 |
| 21 a 50       | 10,58 / m³                 |
| Acima de 50   | 11,65 / m³                 |


O consumidor que paga as tarifas da tabela `Social Residencial` deve atender as seguintes exigências:

1. Ter renda familiar de até 3 salários mínimos (atualmente em R$ 1.100,00)
2. Ser morador de habitação com área útil construída menor que 60m²
3. Ser consumidor de energia elétrica com consumo de até 170 kwh/mês

Portanto, para calcular a conta da Sabesp, estes dados devem ser informados.

### Exemplo

#### Entrada
`Salário:` 1200

`Área construída:` 50

`Consumo elétrico (kwh):` 90

`Consumo água (m³):` 10


#### Saída
`Consumo:` 10 m³

`Total:` R$ 9,18

### TAREFA

Crie uma classe chamada `Recuperacao<SeuNome>` com o método **main** com as variáveis de entrada e exiba a conta da Sabesp com o consumo e o valor total a ser pago. A classe terá os métodos:

- ehSocialResidencial() que receberá o salário, a área construída e o consumo elétrico e devolverá true para o caso de consumidor Social Residencial ou false, caso contrário;

- calcularConsumoSocial() que receberá o consumo de água e retornará o valor total a pagar de conta de água conforme tabela Social Residencial;

- calcularConsumoNormal() que receberá o consumo de água e retornará o valor total a pagar de conta de água conforme tabela Normal Residencial;

- main() com as variáveis de entrada e a exibição do consumo em m³ e do total a pagar. Não esqueça de utilizar os métodos acima para determinar o tipo de conta (social/normal) e o valor a pagar.


#### Casos de teste

**Entrada**

`Salário:` 1200

`Área construída:` 50

`Consumo elétrico (kwh):` 90

`Consumo água (m³):` 10


**Saída**

`Consumo:` 10 m³

`Total:` R$ 9,18


--------------------------------------------

**Entrada**

`Salário:` 1200

`Área construída:` 50

`Consumo elétrico (kwh):` 90

`Consumo água (m³):` 30


**Saída**

`Consumo:` 30 m³

`Total:` R$ 168,30


--------------------------------------------

**Entrada**

`Salário:` 1200

`Área construída:` 50

`Consumo elétrico (kwh):` 190

`Consumo água (m³):` 10


**Saída**

`Consumo:` 10 m³

`Total:` R$ 27,07


--------------------------------------------

**Entrada**

`Salário:` 1200

`Área construída:` 50

`Consumo elétrico (kwh):` 190

`Consumo água (m³):` 30


**Saída**

`Consumo:` 30 m³

`Total:` R$ 317,40

