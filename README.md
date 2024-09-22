# terraform-sample

<h3>
  Este repositório fornece um estudo completo, cobrindo todo o processo de construção e implantação de uma aplicação SpringBoot utilizando Terraform, AWS e Docker.
</h3>

## Tecnologias utilizadas

* Terraform
* AWS - EC2

## Pré Requisitos

- Conta AWS
- AWS CLI
- Terraform CLI
- Public and Private KeyPair for SSH

## Passo a passo

- Efetue a criação de uma conta na AWS
- Crie um usuário com acesso programático (aws_access_key_id & aws_secret_access_key)
- Instale a AWS CLI no seu computador e execute o 'aws configure'
- Instale o Terraform CLI no seu computador
- Gere um KeyPair para poder acessar a EC2 via SSH (ssh-keygen)
- Execute 'terraform init' dentro da pasta 'infra' no terminal
- Execute 'terraform plan' dentro da pasta 'infra' para verificar o plano de criação do terraform

- Execute 'terraform apply' dentro da pasta 'infra' para criar a infraestrutura
- Execute 'terraform destroy' dentro da pasta 'infra' destruir toda a infraestrutura criada

## Construindo a imagem docker e enviando para o dockerhub

```

$ ./app docker build . -t agnaldoanjos/public-api:latest
$ ./app docker login
$ ./app docker push agnaldoanjos/public-api:latest

```

Baixe o projeto e teste você mesmo na prática.

