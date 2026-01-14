
### Identação

Identação é muito chata por isso tem que estar sempre alinhada

```
paths:
	'/users':
	description: teste do teste
	
	post: 
		description: descrição do metodo #descrição do metodo e deve ficar a uma identação a mais
		tags: #vocÊ consegue segregar por tags cada metodo
		- Usuarios
		
		requestBody: #alinhado com o description e acima de response, sempre
			content: 
				applicatin/json: #responsavel pelo tipo de midia que vai ser consumida. Nesse caso ela vai receber dados formatados como JSON
		response:
			'200'
		description: Teste da resposta


```