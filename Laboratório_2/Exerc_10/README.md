Exerc_10:

Na primeira linha (MOV R0, #0x4), atribu�mos ao registrador R0 o valor hexadecimal de 4;
J� na segunda linha, atribu�mos o valor 2 hexadecimal ao Registrador R1;
Na terceira realizamos atrav�s do MUL a multiplica��o de R0 e R1, e atribu�mos a R3 para efeito de compara��o;
Na quarta linha chamamos a subrotina Mul16b, na qual criamos um m�todo de Multiplica��o que obt�m resultado semelhante ao Mul;
Na quinta linha finalizamos o programa, contudo, o programa antes de ser finalizado, salta a linha a sexta linha, na qual desenvolvemos a subrot�na Mul16b;
Nessa Subrot�na criamos uma pilha com os registradores R0, R1 e R3 atrav�s do m�todo PUSH;
Na pr�xima linha atribu�mos o valor 0 ao Registrador R2, e na seguinte atribu�mos ao registrador R3 o valor #16;
Ap� isso criamos uma subrotina chamada "loop", na qual Validamos se o R3 � 0 e quanton�o for vamos realizarando a opera��o l�gica semelhante a multiplica��o;
Enquanto R3 n�o for 0 e enquanto R2 n�o chegar ao final da multiplica��o, a subrotina fica em looping;
Depois que uma das condi��es � atendida o c�digo retorna a "main", e finaliza!


Exerc_11:

Na primeira linha da "main" atribuimos o valor 4 hexadecimal ao registrador R0, e j� na sequencia chamamos a subrotina criada para fatora��o, chamada :Fat;
Na subrotina Fat, criamos uma pilha atrav�s do m�todo push, utilizando o registrador LR;
Na sequ�ncia, atribuimos o valor do registrador R0 em LR;
Depois, chamamos uma subrotina de loop que subtrai 1 de LR e Retorna atribuir o valor de RL-1 em LR, atrav�s do mnem�nico SUBS, com a condicional de carry {S};
Assim, chamamos a condicional BEQ em paralelo com a subrotina denominada jump na qual limpa-se o contador LR;
Na pr�xima linha o Valor de LR � multiplicado com o valor de R0  e atribu�do o resultado a R0, e retorna a subrotina loop;
por fim, essas subrotinas rodam at� o LR chegar a 0, quando ele chega a 0, a opera��o acaba sendo interrompida e adquirimos em R0 o valor fatorial inicial, nesse caso o fatorial de 4!
