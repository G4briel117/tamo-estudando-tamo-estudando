
## Uso

O tipo de dados `long` é comumente usado em situações em que são necessários valores inteiros grandes, como em cálculos científicos, aplicativos financeiros ou ao lidar com grandes conjuntos de dados

### Sintaxe

`long variableName = value;`

```Java

public class LongExample {
    public static void main(String[] args) {
        long population = 7800000000L;
        long distanceToMoon = 384400000L;
        System.out.println("World Population: " + population);
        System.out.println("Distance to Moon in meters: " + distanceToMoon);
    }
}
```

Neste exemplo, duas variáveis `long` `population` e `distanceToMoon` são declaradas com valores 7.800.000.000 e 384.400.000, respectivamente. O sufixo `L` é usado para indicar que os literais são do tipo `long`.

[[Tipos Primitivos|Para voltar a página de Tipos de Primitivos]]
