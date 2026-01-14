## Uso

O tipo de dados `boolean` é normalmente usado em instruções de fluxo de controle, como os loops `if`, `while` e `for`, para determinar o fluxo do programa com base em determinadas condições.

### Sintaxe

`boolean variableName = value;`

- `variableName`: O nome da variável.
- `value`: O valor a ser atribuído à variável, que deve ser `true` ou `false`.

```Java
public class BooleanExample {
    public static void main(String[] args) {
        boolean isJavaFun = true;
        boolean isFishTasty = false;
        System.out.println("Is Java fun? " + isJavaFun);
        System.out.println("Is fish tasty? " + isFishTasty);
    }
}
```
Neste exemplo, duas variáveis `boolean` `isJavaFun` e `isFishTasty` são declaradas e inicializadas com `true` e `false`, respectivamente. Em seguida, o programa imprime esses valores.

[[Tipos Primitivos|Volte para a pagina de Tipos de primitivos]]
