# Exercícios de C — IF e ELSE

## Orientações

**Para cada exercício:**

**1. Identifique as entradas.**

**2. Identifique o processamento.**

**3. Identifique a condição.**

**4. Identifique as saídas.**

**5. Desenvolva o algoritmo.**

**6. Desenvolva o fluxograma.**

**7. Depois, implemente a solução em C utilizando `if` e `else`.**

---

## 1. Bônus salarial

Faça um programa que leia o salário de um funcionário e calcule o valor do bônus que ele receberá.

A empresa oferece um bônus de **10% do salário** para funcionários que recebem **R$ 3.000,00 ou mais**.

Funcionários que recebem menos de R$ 3.000,00 não recebem bônus.

O programa deverá calcular e apresentar o **valor do bônus** e o **salário final**.

### Exemplo

```text
Digite o salario: 4000

Bonus: R$ 400.00
Salario final: R$ 4400.00
```

### Exemplo 2

```text
Digite o salario: 2500

Sem bonus.
Salario final: R$ 2500.00
```

### Fórmulas

```text
bonus = salario * 10 / 100

salarioFinal = salario + bonus
```

### Regra

```text
Salário >= R$ 3000,00
        ↓
     Bônus de 10%

Salário < R$ 3000,00
        ↓
      Sem bônus
```

---

## 2. Temperatura

Faça um programa que leia uma temperatura em graus Celsius e informe se a temperatura está considerada **quente** ou **não quente**.

Considere que temperaturas **maiores ou iguais a 30°C** são consideradas quentes.

Temperaturas abaixo de 30°C são consideradas não quentes.

### Exemplo

```text
Digite a temperatura: 35

Temperatura quente!
```

### Exemplo 2

```text
Digite a temperatura: 25

Temperatura nao quente.
```

### Regra

```text
Temperatura >= 30°C
        ↓
Temperatura quente

Temperatura < 30°C
        ↓
Temperatura não quente
```

---

## 3. Votação

Faça um programa que leia o **ano de nascimento de uma pessoa** e informe se ela poderá ou não votar no ano atual.

Para este exercício, considere o ano atual como **2026** e não é necessário considerar o mês em que a pessoa nasceu.

O programa deverá calcular a idade da pessoa e verificar se ela possui idade suficiente para votar.

### Exemplo

```text
Digite o ano de nascimento: 2000

Idade: 26 anos
Pode votar!
```

### Exemplo 2

```text
Digite o ano de nascimento: 2015

Idade: 11 anos
Nao pode votar!
```

### Fórmula

```text
idade = 2026 - anoNascimento
```

### Regra

```text
Idade >= 16 anos
        ↓
     Pode votar

Idade < 16 anos
        ↓
   Não pode votar
```

---

## 4. Validação de senha

Faça um programa que leia uma **senha fornecida pelo usuário**.

A senha válida é o número **1234**.

O programa deverá verificar se a senha informada está correta e apresentar uma das seguintes mensagens:

**ACESSO PERMITIDO** caso a senha seja válida.

**ACESSO NEGADO** caso a senha seja inválida.

### Exemplo

```text
Digite a senha: 1234

ACESSO PERMITIDO
```

### Exemplo 2

```text
Digite a senha: 5678

ACESSO NEGADO
```

### Regra

```text
Senha == 1234
      ↓
ACESSO PERMITIDO

Senha != 1234
      ↓
ACESSO NEGADO
```

---

## Objetivo

Praticar a transformação de um problema em:

```text
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
