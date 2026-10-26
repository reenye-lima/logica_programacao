# Exercícios de C — IF e ELSE (Aplicações em Mecatrônica)

## Orientações

**Para cada exercício proposto:**

1. **Identifique as entradas** (sensores, dados lidos, etc.).
2. **Identifique o processamento** (cálculos ou conversões necessárias).
3. **Identifique a condição** (regra de decisão lógica).
4. **Identifique as saídas** (atuadores, mensagens de alerta, displays).
5. **Desenvolva o algoritmo** em pseudocódigo / português estruturado.
6. **Desenvolva o fluxograma** (representação gráfica da solução).
7. **Implemente a solução em C** utilizando as estruturas `if` e `else`.

---

## 1. Monitoramento de Pressão Pneumática

Em uma linha de montagem automatizada, um sensor analógico lê a pressão de um cilindro pneumático em bar. Para evitar falhas de atuadores e travamento de peças, a pressão ideal de trabalho do sistema deve ser de **no mínimo 5.0 bar**.

Faça um programa que leia a pressão atual do sistema e exiba a mensagem **SISTEMA OPERACIONAL** caso a pressão seja suficiente, ou **PRESSAO INSUFICIENTE - LIGAR COMPRESSOR** caso esteja abaixo do limite mínimo.

### Exemplo 1

```text
Digite a pressao do sistema (bar): 6.2

SISTEMA OPERACIONAL
```

### Exemplo 2

```text
Digite a pressao do sistema (bar): 4.1

PRESSAO INSUFICIENTE - LIGAR COMPRESSOR
```

### Regra

```text
Pressao >= 5.0 bar
        ↓
SISTEMA OPERACIONAL

Pressao < 5.0 bar
        ↓
PRESSAO INSUFICIENTE - LIGAR COMPRESSOR
```

---

## 2. Controle de Frequência do Inversor de Frequência

Um inversor de frequência controla a velocidade de rotação de um motor trifásico acoplado a uma esteira transportadora. O motor possui um limite máximo de segurança operacional de **60.0 Hz**.

Faça um programa que leia a frequência enviada ao motor. Se a frequência informada for estritamente **maior que 60.0 Hz**, o programa deve aplicar um fator de correção/corte de **10.0 Hz** por segurança e exibir a nova frequência ajustada. Caso contrário, deve apenas exibir a frequência normal mantida.

### Exemplo 1

```text
Digite a frequencia do motor (Hz): 68.5

ALERTA: SOBREFREQUENCIA!
Frequencia ajustada para: 58.5 Hz
```

### Exemplo 2

```text
Digite a frequencia do motor (Hz): 45.0

Frequencia normal: 45.0 Hz
```

### Fórmulas

```text
frequenciaAjustada = frequencia - 10
```

### Regra

```text
Frequencia > 60.0 Hz
        ↓
Aplicar redução de 10 Hz

Frequencia <= 60.0 Hz
        ↓
Manter frequencia original
```

---

## 3. Verificação de Alinhamento do Braço Robótico

Um braço robótico industrial possui um encoder absoluto responsável por medir o ângulo de acionamento da sua junta principal. Para realizar o pino de trava (posição de descanso/home), a junta deve estar calibrada exatamente no ângulo neutro de **90 graus**.

Faça um programa que leia o ângulo atual retornado pelo encoder e informe **POSICAO DE TRAVA OK** se o ângulo for exatamente igual a 90°, ou **NECESSITA RECALIBRACAO** se houver qualquer desvio em relação ao ponto ideal.

### Exemplo 1

```text
Digite o angulo lido (graus): 90

POSICAO DE TRAVA OK
```

### Exemplo 2

```text
Digite o angulo lido (graus): 93

NECESSITA RECALIBRACAO
```

### Regra

```text
Angulo == 90
      ↓
POSICAO DE TRAVA OK

Angulo != 90
      ↓
NECESSITA RECALIBRACAO
```

---

## Objetivo da Atividade

Praticar a transformação de um problema de engenharia/automação na seguinte sequência de resolução:

```text
Problema Prático
       ↓
 Algoritmo/Lógica
       ↓
    Fluxograma
       ↓
   Código em C
```

### Conceitos Trabalhados

- Leitura de dados de processo (pressão, frequência, ângulo)
- Variáveis de ponto flutuante (`float`) e inteiros (`int`)
- Operadores relacionais (`>=`, `>`, `==`, `!=`)
- Tomada de decisão com `if` e `else`
- Lógica de segurança e controle industrial
- Modelagem através de fluxogramas

---

### [Formulário de envio](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=SxwFsZQ7q0GUQec6cjQv3UH_JtxNK51Ktr8saWcaWU9UODdFQ1JEMlNPMTFUMDRMQjMxM0hUSlBaVC4u)
