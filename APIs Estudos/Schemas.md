
seção que pode ser chamada de estrutura de dados ou modelo de dados  que mostram os dados que vao ser consumidos ou reproduzidos pela API. Vai criar uma seção que pode ser acessado pelo nome schemas


```yaml

components:
	schemas:
		User:
			type: object #Ele pertence a use e ele é um objeto
			properties: #ele tem como propriedade o id e name
				id:
					type: integer
					format: double
					example: 1
				name:
					type: String
					example: Clovis Basilio
			required: #tao informado que toda vez que o User for usado ele tem que usar o id e name. São campos requiridos. Por exmeplo: Todas as vezes que vocÊ for cadastrar um usuario esse campo não pode ficar em branco. Por isso o required
				-id
				-name
		

```