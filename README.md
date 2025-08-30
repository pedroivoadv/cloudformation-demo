# AWS CloudFormation Demo

## Validar template

    aws cloudformation validate-template --template-body file://template.yaml

## Criar um nova pilha

    aws cloudformation create-stack --stack-name MinhaPilha --template-body file://template.yaml

## Atualizar pilha

    aws cloudformation update-stack --stack-name MinhaPilha --template-body file://template.yaml

## Deletar pilha

    aws cloudformation delete-stack --stack-name MinhaPilha

## Resumo

    Resumindo o fluxo de uma aplicação típica com esses serviços:

    Usuário acessa um endpoint no API Gateway.

    O API Gateway chama uma Lambda para processar a requisição.

    A Lambda pode ler/escrever no DynamoDB ou interagir com o S3.

    Tudo isso foi criado/configurado pelo CloudFormation.