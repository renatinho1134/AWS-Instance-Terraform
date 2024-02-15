# Configuração de uma Instância t2.micro na AWS com Terraform

Este repositório contém os arquivos necessários para provisionar uma instância t2.micro na AWS usando o Terraform. Esta é uma maneira rápida e eficiente de configurar sua infraestrutura na nuvem de forma automatizada.

## Pré-requisitos

Antes de começar, certifique-se de ter os seguintes itens instalados em seu ambiente de desenvolvimento:

- [Terraform](https://www.terraform.io/downloads.html)
- [AWS CLI](https://aws.amazon.com/cli/)

Além disso, você precisa configurar suas credenciais da AWS no seu ambiente. Isso pode ser feito executando `aws configure` e fornecendo suas credenciais de acesso IAM.

## Instruções de Uso

1. Clone este repositório para o seu ambiente local:

    ```
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```

2. Navegue até o diretório do projeto:

    ```
    cd nome-do-repositorio
    ```

3. Inicialize o diretório do Terraform:

    ```
    terraform init
    ```

4. Visualize as mudanças planejadas:

    ```
    terraform plan
    ```

5. Aplique as mudanças para provisionar a instância na AWS:

    ```
    terraform apply
    ```

6. Após a conclusão bem-sucedida, você verá a saída com informações sobre a instância provisionada.

## Personalização

Você pode personalizar a instância conforme suas necessidades, modificando o arquivo `main.tf`. Este arquivo contém a configuração da instância EC2, incluindo tipo, região, chave SSH, etc.

## Limpeza

Para evitar custos desnecessários, é recomendável destruir os recursos provisionados quando não estiverem mais em uso. Você pode fazer isso executando:
```
terraform destroy
```
## Avisos

- **Custos**: Esteja ciente de que provisionar recursos na AWS pode resultar em custos. Certifique-se de entender a estrutura de preços da AWS e os custos associados à execução de instâncias EC2.
- **Segurança**: Não compartilhe suas credenciais da AWS com terceiros e siga as melhores práticas de segurança ao lidar com infraestrutura na nuvem.

Para mais informações sobre como usar o Terraform com a AWS, consulte a [documentação oficial do Terraform](https://learn.hashicorp.com/collections/terraform/aws-get-started).

