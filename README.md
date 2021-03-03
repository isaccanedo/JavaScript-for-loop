# JavaScript-for-loop
:star2: # JavaScript for Loop

### Introdução ao JavaScript para instrução de loop

A instrução de loop for JavaScript permite que você crie um loop com três expressões opcionais. O seguinte ilustra a sintaxe da instrução for loop:

```
for (initialization; condition; post-expression) {
    // statements
}
```

### 1) inicialização
A expressão de inicialização inicializa o loop. A expressão de inicialização é executada apenas uma vez quando o loop começa. Normalmente, você usa a inicialização para inicializar uma variável de contador. Se você usar a palavra-chave var para declarar a variável do contador, a variável terá uma função ou escopo global. Em outras palavras, você pode fazer referência à variável do contador após o término do loop. No entanto, se você usar a palavra-chave let para declarar a variável do contador, a variável terá um escopo bloqueado, que só pode ser acessado dentro do loop.

### 2) condição
A condição é uma expressão avaliada uma vez antes de cada iteração. A instrução dentro do loop é executada apenas quando a condição é avaliada como verdadeira. O loop é encerrado se a condição for avaliada como falsa. Observe que a condição é opcional. Se você omiti-lo, a instrução for loop o considera verdadeiro.

### 3) pós-expressão
A instrução for loop também avalia a pós-expressão após cada iteração do loop. Geralmente, você usa a pós-expressão para atualizar a variável do contador. O fluxograma a seguir ilustra o loop for:

<img src="https://github.com/isaccanedo/JavaScript-for-loop/blob/main/JavaScript-for-Loop.png">
    
 No loop for, as três expressões são opcionais. O seguinte mostra como usar o loop for sem quaisquer expressões:
 
 ```
 for ( ; ; ) {
   // statements
}
 ```
 
### JavaScript para exemplos de loop

Vamos dar alguns exemplos de uso do loop for.

1) Simples para exemplos de loop
O exemplo a seguir usa a instrução de loop for que mostra os números de 1 a 5 na janela do console.
 
 ```
 for (var counter = 1; counter < 5; counter++) {
    console.log('Inside the loop:' + counter);
}
console.log('Outside the loop:' + counter);
 ```
 
 Saída:
 
 ```
Dentro do loop: 1
Dentro do loop: 2
Dentro do loop: 3
Dentro do loop: 4
Fora do loop  : 5
 ```
 
 ### Como funciona.

- Primeiro, declare um contador de variável e inicialize-o como 1.
- Em segundo lugar, exiba o valor do contador na janela do console se o contador for menor que 5.
- Terceiro, aumente o valor do contador em um em cada iteração do loop.

Como o loop for usa a palavra-chave var para declarar counter, o escopo de counter é global. Portanto, podemos acessar a variável do contador após o término do loop. No ES6, você pode usar a palavra-chave let para declarar a variável do contador que é local para o loop:

```
for (let counter = 1; counter < 5; counter++) {
    console.log('Inside the loop:' + counter);
}
console.log('Outside the loop:' + counter);
```
Erro:

```
ReferenceError: counter is not defined
```

Acessar a variável do contador após o loop causou um ReferenceError.

### 2) O loop for sem o exemplo da parte de inicialização
O exemplo a seguir usa um loop for que omite a parte de inicialização:

```
var j = 1;
for (; j < 10; j += 2) {
    console.log(j);
}
```
Saída:

```
1
3
5
7
9
```

### 3) O loop for sem o exemplo de condição
Semelhante à expressão de inicialização, a expressão de condição é opcional. Se você omitir a expressão de condição, precisará usar uma instrução break para encerrar o loop.

```
for (let j = 1;; j += 2) {
    console.log(j);
    if (j > 10) {
        break;
    }
}
```
Saída:

```
1
3
5
7
9
11
```
### 3) O loop for sem nenhum exemplo de expressão
Todas as três expressões das instruções de loop for são opcionais, portanto, você pode omitir todas elas. Novamente, você deve usar uma instrução break para encerrar o loop e também modificar a variável do contador para fazer com que a condição para a instrução break se torne verdadeira em algum ponto.

```
// initialize j variable
let j = 1;
for (;;) {
    // terminate the loop if j is greater than 10;
    if (j > 10) break;
    console.log(j);
    // increase the counter j
    j += 2;
}
```
Saída:

```
1
3
5
7
9
```
### 4) O loop for sem o exemplo do corpo do loop
Curiosamente, a instrução for pode ter uma instrução vazia. Nesse caso, você coloca um ponto-e-vírgula (;) imediatamente após a instrução for. O exemplo a seguir calcula o total de números de 1 a 10.

A expressão é colocada na pós-expressão, portanto, ela usa uma instrução vazia no corpo do loop.

```
let sum = 0;
for (let i = 0; i <= 9; i++, sum += i);
console.log(sum);
```
Saída:

```
55
```

Neste tutorial, você aprendeu como usar a instrução de loop for JavaScript para criar um loop com várias opções.

