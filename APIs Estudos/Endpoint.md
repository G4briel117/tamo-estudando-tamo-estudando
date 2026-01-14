
São elas que permitem a comunicação entre os sistemas 

***Cada endpoint representa um recurso ou função especifica dentro da API

*Nem toda classe vai ter um endpoint* e o fator que determina isso é: "Alguma API vai disponibilizar algum objeto dessa classe ? " "A API vai utilizar algum dado dessa classe ?"

No API REST o que define o endpoint é o metodo, não o nome.

Para a criação de um Endpoint no openAPI:

``` YAML
paths:
	/endpoint

```