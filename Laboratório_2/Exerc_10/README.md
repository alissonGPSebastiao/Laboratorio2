Exerc_10:

Na primeira linha (MOV R0, #0x4), atribuímos ao registrador R0 o valor hexadecimal de 4;
Já na segunda linha, atribuímos o valor 2 hexadecimal ao Registrador R1;
Na terceira realizamos através do MUL a multiplicação de R0 e R1, e atribuímos a R3 para efeito de comparação;
Na quarta linha chamamos a subrotina Mul16b, na qual criamos um método de Multiplicação que obtém resultado semelhante ao Mul;
Na quinta linha finalizamos o programa, contudo, o programa antes de ser finalizado, salta a linha a sexta linha, na qual desenvolvemos a subrotína Mul16b;
Nessa Subrotína criamos uma pilha com os registradores R0, R1 e R3 através do método PUSH;
Na próxima linha atribuímos o valor 0 ao Registrador R2, e na seguinte atribuímos ao registrador R3 o valor #16;
Apó isso criamos uma subrotina chamada "loop", na qual Validamos se o R3 é 0 e quantonão for vamos realizarando a operação lógica semelhante a multiplicação;
Enquanto R3 não for 0 e enquanto R2 não chegar ao final da multiplicação, a subrotina fica em looping;
Depois que uma das condições é atendida o código retorna a "main", e finaliza!


Exerc_11:

Na primeira linha da "main" atribuimos o valor 4 hexadecimal ao registrador R0, e já na sequencia chamamos a subrotina criada para fatoração, chamada :Fat;
Na subrotina Fat, criamos uma pilha através do método push, utilizando o registrador LR;
Na sequência, atribuimos o valor do registrador R0 em LR;
Depois, chamamos uma subrotina de loop que subtrai 1 de LR e Retorna atribuir o valor de RL-1 em LR, através do mnemônico SUBS, com a condicional de carry {S};
Assim, chamamos a condicional BEQ em paralelo com a subrotina denominada jump na qual limpa-se o contador LR;
Na próxima linha o Valor de LR é multiplicado com o valor de R0  e atribuído o resultado a R0, e retorna a subrotina loop;
por fim, essas subrotinas rodam até o LR chegar a 0, quando ele chega a 0, a operação acaba sendo interrompida e adquirimos em R0 o valor fatorial inicial, nesse caso o fatorial de 4!
