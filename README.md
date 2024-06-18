# mike-sem9


## Passos a passo: Mike M

## Arquivo main.tf

```
    terraform {
        required_providers {
            aws = {
            source  = "hashicorp/aws"
            version = "~> 4.16"
            }
        }

        required_version = ">= 1.2.0"
        }

        provider "aws" {
        region = "us-east-1"
        }

        resource "aws_instance" "app_server" {
        ami           = "ami-830c94e3"
        instance_type = "t2.micro"

        tags = {
            Name = "ExampleAppServerInstance"
        }
    }

```

## Instalação:

```
aws configure
```

```
    aws configure set aws_session_token SESSIONTOKENHERE
```

```
    terraform init
```

```
    terraform fmt
```  

```
    terraform validate
```

```
    terraform plan
```

```
    terraform apply
```



## AWS:

Foi criada um instância EC2 na AWS.


### Comando

```
    terraform show
```
