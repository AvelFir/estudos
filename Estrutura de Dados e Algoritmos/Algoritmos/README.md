 # Algoritmos
 - O objetivo de aprender Algoritmos é escrever codigos **corretos** e **eficientes**
## O que é um algoritmo
- Um algoritmo é um conjunto de operaçoes computacionais bem definidas que podem receber um conjunto de valores de entradas e produzir um conjunto de valores de saida.
- Um algoritmo é uma ferramenta para resolver um problema computacional

## Problema Computacional
- Um problema computacional é um problema que especifica uma relaçao entre uma entrada e uma saida.

### Problema de Ordenaçao

**Entrada:** uma sequencia de n numeros a1,a2,...an.

**Saida:** uma permutaçao a1,a2,...an da entrada tal que a1 e a2 <= ... <= an.

Exemplo:

**Entrada:** 31,42,59,26,42,58

**Um algoritmo de ordenaçao deve produzir:**

**Saida:** 26,31,42,42,58,59
- Uma entrada especifica é chamada de uma **instancia do problema**.
- Um algortimo é **correto** se ele fornece a saida correta para toda entrada possivel do problema.
- Um algoritmo correto **resolve** um problema computacional


## Eficiencia

### Algoritmos para ordenar n valores
ops = operaçoes
- Insertion Sort: 2n² ops = 2 * n * n
- Merge Sort: 50nlogn ops = 2 * n * 25logn

#### Qual algoritmo é melhor?

##### n de operaçoes aproximados

| n    | Insertion Sort | Merge Sort  |    
|------|----------------|-------------|
| 1    | 2              | 0           |
| 10   | 200            | 1500        |
| 100  | 20.000         | 33.200      |
| 10^3 | 2.000.000      | 500.000     |
| 10^6 | 2 * 10^12      | 10^9        |
| 10^9 | 2 * 10^18      | 1,5 * 10^12 |


- Computador A: 10 bilhoes ops/s
- Computador B: 10 milhoes ops/s

##### Tempo
Tempo = n_ops / n_ops_s

| n    | Insertion Sort A | Insertion Sort B | Merge Sort A | Merge Sort B |    
|------|------------------|------------------|--------------|--------------|
| 1    | < 1s             | < 1s             | < 1s         | < 1s         |
| 10   | < 1s             | < 1s             | < 1s         | < 1s         |
| 100  | < 1s             | < 1s             | < 1s         | < 1s         |
| 10^3 | < 1s             | < 1s             | < 1s         | < 1s         |
| 10^6 | 3,3m             | 2,3 dias         | < 1s         | 1,6m         |
| 10^9 | 6,3 anos         | 6300 anos        | 2,5m         | 1,7 dias     |


- Em questao de numero de operaçoes, para valores pequenos o insertion é melhor, porem para valores grandes a funçao logn cresce muito mais lentamente.
- Em questao de tempo, valores pequenos tem o mesmo processamento nos dois algoritmos quando se trata de valores pequenos nao importa qual dos dois usar, no fundo oque importa é quando a entrada é grande, dessa forma usa-se valores grandes para analisar eficiencia de algoritmos.
- Algoritmos tambem sao tecnologia, independente de um computador mais rapido, um algoritmo melhor se sai muito melhor em um computador ruim do que um algoritmo ruim em um computador muito bom.


