# Exercícios de C — IF e ELSE

## Orientações

Para cada exercício:

1. Identifique as entradas.
2. Identifique o processamento.
3. Identifique a condição.
4. Identifique as saídas.
5. Desenvolva o algoritmo.
6. Desenvolva o fluxograma.
7. Depois, implemente a solução em C utilizando `if` e `else`.

---

## 1. Frete grátis

Faça um programa que leia o valor de uma compra e informe se o cliente terá direito a **frete grátis**.

A loja oferece frete grátis para compras com valor **maior ou igual a R$ 150,00**.

Caso o valor da compra seja menor que R$ 150,00, o cliente deverá pagar pelo frete.

### Exemplo

```
Digite o valor da compra: 200

Frete gratis!

```

### Exemplo 2

```
Digite o valor da compra: 120

Frete a pagar.

Valor da Compra com Frete: R$ 150

```

### Regra

```
Valor da compra >= R$ 150,00
        ↓
      Frete grátis

Valor da compra < R$ 150,00
        ↓
      Frete a pagar (R$ 30)

```

---

## 2. Consumo de combustível

Faça um programa que leia a quantidade de **quilômetros percorridos** por um carro e a quantidade de **litros de combustível consumidos**.

O programa deverá calcular o consumo médio do veículo e informar se o veículo é considerado **econômico** ou possui **consumo alto**.

Considere que veículos com consumo **maior ou igual a 12 km/l** são considerados econômicos.

### Exemplo

```
Digite a distância percorrida: 480
Digite a quantidade de litros consumidos: 40

Consumo médio: 12.00 km/l
Veiculo economico!

```

### Exemplo 2

```
Digite a distância percorrida: 400
Digite a quantidade de litros consumidos: 40

Consumo médio: 10.00 km/l
Consumo alto!

```

### Fórmula

```
consumo = distância / litros

```

### Regra

```
Consumo >= 12 km/l
        ↓
   Veículo econômico

Consumo < 12 km/l
        ↓
     Consumo alto

```

---
<!-- 
## Formulário de Entrega

[Formulário](https://forms.cloud.microsoft/r/UEgjudBjPb)

--- -->

## Objetivo

Praticar a transformação de um problema em:

```
Problema
   ↓
Algoritmo
   ↓
Fluxograma
   ↓
Código em C

```

### Conceitos trabalhados

- Variáveis
- Entrada de dados
- Saída de dados
- Operadores matemáticos
- Operadores de comparação
- Estruturas de decisão
- `if`
- `else`
- Organização do algoritmo
- Construção de fluxogramas
- Implementação em C