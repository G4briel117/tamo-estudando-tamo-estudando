  

```Java
package javaapplication3;
import java.util.Scanner;
import java.util.Random;
public class JavaApplication3 {

    public static void main(String[] args) {
        // TODO code application logic here
   Scanner leia = new Scanner(System.in);
    Random random = new Random();
       
    boolean acertou = false;
    int tentativas = 10;
    int numeroSecret = random.nextInt();
    long chute = 0;
    
    System.out.println(numeroSecret);
        while(tentativas > 0 && acertou==false){
        
            System.out.println("Qual o seu chute no random meno ?");
                chute = leia.nextLong();
                
        
                if(numeroSecret == chute){
                
                System.out.println("Acertou demais essa porra de numeo, da não ");
                 acertou=true;
                
                    }else if(chute< numeroSecret){
                     --tentativas;   
                     System.out.println("Ta pequeno irmao, vai mais maior por ai "+tentativas+" tentativas restantes");
                                
                         }else if (chute > numeroSecret){
                            --tentativas;
                             System.out.println("Ta maior carai "+tentativas+" Tentativas restantes");
                                          
                                  }else if(chute > numeroSecret&&tentativas==1){
                                   --tentativas;
                                      System.out.println("Maluco, tu chegou a 0 tentativas pqp "+tentativas);
                                  
                                  } else if(chute < numeroSecret&&tentativas==1){
                                  --tentativas;
                                      System.out.println("Maluco, tu chegou a 0 tentativas pqp "+tentativas);
                                  
                                  }
                
                
                
        }
    
    
    
    
   
    }
    
    
}
```

  

  

![[Untitled 10.png|Untitled 10.png]]

  

explicarei mais tarde, desculpa