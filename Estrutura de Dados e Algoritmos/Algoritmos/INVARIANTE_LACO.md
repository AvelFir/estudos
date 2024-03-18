# Invariante de laço

- Parecida com a induçao matematica, quando queremos mostrar algo por induçao queremos mostrar que uma propriedade é valida.

- A invariante de laço, também conhecida como "invariant loop condition" em inglês, é uma expressão lógica que é verdadeira toda vez que o controle do programa alcança o ponto em que é verificada dentro de um laço (loop). Em outras palavras, é uma propriedade que se mantém constante durante a execução de um laço.

- A importância das invariantes de laço reside no fato de que elas ajudam os programadores a entender e a verificar a correção do código que contém laços. Uma invariante de laço eficaz ajuda a garantir que o laço termine corretamente e produza os resultados esperados.

Por exemplo, considere o seguinte laço em pseudocódigo:

```
x = 0
enquanto x < 10 faça
    x = x + 1
``` 
- Uma invariante de laço para este exemplo poderia ser "x é sempre menor que 10". Isso é verdadeiro toda vez que o controle do programa verifica a condição do laço, garantindo que o laço terminará quando x atingir ou exceder 10, conforme esperado.

- As invariantes de laço são úteis em várias áreas da ciência da computação, incluindo análise de algoritmos, verificação de programas e otimização de código. Elas ajudam a garantir a correção do código e podem ser usadas para demonstrar a correção de algoritmos ou identificar possíveis erros durante o desenvolvimento do software.

Com a invariante mostramos  2 coisas e obtem-se 1 de graça

```
Propriedade P em que mostramos: 
Inicio: P vale antes da primeira interaçao do laço
Manutençao: se P vale antes de uma iteraçao, entao P continua verdadeiro na proxima iteraçao
Termino: quando o laço termina, o que a invariante nos diz sobre o algoritmo. 
```

```
int n = 10;
int soma = 0;
for(i=1;i<=n;i++){
    soma +=i;
}
print(soma);

Propriedade: a variavel soma sempre resultara em um numero inteiro positivo
Inicializaçao: soma é um inteiro positivo
Execuçao: soma continua sendo um inteiro positivo
Termino: soma continua sendo um inteiro positivo
```