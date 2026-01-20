#patterns #LargeScale #ComplexArchtectures 
### Patterns - São padrões existentes na arquitetura que resolvem diversos problemas testados 

*A falta de conhecimento desses Patterns fere a qualidade de uma arquitetura na qual foi selecionada*

Imagina que você tem a sua arquitetura e você quer expandir ela. Pra aumentar o consumo da sua arquitetura.
Então como que você expande o seu banco de dados, expande os seus componentes ? São coisas que você vai fazendo por etapas

*Over Thinking* - Excesso de pensamento 

Auto Scalling - Aumento de capacidade ou não 
	Ex: Um site que recebe poucas visitas à noite e muitas durante o dia.  
O próprio sistema cria mais servidores de dia e reduz à noite. ^80205f

*Trace Ability* - Basicamente o rastreamento, a capacidade de saber exatamente de onde algo veio, por onde passou e onde esta agora dentro de um sistema ^726c22

 *Deploy*  - colocar ou atualizar a aplicação em um ambiente
 *Deploy em prod* → quando ela vai para **prod**  

*OKR ( Objective and Keys Results)*- São definidos resultados chaves que são medido em cima de um objetvo
 Exemplo ^ee194a
- Imagina que é passado um Objetivo de melhorar a relação e comunicação com o cliente.
  
  As areas vão se perguntar: O que eu posso fazer para melhorar isso ? 
  
  -É passado isso para TI no caso. O T.I pode ter a iniciativa de: "Podemos construir um chatbot para melhorar a relação e o atendimento do cliente e facilitar a vida do atendente na hora de resolver os problemas com o cliente e no final é medido o impacto desse resultado para saber se o objetivo foi alcançado"
  
  O time tecnico então sera encarregado disso e fará essa tarefa
  
  Os resultados vão ser medidos e depois de concluidos o objetivo sera atingido

##### Failover

^06fcb5

###### Explicação prática

- Servidor A está em produção (principal).
    
- Servidor A cai.
    
- Servidor B assume automaticamente.
    
- O usuário final quase não percebe a falha.


TPS (Transaction Per Second) -> Transações por segundo ^b06802