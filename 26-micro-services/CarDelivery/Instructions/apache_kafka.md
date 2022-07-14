## Porque usar o Apache Kafka?
event-driven
  _ Carros.
  _ E-commerce.
  _ Alarmes.
  _ Monitoramento.
  _ Microsserviços.

Tempo Real
  É um sistema que quando se envia uma mensagem para ele, você dispara eventos muito mais rapidamente por conta da sua baixa latencia. Em média de 2 milissegundos. 

Histórico dos dados
  Ao fazer alguma coisa e envia-la ao kafka, ele vai pegar essa mensagem e persistir com um tempo determinado pelo desenvolvedor.

Caracteristicas
  _ Plataforma.
  _ Trabalha de forma destribuida.
  _ Banco de dados.
  _ Extremamente rápido e com baixa latência.
  _ Utiliza o disco ao invés da memória para processar os dados.


__NÃO É APENAS UM SISTEMA TRADICIONAL DE FILAS COMO O RabbitMQ__ 


## Conceito básico
O que é um "topic"
  _ Stream de dados que atua como banco de dados
  _ Todos os dados ficam armazenados, ou seja, cada topic tem o seu "local" para armazenar seus dados.
  _ Tópico possui diversas partições.
    _ Cada partição é definida por número. Ex: 0, 1, 2.
    _ Você é obrigado a definir a quantidade de partições quando for criar um Topic.


## Kafka Cluster
_ Conjunto de Brokers.
_ Cada Broker é um server.
_ Cada Broker é responsável por armazenar os dados de uma partição.
_ Cada partição de Topic está distribuida em diferentes brokers.

## Ecossistema
- Kafka Connect
  _ Connectors
- Confluent Schema Registry
- Rest Proxy
- ksqlDB
- Streams