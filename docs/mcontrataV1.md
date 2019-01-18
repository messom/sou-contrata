### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

## End-points

HTTP requisição | Descrição | Exemplo
------------- | ------------- | -------------
**GET** /notices/{id} | Exibe todos os editais | *http://localhost:3001/api/v1/notices/*





**GET** /student/{id}
---
Exibe o estudante

Exibe o estudante pelo seu id

### Parâmetros

Nome | Tipo | Descrição | Exemplo
------------- | ------------- | ------------- | -------------
 **id** | **Integer** | requerido no PATH | *http://localhost:3001/api/v1/student/1*

### Status Code

**200** ```OK```

### Exemplo de resposta
```json
{
	"studentData": [
		{
			"id": 1,
			"firstName": "Alice",
			"lastName": "Pereira Rodrigues",
			"assumedName": "",
			"birthDate": "1989-01-06",
			"gender": "F",
			"countryBirth": "Brasil",
			"nationality": "Brasileira",
			"race": 0,
			"marital": 2,
			"bloodType": 2,
			"organDonor": true,
			"cellphone": "35992755126",
			"personalEmail": "alicepereirarodrigues@outlook.com",
			"professionalEmail": "alice.rodrigues@jourrapide.com",
			"documents": {
				"rg": {
					"number": "273044576",
					"issuer": "SSP"
				},
				"cpf": "17143053929",
				"electoralCard": "516485230175",
				"certificateReservist": ""
			},
			"parents": {
				"motherName": "Joana Pereira Rodrigues",
				"fatherName": "Jurandir Oliveira Rodrigues"
			},
			"address": {
				"street": "Rua da Vitória",
				"number": "66",
				"zip": "07600100",
				"district": "Anhangabau",
				"city": "São Paulo",
				"state": "SP"
			}
		}
	]
}
```
**404** ```Not Found```

**500** ```Erro interno no servidor```
