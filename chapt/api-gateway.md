## API Gateway

O **Amazon API Gateway** é um serviço gerenciado para criação, publicação, monitoramento e proteção de APIs REST, HTTP e WebSocket. Ele atua como porta de entrada (*front door*) para aplicações backend, seja em instâncias EC2, funções Lambda ou outros endpoints HTTP.

O API Gateway integra-se nativamente com o Lambda, formando a base da arquitetura serverless na AWS: o Gateway recebe as requisições HTTP, roteia para a função Lambda correspondente e retorna a resposta ao cliente. O serviço oferece recursos como autenticação via Cognito ou Lambda Authorizers, throttling, caching de respostas e geração automática de SDKs para os consumidores da API.
