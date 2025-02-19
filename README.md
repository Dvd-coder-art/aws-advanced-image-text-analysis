# Análise Avançada de Imagens e Texto com IA na AWS

Este projeto visa demonstrar como é possível realizar a **análise de imagens e textos** usando ferramentas poderosas da **AWS**, como **Amazon Textract** para extração de texto e dados estruturados, e **Amazon SageMaker** para aplicar modelos de machine learning na automação e melhoria das análises.

## Objetivo

O objetivo deste projeto é extrair texto e dados estruturados de documentos, como **faturas, contratos, formulários e outros tipos de arquivos digitalizados** utilizando **Amazon Textract**, e depois utilizar o **Amazon SageMaker** para aplicar técnicas de machine learning na análise dos dados extraídos. O projeto pode ser estendido para diferentes cenários de uso, como análise de imagens, processamento de dados financeiros, ou automação de processos de negócios.

## Ferramentas e Tecnologias Utilizadas

- **Amazon Textract**: Serviço de OCR (Reconhecimento Óptico de Caracteres) que permite a extração de texto e dados estruturados de documentos digitalizados.
- **Amazon SageMaker**: Serviço de machine learning que facilita a criação, treinamento e implementação de modelos de ML.
- **Amazon S3**: Armazenamento de dados, utilizado para salvar os documentos processados.
- **AWS Lambda**: Para automação do processo de extração e análise.
- **Python**: Linguagem utilizada para scripts e automação dos fluxos de trabalho.

## Passo a Passo do Projeto

### 1. Configuração do Amazon Textract
Primeiro, o serviço **Amazon Textract** foi utilizado para extrair texto e dados estruturados de documentos digitalizados. O processo de extração envolveu a configuração do serviço para identificar texto, tabelas e campos-chave, com o objetivo de coletar as informações essenciais de documentos como **contratos** e **faturas**.

#### Exemplos de documentos processados:
- **Faturas de fornecedores**
- **Contratos comerciais**
- **Formulários de cadastro de clientes**

![Exemplo de documento processado](screenshot1.png)

### 2. Integração com o Amazon SageMaker
Após a extração dos dados, os resultados foram utilizados como entrada para modelos de **machine learning** no **Amazon SageMaker**. O objetivo aqui foi aplicar modelos que pudessem automatizar a **análise de dados** para prever ou classificar informações extraídas, como valores de transações ou identificar padrões de comportamento nos contratos.

#### Modelos usados:
- **Modelo de Regressão** para prever valores baseados nos dados extraídos.
- **Classificação** para categorizar documentos de acordo com sua natureza (ex: fatura, contrato, etc.).

### 3. Insights e Possibilidades
Durante o desenvolvimento deste projeto, alguns **insights importantes** foram descobertos:
- **Precisão de extração**: O Amazon Textract tem uma alta taxa de precisão, mas em alguns casos, especialmente em documentos com formatação inconsistente, a limpeza e preparação dos dados extraídos podem ser necessárias.
- **Expansão para outros cenários**: A automação de análise de documentos pode ser expandida para **atendimento ao cliente**, **processamento de sinistros de seguros** ou até mesmo **análise de compliance**.
- **Melhoria com Custom Models**: O uso de modelos personalizados no SageMaker pode ajudar a melhorar a precisão das previsões e permitir análises mais específicas com dados personalizados.

### 4. Desafios
- **Documentos com texto manuscrito**: Documentos com texto manuscrito ou muito mal formatados podem representar um desafio para o Textract, resultando em algumas imprecisões.
- **Limitações de formato**: O Textract funciona melhor com arquivos PDF ou imagens bem formatadas, sendo necessário algum pré-processamento para garantir a melhor qualidade de extração.

## Como Executar o Projeto

1. Clone este repositório para seu ambiente local:
   ```bash
   git clone https://github.com/seunome/aws-advanced-image-text-analysis.git
