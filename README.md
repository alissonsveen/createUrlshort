# 🔗 **URL Reduzida - Java com AWS Lambda e S3** 🚀

Este projeto Java tem como objetivo criar uma URL reduzida a partir de uma URL longa. Ele utiliza a **AWS Lambda** para processar as requisições e **Amazon S3** para armazenar as URLs curtas geradas. A manipulação dos dados é feita com a biblioteca **Jackson**.

## 🚀 **Tecnologias Utilizadas**

- **Java**: Linguagem de programação principal.
- **AWS**:
  - **AWS Lambda**: Função serverless para processar a geração das URLs encurtadas.
  - **Amazon S3**: Para armazenar as URLs encurtadas e gerenciar os arquivos.
  - **Jackson**: Para manipulação de JSON.
  
## ⚙️ **Funcionalidades**

- 📝 **Entrada**: Recebe uma URL longa como entrada.
- 🔗 **Geração**: Cria uma URL curta única e a armazena em um arquivo no S3.
- 🛠 **Escalabilidade**: Utiliza a AWS Lambda para processar as requisições de forma escalável e eficiente.
- 🌍 **Saída**: Retorna a URL curta gerada.

## 🧩 **Como Funciona?**

O código funciona criando uma versão encurtada de uma URL longa e armazena essa URL curta em um arquivo no **Amazon S3**. O processo é feito através de uma **função Lambda** que recebe a URL longa, gera a chave curta e salva no S3. Quando a URL curta é acessada, a Lambda retorna a URL longa associada.

### Passos do Funcionamento:
1. **Recebe a URL longa**: O usuário fornece a URL longa.
2. **Gera uma chave curta**: O código cria uma chave compacta (geralmente um hash ou base64).
3. **Armazena a chave no S3**: A chave curta e a URL longa são salvas em um arquivo no S3.

## 🛠 **Como Rodar o Projeto**

### Pré-requisitos:
- 🌐 **Java 8 ou superior** instalado.
- 🧑‍💻 **IDE** como IntelliJ IDEA, Eclipse ou NetBeans (opcional).
- 🛠 **AWS CLI**: Ferramenta de linha de comando da AWS configurada com suas credenciais.
- 💡 **AWS Account**: Conta configurada para usar S3 e Lambda.
- **Jackson**: Para manipulação de JSON.
