Repositório para armazenar os códigos utilizados na Monografia da Especialização em Engenharia de Dados e Big Data da Poli USP (PECE)

## Configuração dos serviços da AWS:
1. Cria um bucket

```
aws s3api create-bucket \
  --bucket debt-recovery-segmentations \
  --region us-east-1
```
