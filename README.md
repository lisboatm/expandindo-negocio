# README - Consulta de Cidades com Clientes

## Descrição

Este projeto tem como objetivo ajudar uma locadora a identificar todas as cidades onde seus clientes residem. A locadora planeja expandir suas franquias pelo Brasil e precisa de informações precisas sobre a localização de seus clientes. O foco é obter uma lista única de cidades, sem repetições.

## Estrutura do Banco de Dados

### Tabela: `customers`

A tabela `customers` contém informações sobre os clientes da locadora e possui a seguinte estrutura:

| Coluna | Tipo     | Descrição                          |
|--------|----------|------------------------------------|
| id     | numeric  | Identificador único do cliente (PK)|
| name   | varchar  | Nome do cliente                    |
| street | varchar  | Endereço do cliente                |
| city   | varchar  | Cidade onde o cliente reside       |

#### Exemplo de Dados

| id | name                         | street                                  | city            |
|----|------------------------------|----------------------------------------|------------------|
| 1  | Giovanna Goncalves Oliveira   | Rua Mato Grosso                        | Canoas           |
| 2  | Kauã Azevedo Ribeiro         | Travessa Ibiá                         | Uberlândia       |
| 3  | Rebeca Barbosa Santos        | Rua Observatório Meteorológico         | Salvador         |
| 4  | Sarah Carvalho Correia       | Rua Antônio Carlos da Silva           | Uberlândia       |
| 5  | João Almeida Lima            | Rua Rio Taiuva                        | Ponta Grossa     |
| 6  | Diogo Melo Dias             | Rua Duzentos e Cinqüenta             | Várzea Grande    |

## Objetivo da Consulta

Realizar uma consulta SQL para selecionar o nome de todas as cidades onde a locadora tem clientes, garantindo que cada cidade seja listada apenas uma vez.

### Consulta SQL Exemplo

A consulta pode ser feita da seguinte forma:

```sql
SELECT DISTINCT city
FROM customers;
```

### Saída Esperada

A saída da consulta deve exibir a lista de cidades, ordenada conforme a apresentação desejada, como no exemplo abaixo:

| city           |
|----------------|
| Uberlândia     |
| Canoas         |
| Ponta Grossa   |
| Várzea Grande  |
| Salvador       |

## Instruções de Uso

1. **Conexão com o Banco de Dados**: Certifique-se de estar conectado ao banco de dados que contém a tabela `customers`.

2. **Executar a Consulta**: Utilize a consulta SQL mencionada para obter a lista de cidades.

3. **Verificar Resultados**: Revise a saída para confirmar que todas as cidades foram corretamente listadas, sem repetições.

## Contribuições

Este projeto está aberto a sugestões e melhorias. Sinta-se à vontade para contribuir com novas funcionalidades ou correções.

## Licença

Este projeto não possui uma licença definida. Consulte o responsável pelo projeto para mais informações.
