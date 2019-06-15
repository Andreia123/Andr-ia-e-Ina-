# PONTEIROS, REFERÊNCIAS, FUNÇÕES E BIBLIOTECAS EM ALGUMAS  LINGUAGENS DE PROGRAMAÇÃO




Andreia Nunes Rodrigues
Inaê Ribeiro dos Santos


## Resumo
O artigo tem como objetivo identificar e descrever , de modo sintetizado como funciona ponteiro, na linguagem de programação C/C++, referências em Java, JavaScript e PHP, funções(parâmetro, retorno e recursividade) em C/C++, Java, JavaScript e PHP e, as bibliotecas dentro dessas linguagens.
O nosso artigo tem como propósito aprendemos e passamos aos colegas novas linguagem de programação. Porque até  mesmo para sermos bons programadores devemos ter conhecimento do vasto mundo da liguagem de programação .
Neste artigo vamos explorar os conceitos empregos e definições de ponteiro, referências, parâmetro, retorno, recursividade e bibliotecas, sendo usados as linguagems de programação: C\C++, Java, JavaScript, PHP. 

Palavras-chave: Ponteiro(C/C++), Referências(Java, JavaScript, PHP), Funções: parâmetro, retorno e recursividade(Java, JavaScript, C/C++, PHP), Bibliotecas.


## Definição de ponteiro
São entes que possuem o poder de armazenar o endereço onde estão localizadas determinadas informações. Falando em termos de programação, podemos entender um ponteiro como uma variável que armazena (aponta) um endereço de memória onde está localizado um valor.

Exemplo:
```c
#include <stdio.h>
void main()
{
int a;
int b;
int c;
int *ptr;

a = 90;
b = 2;
c = 3
ptr = &a;
printf("Valor de ptr: %p, Conteúdo de ptr: %d\n, ptr, *ptr")
printf(“B: %d, C: %d, %c“);
}

```

## Ponteiros na linguagem C
Ponteiros na linguagem C são tipos especiais de variáveis que armazenam não um dado diretamente (um inteiro, um real, um caractere) mas sim o endereço de memória onde um dado se encontra. Os ponteiros são declarados como se fossem variáveis normais do tipo desejado, porém usando um  * para indicar que é um ponteiro, como mostra os exemplos abaixo:
Exemplo 1:
```c
int  *ponteiroParaInt;

Exemplo 2:
int umInteiro = 100;
int *ponteiroParaInt = &umInteiro;
printf("%d\n", *ponteiroParaInt);                            // Imprime 100.
*ponteiroParaInt = *ponteiroParaInt * 2;               // Note os dois usos de *.
printf("%d\n", umInteiro);                                      // Imprime 200.
printf("%p\n", ponteiroParaInt);                             // Imprime o endereço.

```

## Referência em Java
As variáveis do tipo referência tem a função de armazenamento de localizações de objetos na memória do computador . Sendo assim os objetos que são referenciados acaba por conter várias variáveis que são denominadas de instância , assim armazenado métodos dentro do objeto apontado.
Para colocar em um objeto os seus métodos de instância é preciso ter referência a algum objeto  . As variáveis de referência que utilizamos para iniciar um método de instância na maioria das vezes será iniciado com o valor “null”.
Exemplo:
```java
Public class AcessaMetodo {
public  Void imprime(){
System.out.printLn(“bem vindo ao Java!”);
}
public  Static Void main (String[]args){
AcessaMetodo acessa =new AcessaMetodo ();
}
}
```

É bom lembrar que as variáveis de tipos valor não se leva referência a objeto , também se emprega as variáveis do tipo primitivo não podem ser inicializadas como referência a um objeto.


## Definção de função em JavaScript
Funções são blocos de construção fundamentais em JavaScript. Uma função é um procedimento de JavaScript - um conjunto de instruções Dque executa uma tarefa ou calcula um valor. Para usar uma função, você deve defini-la em algum lugar no escopo do qual você quiser chamá-la.
A definição da função (também chamada de declaração de função) consiste no uso da palavra chave , function como a seguir:
Nome da Função
Lista de argumentos para a função, entre parênteses e separados por vírgulas. 
Declarações JavaScript que definem a função, entre chaves { }.

Por exemplo, o código a seguir define uma função simples chamada square:

```js

function square(numero) { 
  return numero * numero; 
}

```
A função square recebe um argumento, chamado numero. A função consiste em uma instrução que indica para retornar o argumento da função (isto é, numero) multiplicado por si mesmo. A declaração return especifica o valor retornado pela função.

```j'

return numero * numero;

```

## Funcões com Parâmetro:
Parâmetros primitivos (como um número) são passados para as funções por valor. O  valor é passado para a função, mas se a função altera o valor do parâmetro, esta mudança não reflete globalmente ou na função chamada. Se você passar um objeto (ou seja, um valor não primitivo), tal como Array ou um objeto definido por você) como um parâmetro e a função alterar as propriedades do objeto, essa mudança é visível fora da função, conforme mostrado no exemplo a seguir:


```js

function minhaFuncao(objeto) {
  objeto.make = "Toyota";
}

var meucarro = {make: "Honda", model: "Accord", year: 1998};
var x, y;

x = meucarro.make;            // x recebe o valor "Honda"

minhaFuncao(meucarro);
y = meucarro.make;          // y recebe o valor "Toyota"
                           // (a propriedade make foi alterada pela função)
```

## Retorno em JavaScript
A declaração return finaliza a execução de uma função e especifica os valores que devem ser retonados para onde a função foi chamada, como o exemplo abaixo:

```js

return [[expression]]; 
expression 

```
A expressão cujo valor será retornado. Se omitido, undefined é retornado. 
Quando uma declaração return é usada em um corpo de função, a execução dessa função é parada. Se especificado, um dado valor é retornado à quem chamou a função. Se a expressão for omitida, undefined será retornado. Todas as declarações return a seguir param a execução da função:

```js

return;
return true;
return false;
return x;
return x + y / 3;

```

## Função com recursividade
A recursão acontece quando a solução de um problema depende da aplicação dessa mesma solução a outras instâncias dela. Por exemplo, o fatorial de 4 também pode ser definido como o fatorial de 3 multiplicado por 4 e assim por diante. Isso significa que o fatorial de um número pode ser definido em termos de si mesmo, como o exemplo abaixo:

```js

factorial(5) = factorial(4) * 5
factorial(5) = factorial(3) * 4 * 5
factorial(5) = factorial(2) * 3 * 4 * 5
factorial(5) = factorial(1) * 2 * 3 * 4 * 5
factorial(5) = factorial(0) * 1 * 2 * 3 * 4 * 5
factorial(5) = 1 * 1 * 2 * 3 * 4 * 5
Em poucas palavras, quando uma função se chama, podemos dizer que temos recursão.

```

## Bibliotecas:
### JQuery
jQuery é uma biblioteca JavaScript criada para facilitar o desenvolvimento de web sites e aplicações web based.
Com ela é possível se manipular o HTML das páginas de maneira dinâmica, também é possível a alteração de propriedades, manipulação de eventos como click, mouseover, submit etc. Também é possível usar jQuery para se criar animações e efeitos. Muito útil para designers sem experiência em programação.
O lema desta biblioteca é “Write Less, Do More”. Literalmente, “Escreva Menos e Faça Mais”. jQuery é Cross-browser, ou seja, compatível com os 5 principais navegadores do mercado. Também é compatível com CSS3 e muito leve (aproximadamente 24BK compactada).


## Biblioteca padrão da linguagem
C Standard Library é o nome da biblioteca padrão da linguagem C. Esta biblioteca possui uma série de funções prontas com recursos adicionais e disponíveis para utilização. A biblioteca padrão de C é composta ao todo por 24 arquivos de cabeçalho. Como podemos ver a quantidade de arquivos da biblioteca é bem pequena. A ideia por trás dessa biblioteca é fornecer apenas um conjunto básico de operações, de tal forma que a portabilidade do C ANSI entre diversas plataformas seja relativamente simples.
Além da biblioteca padrão, outras bibliotecas foram desenvolvidas para incorporar outras funcionalidades específicas.














## Referências:
DAMAS, LUÍS. Linguagem C. 10ª Edição, gen|LTC.

E. SILVA, SOUZA, VÍTOR. Programacão básica de Computadores. Universidade Federal do Espírito Santo. (INF 09325) – 2013/1.

https://www.ic.unicamp.br/~wainer/cursos/2s2011/Cap08-Funcoes-texto.pdf
https://www.inf.pucrs.br/~pinho/LaproI/Funcoes/AulaDeFuncoes.htm

http://fabriciosanchez.azurewebsites.net/3/ponteiros-o-que-sao-e-para-que-servem/
https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Fun%C3%A7%C3%B5es
https://medium.com/@osuissa/tudo-sobre-recurs%C3%A3o-ptc-tco-e-stc-em-javascript-58953a5a846a
http://linguagemc.com.br/a-biblioteca-padrao-da-linguagem-c/
http://www.contagia.com.br/tecnologia/jquery/
