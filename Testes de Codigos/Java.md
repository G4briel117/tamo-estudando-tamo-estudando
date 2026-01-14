  

# Teste com While - Enquanto o meu nome não for escrito ele não sairá disso.

```Java
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package pkgwhile;
import java.util.Scanner;
/**
 *
 * @author Luciene
 */
public class While {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
    Scanner ler = new Scanner(System.in);
           int cont =1;
           String nome;
           
           System.out.println("Caso seu nome seja Gabriel, nem escreva, pois saira");
           System.out.println("Digite seu nome: ");
           nome = ler.nextLine();
           
             while(!nome.equals("Gabriel")){
                 
               System.out.println(cont);
               cont++;
               System.out.println("Seja bem vindo"+nome);
               System.out.println("Digite outro nome:");
               nome = ler.nextLine();
               
    }
           }

    
    }
```

## Escreva um programa que le 3 valores inteiros(considere que não serão lidos valores iguais) e escrevê-los em ordem crescente (Usando o If, Else, Else If)

  

```JavaScript
System.out.println("coloque um numero carai, rapidones: ");
    int a = ler.nextInt();
    System.out.println("coloque um numero ai meno: ");
    int b = ler.nextInt();
    System.out.println("coloque o ultimo numero carai, acabou meno, vou ter que fazer moh grandao pqp");
    int c = ler.nextInt();
    
    
int meio; int menor; int maior;
          //a b c = a1 b2 c3
            /*a b c
              1 2 3*/         
               if(a<b && a<c){
                  menor = a;
                   if(b<c){
                   meio=b;
                   maior=c;
                   System.out.println(menor+", "+meio+", "+ maior);}    
                   else{System.out.println(menor+", "+c+", "+b );}
                              
               }else if (a>b && a>c){
                } maior = a;
                    if(b<c){
                    menor=b; meio=c;
                    System.out.println(menor+", "+meio+", "+maior);
                    }
                else{System.out.println(c+","+b+","+maior);}
    
                    if(a<b && a>c){
                        meio = a;}
                        if(b>c){
                     System.out.println(b+", "+a+", "+c);
                    }
                        else{System.out.println(c+", "+a+", "+b);}
                        
}
}
```







#### Teste de While indeterminado com String

```Java
package controle;
import java.util.Scanner;

public class teste_de_repetição {

public static void main(String[] args) {

Scanner ler = new Scanner(System.in);

String number = "";

while(!number.equalsIgnoreCase("40028922")) {

System.out.println("Qual o numero daquele programa da sua infancia ?");

number = ler.nextLine();

if(number.equalsIgnoreCase("40028922")) {

System.out.println("Parabens irmao, você é uma ótima pessoa, sabe das coisa");

}else {

System.out.println("\nContinua que ta pertinho irmao. Quase lá\n");

}

}

System.out.println(number);

double valor = Double.parseDouble(number);

System.out.println("sabia que esse numero acima da conversa é do bom dia e cia ?");

double soma = valor + 10;

System.out.println(soma);
```