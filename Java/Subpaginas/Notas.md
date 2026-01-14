
## jshell

No Java 9 foi introduzido um recurso que é possivel de fazer que seria introdução de um compilador para testes rapido no cmd. Apenas digitando "jshell" no cmd que é possivel de fazer alguns testes rapido.

*********************************
## Inferência

Um recurso que foi introduzido no Java 10
[[4. Inferência de Tipos|Inferência]] 

************************
## Numero Literal

Se entende como um numero que foi colocado direto no código, não foi um usuário externo que colocou.

*****************

## Separar por Underline

É possível separar os numero por Underline `_`. Aparentemente parece ser mais facil.

***********************************

## String não é um tipo primitivo

- Pois dados primitivos são todos aqueles que derivam de Object.
- String se inicia com `S` e não `s`, pois não é uma palavra reservada.

***************

## Indentação e Correção do códigos


Fazendo o comando `Ctrl + o` o próprio Java arruma o código, adicionando e tirando tudo o que não precisa.

**************

## String o que é ?

Em resumo, as strings correspondem a uma sequência (ou cadeia) de caracteres ASCII delimitados por aspas duplas, que são armazenadas em "instâncias" da classe String.

***********

## Substring o que é ?

uma substring é como um pedacinho de string que você pode pegar emprestado para usar como quiser! Meow, é como cortar um pedaço de fio para 
fazer algo novo.

************

## Uma String é *imutavel*

É impossível modificar o valor que foi colocado em uma String, pois ela é um objeto imutavel.


**********

### Potencia

``` Java
.Math.Pow(variavel,numero da potência que vai ser elevado);
```


``` Java
double a = (3 * 4) - 10;
double b = Math.Pow(a,3);
// ele vai fazer a sentença ser "potencializada a 3(ao cubo)", lembrando que o resultado será double, para mudar basta colocar (int) Math.Pow(a,3);
System.out.println(b)


```


************************


### Operador de Incremento ++

```Java
// Utilizando o ++ em uma variavel é como se estivessemos adiconando ele mesmo +1...


int b = b++ // == b+1



```

###### Isso também serviria para o operador - Que nesse caso seria "--" e ele seria a propria variavel -1

##### Precedência
No Java caso você coloque o sinal antes do elemento `variavel` ele vai entender que você esta com pressa para fazer o incremento, caso opte por colocar depois da `variavel` ele vai entender que você não está com tanta pressa 


##### EX:
```Java
int a=1
int b=2

System.out.println("++a == b--") -> true
// Ele vai entender que primeiro vem o incremento "++a" e depois o "b--". O java entende que só vai decrementado o "b", após ter incrementado o "++a" e comparado se ele é igual com o "b--"

// Por isso que primeiro ele vai incrementar e comparar com o b, então ele vai dar que é true, não false.

```
****
### Operador Ternario
*Operador Condicional* nesse caso você tem a capacidade de *escolher* entre um operador ou outro



Ex: 

```Java

double media = 7.6;
String resultado = media >= 7.0 ? "aprovado" : "recusado";

//Nesse caso a gente tem uma atribuição ternaria, pq tem uma expressão que pode ser verdadeira ou falsa "media >= 7.6" e o operador ternario "?" tem dois simbolos o "?" que separa a expressão e os valores a ser atribuidos ("aprovado", "recusado") e o ":" que separa os valores de atribuição entre falsa e verdadeira (recusado e aprovado)
```
Nesse caso a gente tem uma atribuição ternaria, pq tem uma expressão que pode ser verdadeira ou falsa `media >= 7.6` e o operador ternario `?` tem dois simbolos o `?` que separa a expressão e os valores a ser atribuidos (`"aprovado"`, `"recusado"`) e o `:` que separa os valores de atribuição entre falsa e verdadeira (`recusado` e `aprovado`)

#### Ex com multiplos operadores ternários


```Java

double media = 7.6;

String mediaBaixa = media <= 5.0 ? "vai passar pelo conselho" : "não vai passar pelo conselho ";
String resultado = media >= 7.0 ? "aprovado" : mediaBaixa;

System.out.println(resultado)

// OU

double media = 7.6;
String resultado = media >= 7.0 ? "aprovado" : media <= 5.0 "vai passa pelo conselho" : "não vai passar pelo conselho"


System.out.println(resultado)


```

###### Muito util quando você recebeu um resultado e quer mostrar se é verdadeiro ou demonstrar o valor de uma forma mais visual.

*********

#### JRE vs JDK

Geralmente quando se cria uma classe em java ela é representanda em aquivo `.java`  e quando você executa um arquivo `.java` é feito a compilação `.class`.

E existe o `Bytecode` que é o resultado gerado do arquivo `.class` e para isso ser "lido" pela maquina é necessario um `JVM` que irá se comunicar com o windows atraves disso.

*JRE - Java Runtime Env.* - Usuario que ira utilizar o `JRE`
*JDK - JAVA Dev. Kit* - Dev que irá utilizar o `JDK`
*JVM - Java Virtual Machine* `JVM`
*****************************

## .equalsIgnoreCase(variavel ou string)

Essa comparação de `String` ignora os uppercamelcase, lowecase ou o que for. Apenas executa.


```Java



Scanner ler = new Scanner(System.in);
System.out.println("Que dia tu quer escolher ? Pra somar em pontos");

String dias = ler.nextLine();

if(dias.equalsIgnoreCase("segunda")){
System.out.println(1);
}
else if (dias.equalsIgnoreCase("terça")){
System.out.println(2);
}

```

******************

Declaração de variaveis dentro de um laço

Ja sabemos que é impossível acessar uma variavel se ela for declarada dentro do `escopo` do `for`, pois ela contem o proprio escopo.
```Java

for(int i =0; i<=10; i++){
System.println(i)
}
System.println(i)// dará erro, pois essa variavel existe apenas dentro do campo for
```

uma forma de poder usar isso é declarar fora do laço
```Java
int i = 0;

for(;i<=10; i++){

System.out.println(i)

}
System.println(i)// Nesse caso mostrará o valor de 10, pois ela foi declara fora do escopo for

```

*************



#java #jshell