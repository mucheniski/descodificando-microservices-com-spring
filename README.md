# Descodificando Microservices com Spring  
Evento Michelli Brito  

### -> Dia 18/10 (segunda-feira) - O fim dos Monolíticos  
Com os fim dos sistemas monolíticos é preciso saber mais do que apenas Java com Spring ou criação de APIs e para entender o que realmente te trará destaque no mercado nos dias de hoje e o que é preciso para receber as melhores remunerações acompanhe o primeiro dia do evento.  

É preciso criar sistemas Escaláveis, Disponíveis e Sustentáveis.  


### -> Dia 19/10 (terça-feira) - Fundamentos de Microservices  
Depois dos vários anos trabalhando com Microservices e diversos problemas enfrentados adquiri experiência e maturidade que quero compartilhar com vocês, vou discutir premissas essenciais sobre sistemas distribuídos e também trarei esclarecimentos sobre equívocos que geralmente causam confusão sobre Microservices.  

Exemplo de monolito.  
![](images/ArquiteturaMonolitica.png)  

Exemplo de Microserviços. 
![](images/ArquiteturaMicroservicos.png) 


Na arquitetura é preciso definir softwares com Alta disponibilidade e Manutenbilidade.
![](images/AltaDisponibilidadeeManutenbilidade.png)  

A arquitetura envolve desde conceitos tecnicos, até financeiros e gerenciais, moldados de acordo com a necessidade do negócio.  

Outro ponto a ser pensado é sobre a sincronia de dados, pois os bancos de dados estão separados.  
Consistência de dados é quando garantimos a integridade, não temos divergência e nem ambiguidade de dados dentro da aplicação.  
Quando os dados em todas as bases são replicados e atualizados.  
Porém não é possível garantir 100% de consistência com 100% de disponibilidade, é preciso fazer um trade off de acordo com a necessidade do negócio, por exemplo quando os dados de service de cliente são atualizados ou um novo cliente é criado, não é necessário deixar o service de pagamentos indisponível, pode ser feito o pagamento, e em outro momento os dados serem replicados do cliente para o pagamento.  
![](SincroniaDadosSistemasDistribuidos.png)  

Consistencia VS Disponibilidade. Teorema CAP.  
Possui 3 pontas - Disponibilidade, Consistência e Partição, e diz que nunca teremos condições de priorizar essas 3 pontas, sempre apenas 2 serão priorizadas.  
Microservices já priorizam a partição por se tratar de sistemas distribuídos, no caso precisamos pensar na arquitetura em um balanceamento entre as outras duas pontas.  
![](images/TeoremaCAP.png)  

Nesse caso existe uma consistencia eventual, pois os dados ficam por um tempo desatualizados, porém em algum momento esse dados vai ser atualizado para o sistema como um todo.  

Identificadores UUIDs temporais são uma boa prática para serem utilizados em sistemas de dados distribuidos, para evitar conflitos de identificadores.  

Não existe desacoplamento absoluto em microservices, e sim um acoplamento fraco, o objetivo é otimizar o acoplamento o máximo possível de forma a criar a interdependencia entre os serviços minimamente.  
Esse dependencia não é arquitetural, deve ser definido de acordo com a nescessidade do negócio.  
![](images/AcoplamentoFraco.png)  

Também não existe 100% de disponibilidade, os servicos sao criados de forma que alguns possam parar sem que afetem os demais, que é bem melhor do que nenhum parando.  
![](images/Disponibilidade.png)  


Também pode existir um serviço de base de dados compartilhada, onde alguns services comoartilham uma base e outros nao.  
![](images/DistribuicaoBaseDados.png)  


Não existe uma regra ou modelo para arquitetura de microservices, devem ser adaptados a cada negocio de acordo com a necessidade.  


### -> Dia 20/10 (quarta-feira) - Microservices Patterns  
API Composition, SAGA, Event Driven com Event Notification e Event State transfer, Circuit Breaker, Cross-Cutting e muito mais, uma verdadeira descodificação dos principais Microservices Patterns utilizados no mercado. Aprender esses padrões te trará conhecimentos necessários para não cometer erros ou reinventar a roda, um conjunto de soluções que te farão dar um salto na carreira.  


### -> Dia 21/10 (quinta-feira) - Apresentação Projeto Decoder  
Este evento é apenas uma degustação do que é realmente o Projeto Decoder, que venho trabalhando a meses e contém um conteúdo inédito e exclusivo no Brasil, acompanhe neste último dia o que tenho para você, é imperdível!  



Link dos vídeos.  
https://www.decoderproject.com/fundamentos-de-microservices?vgo_ee=Zs9SBwfBdP9E2QddIgXzpHwFoqDlMHNmyq65fGLdufk%3D  
