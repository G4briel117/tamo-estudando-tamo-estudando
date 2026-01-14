
Ele é responsavel pelo tipo de mídia que vai ser consumido pelo endpoint. Seja no response ou requestbody....


```yaml
paths:
	/usuario:
		get:
			tags:
				-busca ae pae
				summary: Isso é importante ta ? 
				description: Isso é importante para muita coisa ta ? Descrição
				requestBody:
					description: Descrição do corpo 
					content:
						application/json:
							schema:
								$ref: '#/components/schemas/usuario'
					required: true
				
				responses:
					'200':
					description: Tlg né ?
					content: 
						application/json:
							schema:
								$ref: '#/components/schemas/respostadousuario'	



```