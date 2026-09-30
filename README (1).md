# Lógica Proposicional: Representação e Tabelas-Verdade

Exercícios de lógica proposicional: tradução de frases em linguagem natural para a forma lógica, usando os conectivos apropriados, e construção das tabelas-verdade com todas as combinações de valores **V** (verdadeiro) e **F** (falso).

## Conectivos utilizados

| Símbolo | Nome | Leitura | Quando é verdadeira |
|---------|------|---------|---------------------|
| ∧ | Conjunção | P **e** Q | Somente quando P e Q são ambas V |
| ∨ | Disjunção (inclusiva) | P **ou** Q | Quando pelo menos uma é V |
| → | Condicional | **Se** P, **então** Q | Falsa somente quando P é V e Q é F |
| ↔ | Bicondicional | P **se e somente se** Q | Quando P e Q têm o mesmo valor lógico |

## Índice

1. [Estudei e fiz os exercícios](#1-eu-estudei-para-a-prova-e-fiz-todos-os-exercícios)
2. [Cinema ou séries](#2-eu-vou-ao-cinema-ou-fico-em-casa-assistindo-séries)
3. [Acordar cedo → ônibus](#3-se-eu-acordar-cedo-então-conseguirei-pegar-o-ônibus)
4. [Estudar muito → passar e ganhar presente](#4-se-eu-estudar-muito-então-passarei-na-prova-e-ganharei-um-presente)
5. [Videogame ou lógica de programação](#5-eu-vou-jogar-videogame-ou-vou-estudar-lógica-de-programação)
6. [Pizza e refrigerante](#6-eu-comi-pizza-e-tomei-refrigerante)
7. [Dinheiro → viagem](#7-se-eu-tiver-dinheiro-então-viajarei-nas-férias)
8. [Livro ↔ trabalho](#8-eu-lerei-um-livro-se-e-somente-se-terminar-meu-trabalho)
9. [Sol → praia ou parque](#9-se-estiver-sol-então-irei-à-praia-ou-ao-parque)
10. [Bolo ↔ ingredientes](#10-eu-farei-um-bolo-se-e-somente-se-comprar-os-ingredientes)
- [Resumo](#resumo)

---

## 1. "Eu estudei para a prova e fiz todos os exercícios."

- **P**: Eu estudei para a prova.
- **Q**: Eu fiz todos os exercícios.
- **Forma lógica:** `P ∧ Q`

| P | Q | P ∧ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **F** |
| F | F | **F** |

---

## 2. "Eu vou ao cinema ou fico em casa assistindo séries."

- **P**: Eu vou ao cinema.
- **Q**: Eu fico em casa assistindo séries.
- **Forma lógica:** `P ∨ Q`

| P | Q | P ∨ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **V** |
| F | V | **V** |
| F | F | **F** |

> **Observação:** foi usado o "ou" inclusivo. Se a intenção fosse "ou um, ou outro" (exclusivo, `P ⊻ Q`), a primeira linha seria F.

---

## 3. "Se eu acordar cedo, então conseguirei pegar o ônibus."

- **P**: Eu acordo cedo.
- **Q**: Eu consigo pegar o ônibus.
- **Forma lógica:** `P → Q`

| P | Q | P → Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **V** |
| F | F | **V** |

---

## 4. "Se eu estudar muito, então passarei na prova e ganharei um presente."

- **P**: Eu estudo muito.
- **Q**: Eu passo na prova.
- **R**: Eu ganho um presente.
- **Forma lógica:** `P → (Q ∧ R)`

| P | Q | R | Q ∧ R | P → (Q ∧ R) |
|---|---|---|-------|-------------|
| V | V | V | V | **V** |
| V | V | F | F | **F** |
| V | F | V | F | **F** |
| V | F | F | F | **F** |
| F | V | V | V | **V** |
| F | V | F | F | **V** |
| F | F | V | F | **V** |
| F | F | F | F | **V** |

---

## 5. "Eu vou jogar videogame ou vou estudar lógica de programação."

- **P**: Eu vou jogar videogame.
- **Q**: Eu vou estudar lógica de programação.
- **Forma lógica:** `P ∨ Q`

| P | Q | P ∨ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **V** |
| F | V | **V** |
| F | F | **F** |

---

## 6. "Eu comi pizza e tomei refrigerante."

- **P**: Eu comi pizza.
- **Q**: Eu tomei refrigerante.
- **Forma lógica:** `P ∧ Q`

| P | Q | P ∧ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **F** |
| F | F | **F** |

---

## 7. "Se eu tiver dinheiro, então viajarei nas férias."

- **P**: Eu tenho dinheiro.
- **Q**: Eu viajo nas férias.
- **Forma lógica:** `P → Q`

| P | Q | P → Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **V** |
| F | F | **V** |

---

## 8. "Eu lerei um livro se e somente se terminar meu trabalho."

- **P**: Eu leio um livro.
- **Q**: Eu termino meu trabalho.
- **Forma lógica:** `P ↔ Q`

| P | Q | P ↔ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **F** |
| F | F | **V** |

---

## 9. "Se estiver sol, então irei à praia ou ao parque."

- **P**: Está sol.
- **Q**: Eu vou à praia.
- **R**: Eu vou ao parque.
- **Forma lógica:** `P → (Q ∨ R)`

| P | Q | R | Q ∨ R | P → (Q ∨ R) |
|---|---|---|-------|-------------|
| V | V | V | V | **V** |
| V | V | F | V | **V** |
| V | F | V | V | **V** |
| V | F | F | F | **F** |
| F | V | V | V | **V** |
| F | V | F | V | **V** |
| F | F | V | V | **V** |
| F | F | F | F | **V** |

---

## 10. "Eu farei um bolo se e somente se comprar os ingredientes."

- **P**: Eu faço um bolo.
- **Q**: Eu compro os ingredientes.
- **Forma lógica:** `P ↔ Q`

| P | Q | P ↔ Q |
|---|---|-------|
| V | V | **V** |
| V | F | **F** |
| F | V | **F** |
| F | F | **V** |

---

## Resumo

| Nº | Forma lógica | Tipo | Nº de linhas |
|----|--------------|------|--------------|
| 1 | `P ∧ Q` | Conjunção | 4 |
| 2 | `P ∨ Q` | Disjunção | 4 |
| 3 | `P → Q` | Condicional | 4 |
| 4 | `P → (Q ∧ R)` | Condicional com conjunção | 8 |
| 5 | `P ∨ Q` | Disjunção | 4 |
| 6 | `P ∧ Q` | Conjunção | 4 |
| 7 | `P → Q` | Condicional | 4 |
| 8 | `P ↔ Q` | Bicondicional | 4 |
| 9 | `P → (Q ∨ R)` | Condicional com disjunção | 8 |
| 10 | `P ↔ Q` | Bicondicional | 4 |

> O número de linhas de cada tabela é `2^n`, onde `n` é a quantidade de proposições simples (2 proposições → 4 linhas; 3 proposições → 8 linhas).
