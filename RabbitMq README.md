Running the RabbitMQ using Docker. we have certain steps :
1) run this (docker ps) to check docker is running or not ?

2) docker run -d --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:management

Run RabbitMQ in detached mode (-d)

Expose:

5672 for AMQP (backend connection)

15672 for the management UI (browser access)

3)next run the program in IntelliJ 

4) check the message is published or not using
 http://localhost:15672

5) The Consumer will arrive then the ready queue message will consumed by consumer. 