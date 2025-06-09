---
Title: Composição de Funções
Date: 2025-06-07
Time: 22:25:00
related:
  - "[[Função]]"
  - "[[Função Inversa]]"
  - "[[Função Injetora]]"
  - "[[Função Sobrejetora]]"
  - "[[Função Bijetora]]"
  - "[[Gráfico de Função]]"
  - "[[Domínio e Contradomínio]]"
  - "[[Imagem de Função]]"
---

A **composição de funções** é uma operação que aplica uma função a outra.

## Definição

Sejam $f: A \to B$ e $g: B \to C$. A composição $g \circ f$ é a função de $A$ em $C$ definida por:
$$
(g \circ f)(x) = g(f(x))
$$

## Características

- A ordem importa: geralmente, $g \circ f \ne f \circ g$.
- O domínio de $g \circ f$ é o conjunto de todos os $x \in A$ para os quais $f(x) \in B$ e $g(f(x))$ está definido.
- A composição é associativa:
  - $(h \circ (g \circ f)) = ((h \circ g) \circ f)$

## Exemplo

Se $f(x) = 2x$ e $g(x) = x + 1$, então:
- $(g \circ f)(x) = g(f(x)) = 2x + 1$
- $(f \circ g)(x) = f(g(x)) = 2(x + 1) = 2x + 2$

## Observações

- A composição é fundamental para construir funções mais complexas.
- Importante em transformações geométricas e mudanças de variáveis.
