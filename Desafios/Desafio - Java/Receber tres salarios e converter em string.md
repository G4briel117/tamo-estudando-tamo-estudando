```Java

public class desafio {

public static void main(String[] args) {

Scanner ler = new Scanner(System.in);

System.out.println("salario de voces: ");

String sal1 = ler.nextLine().replace(",", ".");

String sal2 = ler.nextLine().replace(",", ".");

String sal3 = ler.nextLine().replace(",", ".");

System.out.println("Salarinho");

Double numb1 = Double.parseDouble(sal1);

Double numb2 = Double.parseDouble(sal2);

Double numb3 = Double.parseDouble(sal3);

Double result = numb1 + numb2 + numb3;

System.out.println(result);

System.out.println("A média dos seus salarios são: "+result/3 );

}
```


Como é possivel ver a gente utilizou o `.replace(",",".")` Para que todas as vezes que o ponto a virgula fosse colocada, fosse feito a troca para o `.` e assim não dar erro no nosso código.


