# Matriz

![Matriz](./imgs/matriz.png)

## Caracteristicas
- Tambem chamadas de matrizes de dimensao n, onde n sao o numero de indexes requeridos.
- A maioria das linguagens nao impoe um limite de tamanho, ficando a cargo do programador definir quanto ele necessita.

## Declaraçao

A declaraçao de uma matriz é similar ao Array, pois um array é uma matriz de dimensao 1
1. Nome
2. Tipo
3. Entre colchetes definimos o tamanho de cada dimensao
4. Usualmente, em uma matriz bidimensional o primeiro index indica a linha e o segundo a coluna

### Pseudocodigo:
Matriz : vetor [1...n,1...n] de inteiros

### Java:
Em java nao possuimos Matriz por padrao, o que se obtem é um array de arrays declarado da seguinte forma:

int[][] matriz = new int[n][n];

## Acesso e Atribuiçao de valor

### Atribuiçao de valor
Para a atribuiçao de valor devemos especificar n indexes, sendo n o numero de dimensoes.
Ex:
matriz[0][0] = 1; 
matriz[0][1] = 2; 

### Acesso ao valor
Para a acessar um valor devemos especificar n indexes, sendo n o numero de dimensoes.
Ex:
System.out.println("O numero da primeira linha e da primeira coluna é : " + matriz[0][0]);


## Eficiência e Complexidade

A eficiência e complexidade de uma matriz seguem princípios semelhantes aos de um array, mas com algumas considerações adicionais devido à sua natureza bidimensional. Aqui estão alguns pontos importantes sobre a eficiência e a complexidade de operações comuns em matrizes:

### Acesso (leitura/gravação) de elementos:
- Eficiência: O acesso a um elemento específico de uma matriz também é geralmente eficiente, pois envolve o cálculo do deslocamento com base nas coordenadas da linha e da coluna.
- Complexidade: O acesso a um elemento de uma matriz tem complexidade O(1), desde que as dimensões da matriz sejam conhecidas e fixas.

### Inserção/Remoção de elementos:
- Eficiência: Inserir ou remover elementos no final de uma linha ou coluna de uma matriz é geralmente eficiente, desde que haja espaço livre disponível.
- Complexidade: Inserir/remover no final de uma linha ou coluna tem complexidade O(1). No entanto, inserções/remoções no meio da matriz ou em posições arbitrárias podem ter complexidade O(n^2), pois podem exigir o deslocamento de muitos elementos.

### Pesquisa (ou busca) linear:
- Eficiência: A pesquisa linear em uma matriz envolve percorrer cada elemento, linha por linha ou coluna por coluna.
- Complexidade: A pesquisa linear em uma matriz de tamanho m x n tem complexidade O(m * n), pois pode ser necessário percorrer todas as linhas e colunas até encontrar o elemento desejado ou determinar que ele não está presente.

### Ordenação:
- Eficiência: A ordenação de uma matriz geralmente envolve a ordenação de cada linha ou coluna separadamente.
- Complexidade: A complexidade da ordenação de uma matriz depende do algoritmo de ordenação utilizado. Se uma matriz for considerada como uma lista de linhas ou colunas, a ordenação terá complexidade O(m * n * log(m * n)), onde m é o número de linhas e n é o número de colunas.

### Operações matriciais:
- Eficiência: Operações matriciais comuns, como multiplicação de matriz, transposição, determinante, entre outras, podem ter eficiência variada dependendo do algoritmo e das características das matrizes envolvidas.
- Complexidade: A complexidade dessas operações pode variar amplamente dependendo da operação específica e do algoritmo utilizado. Por exemplo, a multiplicação de matriz tem complexidade O(m * n * p), onde m, n e p são as dimensões das matrizes envolvidas.

**Em resumo, as operações em uma matriz podem ter complexidades diferentes dependendo da operação específica e das características da matriz. É importante considerar esses fatores ao projetar e implementar algoritmos que envolvam o uso de matrizes para garantir um desempenho adequado.**