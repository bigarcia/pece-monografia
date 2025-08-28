Repositório para armazenar os códigos utilizados na Monografia da Especialização em Engenharia de Dados e Big Data da Poli USP (PECE)

## Configuração dos serviços da AWS:
1. Cria um bucket

```
aws s3api create-bucket \
  --bucket debt-recovery-segmentations \
  --region us-east-1
```
```
aws s3api put-bucket-versioning \
  --bucket debt-recovery-segmentations \
  --versioning-configuration Status=Enabled
```

```
aws s3api put-bucket-encryption \
  --bucket debt-recovery-segmentations \
  --server-side-encryption-configuration \
  '{"Rules":[{"ApplyServerSideEncryptionByDefault":{"SSEAlgorithm":"AES256"}}]}'
```
<img width="928" height="618" alt="image" src="https://github.com/user-attachments/assets/1b4b1420-66e1-4428-97ae-f32872e4ef98" />
