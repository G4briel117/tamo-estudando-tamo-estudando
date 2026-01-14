  

  

## Fazer uma tabuada no for:

  

![[Untitled 38.png|Untitled 38.png]]

```Java
int mult;
    int tabu;
System.out.println("Quantos numeros terah a sua tabuada ?");
   tabu = leia.nextInt();
    System.out.println("Digite o numero para a tabuada  ");
        mult = leia.nextInt();
            
            for(int i = 1; i<=tabu;i++){
                double produto = i * mult;
                    
                    System.out.println(i+" X "+mult+" = "+ produto);
                
    
            }
    
    }

    
}
```

## Em ação

![[Untitled 1 26.png|Untitled 1 26.png]]





##### For descrecente com numeros pares


```Java

for(int i = 10; i >= 0; i-=2){// i recebe 10 e enquanto ele for maior que 0 ele vai decrementar -2 até ele ficar igual a 0 e essa operação ser verdadeira. O grande segredo é o i>=0 pq por causa desse igual ele só vai parar até ficar = 0.

System.out.println(i)
}


```




#for #repetição #while #dowhile