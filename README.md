### Curso: Programação Orientada a Objetos com Java
### http://educandoweb.com.br
### Prof. Dr. Nelio Alves

# workshop-spring-mongodb
### Projeto MongoDB com Spring Boot

# Objetivo geral:

* Compreender as principais diferenças entre paradigma orientado a documentos e relacional
* Implementar operações de CRUD
* Refletir sobre decisões de design para um banco de dados orientado a documentos
* Implementar associações entre objetos
* Objetos aninhados
* Referências
* Realizar consultas com Spring Data e MongoRepository

# Diagrama de Classes:

![image](https://github.com/MauroJRamos/workshop-spring-mongodb/assets/82981926/11cb2ec1-d33b-419a-a861-e95e71e0bbb2)

# Representação da entidade no banco:

```
{
"id": "1001",
"name": "Maria Brown",
"email": "maria@gmail.com",
"posts": [
{
"date": "2018-03-21",
"title": "Partiu viagem",
"body": "Vou viajar para São Paulo. Abraços!",
"comments": [
{
"text": "Boa viagem mano!",
"date": "2018-03-21",
"author": {
"id": "1013",
"name": "Alex Green"
}
},
{
"text": "Aproveite!",
"date": "2018-03-22",
"author": {
"id": "1027",
"name": "Bob Grey"
}
}
]
},
{
"date": "2018-03-23",
"title": "Bom dia",
"body": "Acordei feliz hoje!",
"comments": [
{
"text": "Tenha um ótimo dia!",
"date": "2018-03-23",
"author": {
"id": "1013",
"name": "Alex Green"
}
}
]
}
]
}```
