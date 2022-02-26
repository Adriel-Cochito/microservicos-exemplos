# Aplicações de Microservicos
 Microserviços utilizando PostgreeSQL e Spring Boot

 ## O que faz essa aplicação?
 - Cria uma API em formato de microserviço  que permite o envio de email automaticamente ou programado partindo do email de envio para o destinatário descritos no método POST de requisição a API

 ### Componentes:
 - PostgreeSql
 - RabbitMQ 
 - Spring Boot:
   - Spring Web
   - Spring Data JPA
   - PostgreeSQL Driver
   - Validation
   - Lombok

### Json para envio do email:

Utilizar o Postman no metodo Post com o link abaixo:
```
http://localhost:8080/sending-email
```


Json a ser enviado:
```
{
    "ownerRef": "Adriel",
    "emailFrom": "xxxxxxxxxxx@gmail.com",
    "emailTo": "xxxxxxxxxxxxxx@gmail.com",
    "subject": "Testando envio de Emails por Microservices",
    "text": "Olá! Tudo bem? Meu nome é Cochito e estou passando aqui pra avisar que os testes com microserviços estão sendo realizados, e este email foi enviado automaticamente pelo aplicação JAVA no Spring Boot como um microserviço. Não deixe de acessar também nosso site: https://eletrica3d.tech/ e aprender um pouco mais sobre eletricidade. Abraços."
}
```
