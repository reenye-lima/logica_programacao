# Exercícios de C — Operadores E e OU com IF

## Orientações

Nesta atividade, vamos ampliar o uso da estrutura `if` e `else`, utilizando os operadores lógicos **E (`&&`)** e **OU (`||`)**.

### Para cada exercício:

**1. Identifique as entradas.**

**2. Identifique o processamento.**

**3. Identifique as condições.**

**4. Identifique as saídas.**

**5. Desenvolva o algoritmo.**

**6. Desenvolva o fluxograma.**

**7. Implemente a solução em C utilizando `if` e `else`.**

---

# 1. Operador E — `&&`

O operador **E** é utilizado quando **duas ou mais condições precisam ser verdadeiras ao mesmo tempo**.

Em C, utilizamos:

```c
&&
```

### Exemplo

Considere que um aluno será considerado aprovado quando:

- a média for maior ou igual a 7;
- **E**
- a frequência for maior ou igual a 75%.

As duas condições precisam ser verdadeiras.

```text
Média >= 7
       E
Frequência >= 75%
       ↓
   APROVADO
```

Se uma das condições for falsa, o aluno não será aprovado.

### Tabela de possibilidades

| Média >= 7 | Frequência >= 75% | Resultado |
|---|---|---|
| Verdadeiro | Verdadeiro | Aprovado |
| Verdadeiro | Falso | Reprovado |
| Falso | Verdadeiro | Reprovado |
| Falso | Falso | Reprovado |

### Código base

```c
#include <stdio.h>

int main() {

    float media;
    float frequencia;

    printf("Digite a media: ");
    scanf("%f", &media);

    printf("Digite a frequencia: ");
    scanf("%f", &frequencia);

    if () {
        printf("Aprovado!\n");
    } else {
        printf("Reprovado!\n");
    }

    return 0;
}
```

### Observe

Neste código:

```c
if (media >= 7 && frequencia >= 75)
```

temos **duas condições**:

```text
media >= 7
```

**E**

```text
frequencia >= 75
```

As duas precisam ser verdadeiras para entrar no `if`.

---

# 2. Operador OU — `||`

O operador **OU** é utilizado quando **pelo menos uma das condições precisa ser verdadeira**.

Em C, utilizamos:

```c
||
```

### Exemplo

Uma loja oferece frete grátis quando:

- a compra for maior ou igual a R$ 200;
- **OU**
- o cliente possuir um cupom de frete grátis.

Basta uma das condições ser verdadeira.

```text
Compra >= R$ 200
       OU
Possui cupom
       ↓
  Frete grátis
```

### Tabela de possibilidades

| Compra >= 200 | Possui cupom | Resultado |
|---|---|---|
| Verdadeiro | Verdadeiro | Frete grátis |
| Verdadeiro | Falso | Frete grátis |
| Falso | Verdadeiro | Frete grátis |
| Falso | Falso | Paga frete |

### Código base

```c
#include <stdio.h>

int main() {

    float valorCompra;
    int possuiCupom;

    printf("Digite o valor da compra: ");
    scanf("%f", &valorCompra);

    printf("Possui cupom? (1 = sim / 0 = nao): ");
    scanf("%d", &possuiCupom);

    if () {
        printf("Frete gratis!\n");
    } else {
        printf("Frete pago.\n");
    }

    return 0;
}
```

### Observe

Neste código:

```c
if (valorCompra >= 200 || possuiCupom == 1)
```

basta uma das condições ser verdadeira.

---

# 3. Comparando E e OU

## E — `&&`

Todas as condições precisam ser verdadeiras.

```c
if (condicao1 && condicao2)
```

Exemplo:

```c
if (idade >= 18 && possuiCNH == 1)
```

Significa:

```text
idade >= 18
     E
possui CNH
```

---

## OU — `||`

Pelo menos uma das condições precisa ser verdadeira.

```c
if (condicao1 || condicao2)
```

Exemplo:

```c
if (idade >= 18 || possuiAutorizacao == 1)
```

Significa:

```text
idade >= 18
     OU
possui autorização
```

---

# 4. Atividade 1 — Acesso a uma área restrita

Uma empresa possui uma área restrita que só pode ser acessada por funcionários que:

- tenham idade igual ou superior a 18 anos;
- **E**
- possuam um crachá válido.

Faça um programa que leia:

- idade do funcionário;
- informação se o crachá é válido.

Considere:

```text
1 = crachá válido
0 = crachá inválido
```

O programa deverá informar:

```text
ACESSO PERMITIDO
```

ou:

```text
ACESSO NEGADO
```

### Regra

```text
Idade >= 18
      E
Crachá válido
      ↓
ACESSO PERMITIDO

Caso contrário
      ↓
ACESSO NEGADO
```

### Para desenvolver

**1. Identifique as entradas.**

**2. Identifique o processamento.**

**3. Identifique a condição.**

**4. Identifique as saídas.**

**5. Desenvolva o algoritmo.**

**6. Desenvolva o fluxograma.**

**7. Implemente a solução em C utilizando `if`, `else` e `&&`.**

---

# 5. Atividade 2 — Entrada no evento

Um evento permite a entrada de uma pessoa quando ela:

- possui um ingresso válido;
- **OU**
- possui uma autorização especial da organização.

Faça um programa que leia:

- se possui ingresso válido;
- se possui autorização especial.

Considere:

```text
1 = sim
0 = não
```

O programa deverá informar:

```text
ENTRADA PERMITIDA
```

ou:

```text
ENTRADA NEGADA
```

### Regra

```text
Ingresso válido
      OU
Autorização especial
      ↓
ENTRADA PERMITIDA

Caso contrário
      ↓
ENTRADA NEGADA
```

### Para desenvolver

**1. Identifique as entradas.**

**2. Identifique o processamento.**

**3. Identifique a condição.**

**4. Identifique as saídas.**

**5. Desenvolva o algoritmo.**

**6. Desenvolva o fluxograma.**

**7. Implemente a solução em C utilizando `if`, `else` e `||`.**

---

# Objetivo

Compreender como utilizar operadores lógicos junto às estruturas de decisão.

```text
Condição simples
      ↓
    IF/ELSE
      ↓
Múltiplas condições
      ↓
   && / ||
      ↓
   IF/ELSE
```

## Conceitos trabalhados

- Variáveis
- Entrada de dados
- Saída de dados
- Operadores de comparação
- Operador lógico E (`&&`)
- Operador lógico OU (`||`)
- Estruturas de decisão
- `if`
- `else`
- Algoritmos
- Fluxogramas
- Implementação em C
- Combinação de condições
