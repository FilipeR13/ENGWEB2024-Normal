# ENGWEB2024-Normal

## Preparação de dados

A primeira coisa feita para resolver o teste foi aceder ao site: [https://csvjson.com](https://csvjson.com) para transfomar o formato do ficheiro dado.

O resultado dessa transformação está no ficheiro `contratos2024.json`.

Após uma breve análise do ficheiro, foi possível perceber que os objetos do ficheiro não eram consistentes no que toca ao atributo `PrecoContratual`. Este atributo podia ser um número ou uma string. Para resolver este problema, foi necessário fazer um pequeno script em Python que transformasse todas as strings em números. O resultado dessa transformação está no ficheiro `contratos2024_fixed.json`. Para além disso, também foi tranformado o atributo `idContrato` em `_id` com um simples find and replace 

Com o ficheiro `contratos2024_fixed.json` pronto, foi possível importar os dados para uma base de dados MongoDB.

Para facilitar a importação dos dados, foi gerado o ficheiro `docker-compose.yml`.

Após correr o comando, foi possível aceder à base de dados e verificar que os dados foram importados com sucesso.

## Ex1

Para correr o primeiro exercício basta executar:

```bash
npm install
npm start
```

## Ex2

Para correr o segundo exercício basta executar:

```bash
npm install
npm start
```

## Docker

Foi ainda realizado o Dockerfile e o docker-compose.yml para facilitar a execução dos exercícios. Para correr basta executar:

```bash
docker-compose up --build -d
```
