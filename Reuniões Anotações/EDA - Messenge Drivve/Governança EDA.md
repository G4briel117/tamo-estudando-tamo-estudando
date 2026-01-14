

## Qual a ideia ?

- Mapas de capacidades - Governanças de EDA - Event Daily Archtecture
- Como implementar ?
- Ja falaram que estão fazendo a respeito 

- Falar mais sobre a parte de mensageria



### O que é a Arquitetura de Eventos ?


- O que acontece no govapp quando falamos de cadastro de aplicações 
- Faço o cadastros
	-  Dados
	- Nome
- Quando passa pelo fluxo de cadatro ele é aceito e passa pelo servicenow, o cmd onde faz a integração.
- E o govapp fala pro service now estaá aqui a estrutura e o govapp fala pro leanix

- Arquitetura de eventos 
- Ao inves de fazer a chamada e responder todo mundo que depende dela. A jornada de aplicação depende do término de informar os service now, azure devops, leanix

Transformar o acontecimento a respeito da informação de algo


Publicar em uma fila Que um evento aconteceu e partir dali o govapp não se importa com o que aconteceu e quem está interessado nessa fila vai acompanhar. Basicamente isso

## Terá o envolvimento de dominios

- Basicamente evento não estará associado a nenhuma aplicação, mas sim em um dominio, pois pode ser utilizado por qualquer aplicação.

### Comunicação assincrona

- Pensa que temos um ms1 e ms2.
	- O ms1 pode chamar o ms2 e aguardar ? Seria sincrona


- O ms1 chama o ms2 e ele vai la e posta uma fila e vai ter um outra cara (ms3) para fazer essa comunicação. Isso é assincrono pois ele ta livre e pega pra ele. Essa fila é um componente, pois é a forma que o ms1 tem de se comunicar com o ms2  E neles tem o correlationID, ele bus o mesmo id tanto na requisição, tanto na resposta


Message Drive API - API que usa mensageria como comunicação

- Nossa missão é definir um padrão
	Definimos a comunicação
	Requisitos de comunicação


![[Pasted image 20251201142743.png]]

AsyncAPI - OpenAPI para mensageria 

- Padronizar a espec Message-Driven APIs (AsyncAPIs)
- 

