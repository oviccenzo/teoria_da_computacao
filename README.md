Lista de Exercicios Praticos

Teoria das Funcoes Recursivas e Implementacao em Python

50 Questoes de Progresso Gradual (Versao do Aluno —
Sem Gabarito)

Disciplina: Teoria da Computacao — 

Professor: Getulio de Morais Pereira

September 29, 2026

Instrucoes e Regras para o Laboratorio
Objetivo: Ganhar fluencia no raciocinio recursivo 
denotacional e na construcao formal de funcoes.
Regra de Ouro: Para as questoes de funcoes puras, e
proibido utilizar operadores aritmeticos nativos (+,-, *, 
//, **) dentro das funcoes desenvolvidas. Toda a aritmetica
deve ser construida por meio da composicao das funcoes 
iniciais (z,s,Pn_1) e dos combinadores de 
composicao, recursao primitiva e mu_operador.

Nivel 1: Basico — Funcoes Iniciais e Composicoes Diretas 
(Questoes 1 a 15)

1. Implemente em Python a Funcao Zero z(x), que recebe 
um numero natural x ∈ N e retorna 0.

2. Implemente em Python a Funcao Sucessor s(x), 
que recebe um natural x e retorna x+1.

3. Implemente o projetor unario P1
1(x), que retorna o proprio argumento x.

4. Implemente o projetor binario P2
1(x1,x2), que retorna o primeiro argumento x1.

5. Implemente o projetor binario P2
2(x1,x2), que retorna o segundo argumento x2.

6. Escreva umafabrica geral de projetores em Python proj(i, n) 
que retorna uma funcao n-aria Pni (x1,...,xn).

7. Implemente por composicao direta a funcao 
constante c1(x) = 1 usando s e z.

8. Implemente por composicao direta
a funcao constante c2(x) = 2 usando s e c1.

9. Implemente por composicao a funcao constante 
c3(x) = 3 para qualquer entrada x.

10. Implemente a funcao add2(x) = x + 2 aplicando 
duas vezes a funcao sucessor por composicao.

11. Implemente a funcao add3(x) = x + 3 
por composicao de sucessores.

12. Escreva uma funcao em Python que recebe uma dupla
(x1,x2) e ignora x2, retornando sempre s(x1) usando s1 e P2_1.

13. Escreva uma funcao swap args(x1,x2) que simula 
a inversao de parametros usando projecoes P2_2 e P2_1.

14. Crie uma funcao c2_0(x1,x2) = 0 de aridade 2 que 
descarta ambos os argumentos e retorna zero via z e P2_1.

15. Escreva um decorador em Python @natural
domain que verifica se todos os argumentos de uma funcao sao
inteiros nao-negativos (≥ 0), lancando um ValueError caso contrario.


Nivel 2: Intermediario — Combinadores e Aritmetica Primitiva (Questoes 16 a 35)
16. Implemente o combinador generico de Composicao composicao(g, f_list) 
que constroi h(X) = g(f1(X),...,fk(X)).

17. Implemente o combinador de Recursao Primitiva recursao
primitiva(f, g) para funcoes de aridade arbitraria h(X,y).

18. Construa formalmente a Funcao Adicao add(x,y) = x + y 
usando recursao_primitiva P1_1 , s e p3_3.

19. Construa a Funcao Multiplicacao mult(x,y) = x · y 
usando recursao primitiva, P1_1, s e P3_3. primitiva,
z, add e projetores.

20. Construa a Funcao Exponenciacao exp(x,y) = xy 
por recursao primitiva a partir da multiplicacao.

21. Construa a funcao Fatorial fact(x) = x! por 
recursao primitiva usando mult.

22. Implemente a funcao Antecessor pred(x) = x ˙ - 1, 
onde pred(0) = 0 e pred(y +1) = y.

23. Construa a Subtracao Truncada / Monus sub(x,y) = x ˙ - y = 
max(0,x - y)  usando pred e recursao primitiva.

24. Construa a funcao Diferenca Absoluta abs 
diff(x,y) = |x - y| = (x ˙ - y) +(y ˙ -x).

25. Implemente a Funcao Sinal sg(x), 
que retorna 0 se x = 0 e 1 se x > 0.

26. Implemente a Funcao Sinal Inverso sg 
inv(x) = sg(x), que retorna 1 se x = 0 e 0 se x > 0.

27. Construa o Teste de Igualdade eq(x,y), que 
retorna 1 se x = y e 0 caso contr´ario.

28. Construa o Teste de Desigualdade neq(x,y),
que retorna 1 se x̸ = y e 0 se x = y.

29. Construa a funcao Menor ou Igual leq(x,y), 
que retorna 1 se x ≤ y e 0 caso contrario.

30. Construa a funcao Estritamente Menor lt(x,y), 
que retorna 1 se x < y e 0 caso contrario.

31. Construa a funcao Maior ou Igual 
geq(x,y) e a funcao Estritamente Maior gt(x,y).

32. Implemente a funcao Maximo max val(x,y) = 
max(x,y) usando adicao e subtracao truncada.

33. Implemente a funcao Minimo min val(x,y) = min(x,y) 
usando adicao e subtracao truncada.

34. Implemente o seletores condicional cond
if(c, t, f), que retorna t se c = 1 e f se c = 0.

35. Demonstre que a soma de uma constante fixa add k(k) 
pode ser construida por aplicacao repetida da
composicao do sucessor s.

Nivel 3: Avancado — Minimizacao, Teoria e Algoritmos Com
plexos (Questoes 36 a 50)

36. Implemente o Combinador de Minimizacao Ilimitada 
mu_operador(f), que busca o menor y ∈ N tal que f(X,y) = 0.


37. Construa a Divisao Inteira Exata div(x,y) = 
⌊x/y⌋ via µ-operacao para y > 0.

38. Construa a funcao Resto da Divisao 
/ Modulo mod(x,y) = x (mod y) utilizando sub e mult.

39. Construa a funcao Raiz Quadrada 
Inteira root(x) = ⌊√x⌋ usando o µ-operador.

40. Implemente o predicado Divisibilidade divides(x,y), 
que retorna 1 se x divide y (x | y) e 0 caso contrario.

41. Construa uma funcao num divisors(n) que conta o 
numero total de divisores de n usando recursao limitada.

42. Construa o predicado Teste de Primalidade is prime(n),
que retorna 1 se n for um numero primo e 0 caso contrario.

43. Implemente a Funcao de Ackermann A(m,n) em Python 
e explique por que ela nao pertence `a classe PR.

44. Escreva uma funcao recursiva pura sum
list(lst) em Python que calcula a soma dos elementos de uma
lista sem usar lacos nativos (for/while).

45. Escreva uma funcao recursiva pura len
list(lst) que calcula o comprimento de uma lista em Python.

46. Implemente a busca de elementos contains(lst, elem) em uma lista 
usando estritamente recursao e condicionais funcionais.

47. Construa a Funcao Par de Cantor π(x,y) = (x+y)(x+y+1) / 2 + y ,
que codifica um par de naturais em um único natural de forma bijetiva

48. Implemente o desempacotamento de Cantor π1(z) e π2(z) usando 
a µ-operacao para decodificar o par original (x,y).


49. Simule a parcialidade (⊥) criando uma funcao g(x) = µy[(x · y) + 1 = 0] e 
verifique o comportamento de loop infinito em Python ao tentar executa-la.

50. Explique conceitualmente em um breve texto por que a classe das funcoes
µ-recursivas parciais e equivalente em poder de computacao `as Maquinas de Turing

esse exercício são lista práticos sobre funções recursiva e a teoria das funções que são usado para resolver calculo 
avançado como pré-calculo , calculo 1 e 2 e os calculos 3 e 5 são mais avançado a medida que o calculo matematico seja 
mais dificeis de resolver do que codificar em código fonte python


