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

----
###### System Design e System Architecture
![[Pasted image 20260120211450.png]]

###### System Design - Tem uma visão mais de modulo, não de código de fato, mas ele mostra mais detalhes em especifico
Por Exemplo
- Tem componente A que vai fazer a chamada para uma API e esse API vai bater em um gateway que vai fazer a validação e devolver a chamada para o componente A em formato de arquivo XML 

###### System Architecture - Ele ve de uma maneira mais ampla, mais generalizada o os componentes
Por Exemplo
- Componente B faz uma chamada em um API esse API vai devolver a chamada autenticada

*Event Bus* - Um padrão de design e uma arquitetura que permite.
- Um **evento** é algo que aconteceu  
    👉 “pedido criado”, “pagamento feito”, “botão clicado”
    
- O **Event Bus** é o lugar onde esses eventos são anunciados
     ^9c0727
- Outros pedaços do sistema **escutam** esses eventos e agem

### Pull e Push

👉 **PUSH: o sistema te avisa.**  
👉 **PULL: você pergunta ao sistema.** ^a2fc15


## O que é Kubernetes?

^ef95be

**Kubernetes** (ou **K8s**) é um **robô super organizado** 🤖  
que **cuida dos seus aplicativos** para você.

Ele:

- coloca cada app no lugar certo
    
- fica olhando se algum quebrou
    
- arruma sozinho
    
- cria mais cópias quando tem muita gente usando
    

---

## 📦 Conceitos importantes (bem simples)

### 🟦 Container

É como uma **lancheira** 🍱  
Dentro dela tem o aplicativo + tudo que ele precisa pra funcionar.

Ex: Docker

---

### 🟨 Pod

^8f1b87

É um **grupo de lancheiras** andando juntas.  
Normalmente 1 app por Pod.

---

### 🖥️ Node

É um **computador** onde os Pods rodam.

---

### 🌍 Cluster

É o **conjunto de computadores** (Nodes).

---

### 👮 Kubernetes (o chefe)

Ele decide:

- onde cada Pod vai rodar
    
- se um app caiu → cria outro
    
- se tem pouca gente usando → diminui
    
- se tem muita gente usando → aumenta
    

---

## 🚑 Exemplo simples

1. Seu app está rodando
    
2. Um computador desliga ❌
    
3. Kubernetes percebe
    
4. Ele cria o app em outro computador ✅
    
5. Tudo continua funcionando