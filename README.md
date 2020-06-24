## Objetivo
Criar uma aplicação web que implemente um CRUD de veículos com atributos como Montadora, Modelo, Cor, Quilometragem, Motor e Tipo.
A aplicação é apenas uma API REST utilizando Java Spring Boot e 
que atenda as operações de pesquisa, inserção, edição e exclusão.
A aplicação deve ser executada no <a href="https://www.heroku.com/#">Heroku</a>, um serviço de computação em nuvem do tipo PASS.

### Testes com URL's da API
#### GET <br>
Busca por Id:<br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/10

Filtrado por três atributos(tipo, montadora e km):<br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/filtros/CARRO/FORD/1000

Lista todos veículos:<br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/lista

#### POST <br>
Inserção de dados: <br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/adiciona
<br>
 {
  "id":4,
  "montadora":"BUGATTI",
  "modelo":"CHIRON",
  "cor":"PRETO",
  "km":15000,
  "motor":"9999999",
  "tipo":"CARRO"
 }

#### PUT <br>
Alteração de dados: <br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/modifica
<br>
{
 "id":7,
 "montadora":"KAWAZAKI",
 "modelo":"ZZR",
 "cor":"VERMELHO",
 "km":50000,
 "motor":"1100CC",
 "tipo":"MOTO"
}

#### DELETE <br>
Exclusão de dados por Id: <br>
https://sestrem-veiculos-api.herokuapp.com/veiculos/deleta/2
