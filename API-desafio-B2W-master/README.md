# API-desafio-B2W


Para o Projeto foi utilizado:

Java 8, 
Spring Suite Tools 4 (Spring Boot),
Banco de Dados MongoDB,
Postman



Obs: para executar a API foi utilizada a IDE Spring Tool Suite 4 (STS)





Informações Importantes para uso da API:
- Para utilizar a API é necessário configurar o servidor do MongoDB e iniciá-lo.



Como o projeto foi feito no Linux, foi utilizado o link para configuração (Até o passo 2):

https://www.digitalocean.com/community/tutorials/como-instalar-o-mongodb-no-ubuntu-16-04-pt



Obs: Passo 3 não foi necessário.


Configuração application.properties do Spring:
spring.data.mongodb.host=localhost
spring.data.mongodb.port=27017
spring.data.mongodb.database=b2w




EndPoints da API, realizados através do Postman e localhost via Mozila para comprovacão.


- Listar os planetas Salvos : (GET) http://localhost:8080/planetas 
- Salvar um determinado planteta : (POST) http://localhost:8080/planetas
    Informando um JSON:
    
    Ex:
    
     {
        "nome": "Geonosis",
        "clima": "temperado, árido",
        "terreno": "rocha, deserto, montanha, estéril"
    }
  
  
- Buscar um planeta por id : (GET) http://localhost:8080/planetas/{id}
- Busca um planeta po nome : (GET) http://localhost:8080/planetas/{nome}/nome
- Remover planeta : (DELETE) http://localhost:8080/planetas/{id}


Consumindo a API do link: https://swapi.co/ :

Ao salvar planeta, ele se comunica com API do Star Wars, obtem a quantidade de aparições e finaliza o processo de salvar.
