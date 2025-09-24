# Desafio: Automatizando Tarefas com Lambda Function e S3

## Descrição do Repositório  
Este repositório reúne a prática de automação de tarefas utilizando AWS Lambda, Amazon S3, DynamoDB e API Gateway em ambiente local com LocalStack.  
O projeto demonstra a criação e gerenciamento de recursos por meio de templates do CloudFormation e inclui exemplos de processamento de arquivos JSON, servindo como material de estudo e referência para futuras implementações.  

## Visão Geral  
Este projeto foi desenvolvido em ambiente local utilizando o LocalStack, simulando serviços da AWS para testes.  
Foram aplicados conceitos de automação de infraestrutura na AWS com CloudFormation, permitindo a criação e gerenciamento de recursos via templates.  

## Serviços Utilizados  
- Amazon S3 → Armazenamento de objetos (upload de notas fiscais em `.json`).  
- AWS Lambda → Processamento automático dos arquivos enviados ao S3.  
- Amazon DynamoDB → Armazenamento estruturado dos dados processados.  
- Amazon API Gateway → Exposição dos serviços via endpoint HTTP.  
- LocalStack → Simulação local dos serviços AWS.  
- CloudFormation → Automação da criação de recursos (templates em JSON/YAML).  

## Fluxo da Solução  
1. Criamos um arquivo JSON fake de notas fiscais.  
2. O arquivo foi enviado ao bucket S3.  
3. Esse evento disparou automaticamente a execução de uma função Lambda.  
4. A Lambda processou os dados e os gravou no DynamoDB.  
5. A integração foi exposta via API Gateway, simulando consumo por aplicações externas.  

## Aprendizados  
- Como utilizar o LocalStack para simular recursos AWS.  
- Integração de eventos do S3 com Lambda Functions.  
- Criação de infraestrutura como código com CloudFormation.  
- Uso do DynamoDB como banco serverless para persistência de dados.  
- Exposição de serviços via API Gateway.  
