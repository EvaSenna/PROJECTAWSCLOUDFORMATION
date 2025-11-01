# PROJECTAWSCLOUDFORMATION
# AWS CloudFormation — Infraestrutura como Código (IaC)

Este repositório contém anotações, insights e exemplos práticos adquiridos durante o estudo e implementação de **infraestruturas automatizadas na AWS utilizando o CloudFormation** organizado com ajuda da IA.

O objetivo é fornecer um material de apoio para futuras implementações e consolidação do aprendizado sobre **Infraestrutura como Código (IaC)**.



## O que é o AWS CloudFormation

O **AWS CloudFormation** é um serviço que permite **criar e gerenciar recursos da AWS de forma automatizada e segura**, por meio de **modelos declarativos** escritos em **YAML ou JSON**.

Com ele, podemos:
- Provisionar toda a infraestrutura com um único arquivo (template);
- Garantir consistência entre ambientes (desenvolvimento, testes, produção);
- Versionar a infraestrutura (Git + IaC);
- Automatizar atualizações e remoções com segurança.



## Estrutura básica de um template CloudFormation

Um template geralmente contém quatro seções principais:

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: Template básico para criação de recursos AWS
Resources:
  MeuBucketS3:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: meu-bucket-exemplo
