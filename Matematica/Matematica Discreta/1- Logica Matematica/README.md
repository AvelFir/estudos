

# Logica Matematica

## 1. Logica proposicional

### 1.1 Proposiçoes e valores logicos

Uma proposiçao é uma sentença declarativa que ou é verdadeira ou é falsa:

- O morcego é um mamifero
- Rio de janeiro é a captal do Brasil

Independente de ser verdadeira ou falsa

Uma sentença declarativa que depende de variaveis pode ser considerada uma proposiçao em um contexto onde as variaveis tem valor determinado:
"X é menor que 3" isoladamente nao é uma proposiçao. porem uma vez que o valor de x for definido ela se torna uma proposiçao.

O valor logico ou valor-verdade de uma proposiçao é verdadeiro se ela for verdadeira, e falso caso contrario.

### 1.2 Conectivos logicos e proposiçoes compostas
Todas as linguas possuem conectivos logicos como "e","ou","nao","se... entao".
Proposiçoes compostas sao aquelas que possuem duas proposiçoes simples(atomicas) ligadas por um conectivo logico.

* A e B
* A ou B
* se A entao B
* nao A

O valor logico de proposiçoes compostas depende dos valor logico das proposiçoes simples que a compoem e da maneira que estao ligadas pelo conectivo.

### 1.3 Notaçao para calculo proposicional

A logica proposicional ou calculo proposicional é um formalismo que permite determinar o valor logico de proposiçoes compostas.
Para eliminar a fonte de confusao da liguagem natural, traduzimos as proposiçoes para notaçao algebrica

* proposiçoes represantadas por letras minusculas (p,q,r,...)
* essas letras podem ter apenas dois valores possiveis V e F
* Os conectivos logicos sao reposentados por sinais algebricos (operadores):
  * conjunçao: p ^ q, siginificando "p e q"
  * disjunçao: p V q, siginificando "p ou q"
  * negaçao: ¬p, siginificando "nao p"
  * implicaçao: p -> q, siginificando "se p, entao q"
  * equivalencia: p <--> q, siginificando "p se, e somente se, q"
  * disjunçao exclusiva: p ⊕ q, significa ou p ou q, nao ambos.


### 1.4 Operador de Conjunçao

Por definiçao o valor logico de p ^ q é verdadeiro se p e q sao ambos verdadeiros. Se qualquer uma das duas posiçoes for false, ou ambas, entao p ^ q é falso

#### Tabela Verdade:

| p | q | p^q |
|---|---|-----|
| V | V | V   |
| V | F | F   |
| F | V | F   |
| F | F | F   |


### 1.5 Operador de Disjunçao
Por definiçao o valor logico de p V q é verdadeiro se pelo pelo menos uma das proposiçoes for verdadeira, se ambas forem falsas entao p V q sera falso tambem.

#### Tabela Verdade:
| p | q | pVq |
|---|---|-----|
| V | V | V   |
| V | F | V   |
| F | V | V   |
| F | F | F   |

Este conectivo tambem é chamado de ou inclusivo pois permite que as duas proposiçoes sejam verdadeiras.

### 1.6 Operador de Negaçao

A partir de uma proposiçao p, podemos formas uma nova proposiçao com o valor logico oposto ao de p. Essa nova proposiçao chamada de negaçao de p e denotada por ¬p.

#### Tabela Verdade:
| p | ¬p |
|---|----|
| V | F  |
| F | V  |

### 1.7 Operador de Implicaçao
A proposiçao "se p entao q", denotada por p -> q, é chamada de implicaçao ou condicional. O valor logico de p->q é falso apenas se p for verdadeiro e q for falso. Nos demais casos, o valor de p->q é verdadeiro.

#### Tabela Verdade:
| p | q | p->q |
|---|---|------|
| V | V | V    |
| V | F | F    |
| F | V | V    |
| F | F | V    |

Note que em logica esse conectivo nao pressupoe uma relaçao causal entre p e q. Por exemplo a sentença "se 2 é par entao Brasilia é a capital do Brasil" é verdadeira pois ambas as proposiçoes sao verdadeiras, apesar de nao haver nenhuma relaçao conhecida entre os dois fatos.

Sempre que a hipotese (p) é verdadeira entao a tese tambem é verdadeira (q)

A implicaçao q -> p é a reciproca(a volta) de p -> q. Ha casos em que p -> q é verdadeira, mas sua reciproca q->p é falsa; e vice versa.

A proposiçao (!p) -> (!q) é chamada de inversa de p -> q. Ha casos em que p->q é verdadeira, mas sua inversao é falsa; e vice versa

A proposiçao (!q) -> (!p) é a contrapositiva de p->q, quaisquer sque sejam os valores logicos de p e de q.

Proposição recíproca de p —> q    :    q —> p

Proposição inversa de  p —> q    :    ~p —> ~q

Proposição contrapositiva de p —> q    :    ~q —> ~p

Exemplos:
* A contrapositiva de !p -> q = !q -> !!p = !q -> p
* A reciproca de !q -> p = p -> !q
* A inversa da reciproca de q -> !p = (reciproca) !p -> q = (inversa) !!p -> !q = p -> !q 
* A negaçao de p -> !q = !p -> !!q = !p -> q
* A reciproca de !p V q = q V !p

Observaçao
p -> q - p condicional q, proposiçao logica, pode ser verdadeiro ou falso
p => q - p implica q, estamos afirmando que o valor logico é verdadeiro

### 1.8 Operador de Equivalencia
A proposiçao p se, e somente se, q é chamada de equivalencia ou bicondicional de p e q. Ela é denotada por p <-> q. O valor logico de p <-> q é verdadeiro quando p e q tem o mesmo valor logico, e falso caso o contrario

#### Tabela Verdade:
| p | q | p<->q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | V     |


Observaçao
p <-> q o bicondicional é uma proposicao logica com valor condicional, pode ser verdadeira ou falsa
p <=> q o bicondicional é uma proposicao verdadeira

### 1.9 Operador de Disjunçao Exlusiva

Denotados por p ⊕ q a proposiçao "ou p ou q, mas nao ambos". Esteconectivo é chamado de disjunçao exclusiva de p e q. O valor logico de p ⊕ q é verdadeiro se p e q tem valores logicos opostos, ou seja, exatamente um deles é verdadeiro.

#### Tabela Verdade:
| p | q | p<->q |
|---|---|-------|
| V | V | F     |
| V | F | V     |
| F | V | V     |
| F | F | F     |

### 1.10 Precedencia dos operadores logicos

Em uma proposiçao que usa dois ou mais operadores devem ser aplicados na seguinte ordem ou utilziar parenteses para separa-las.
! = 1
^ = 2
V,⊕ = 3
->,<-> = 4

Assim por exemplo a proposiçao !p ^q -> r ⊕ s ^ v, deve ser entendida como ((!p)^q)->(r⊕(s^v))

Assim como na algebra, deve ser lido da esquerda para a direita.

## 2. Afirmaçoes auto-referentes
 Afirmaçoes que referem a si mesmas, como "esta sentença é falsa", nao sao proposiçoes logicas.
 Tais afirmaçoes, relacaionadas com o paradoxo do Barbeiro, sempre foram um problema para a logica matematica, que nao tem maneiras satisfatorias de lidar comelas.
 Esse problema surge quando ha varias afirmaçoes que se referenciam entre si. Por exemplo a frase "A sentença seguinte é falsa, e a sentença anterior é verdadeira", embora possa ser analisada como uma conjunçao p^q, nao é uma afirmaçao logica porque p é uma afirmaçao sobre q e vice-versa.
 
## 3. Manipulaçao Logica de proposiçoes

### 3.1 Tautologias e contradiçoes