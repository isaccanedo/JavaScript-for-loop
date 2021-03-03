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

<src img = "JavaScript-for-Loop">
    
 No loop for, as três expressões são opcionais. O seguinte mostra como usar o loop for sem quaisquer expressões:
 
 ```
 for ( ; ; ) {
   // statements
}
 ```
 
 
