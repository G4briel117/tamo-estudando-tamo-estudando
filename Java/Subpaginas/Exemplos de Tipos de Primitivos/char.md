## Uso

Uma classe serve como um modelo para a criação de objetos. Ele encapsula os dados do objeto e os métodos para manipular esses dados.

### Sintaxe

`class ClassName {     // fields     // methods }`

- `ClassName`: O nome da classe, que, por convenção, deve começar com uma letra maiúscula.
- `fields`: Variáveis que mantêm o estado da classe.
- `methods`: Funções que definem o comportamento da classe.

```Java
class Animal {
    String name;
    int age;

    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

public class Main {
    public static void main(String[] args) {
        Animal dog = new Animal();
        dog.name = "Buddy";
        dog.age = 5;
        dog.displayInfo();
    }
}
```

Neste exemplo, a classe `Animal` tem dois campos, `name` e `age`, e um método, `displayInfo()`. A classe `Main` demonstra a criação de um objeto `Animal` e a configuração de seus campos.

#java  [[Tipos Primitivos|Para voltar a página Tipos Primitivos]]

