# Arrays

![Arrays](./imgs/array.png)

## Caracteristicas
- Um Array tambem conhecido como vetor, é uma estrutura de dados que armazena uma coleçao ordenada de elementos do mesmo tipo.
- Cada ele elemento é acessado atraves de um indice que deve ser um numero inteiro, que representa sua posiçao no array.
- Os indices geralmente começam de 0 e vão ate até o tamanho do array -1.
- Para manipulaçao de determinado elemento em um vetor, precisamos fornecer seu identificador e o indice do elemento desejado
- Sua indexaçao permite acesso a qualquer elemento, em qualquer instante e em qualquer ordem, sem que a sua posiçao no vetor imponha qualquer custo extra de eficiencia.
## Declaraçao de um Vetor
Um vetor é declarado da seguinte maneira:

1. **Nome**: um identificador valido da linguagem
2. **Tipo**: que determina os dados do elementos do vetor
3. **Tamanho**: que delimita quantos elementos pode armazenar
- utilizam-se colchetes na declaraçao e identificaçao de um elemento do vetor.

Exemplos

### **Pseudocodigo:**

v : vetor [0..N] de inteiros

### **Java:**

< tipo>[]< identificador> = new <tipo> [n] 

ou

< tipo> < identificador>[] = new <tipo> [n] 

ou

< tipo> < identificador>[] = {1,2,3,4}

- Nas variaveis declaradas como primitivos sao guardados dados correspondentes ao tipo
- Nos objetos sao guardadas apenas as referencias aos dados.
- Vetores em java sao objetos e, portanto seus indices representam referencias aos objetos construidos pelo operador new, nao aos valores em si.


## Acesso e Atribuiçao de valor ao vetor
### Atribuiçao de valor
Para atribuir valor a um vetor devemos referenciar o index que queremos atribuir valor seguido do valor que deve ser do mesmo tipo do vetor.

**String[] semana = new String[7];**

**semana[0] = "Domingo";**

**semana[1] = "Segunda";**

**semana[2] = "Terça";**

### Acesso ao valor
A leitura, ou o acesso aos valores dos elementos de um vetor, é semelhante a atribuiçao utilizando o index dele para referenciar o dado

**System.out.println("A semana se inicia no " + semana[0])**
