## Uso

O tipo de dados `float` é normalmente usado em situações em que você precisa economizar memória e a precisão do número de ponto flutuante não é crítica.

### Sintaxe

`float variableName = value;`

```Java
public class FloatExample {
    public static void main(String[] args) {
        float pi = 3.14f;
        float gravity = 9.8F;
        System.out.println("Value of pi: " + pi);
        System.out.println("Value of gravity: " + gravity);
    }
}
```

Aqui, declaramos duas variáveis `float` `pi` e `gravity` com valores 3,14 e 9,8, respectivamente. O sufixo `f` ou `F` é necessário para indicar que esses literais são do tipo `float`. Em seguida, o programa imprime esses valores.

#java [[Tipos Primitivos|Para voltar a página de Tipos Primitivos]]
