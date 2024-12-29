# Sistema de Forum usando Nest e Clean Architecture com conceitos de DDD

## Criando chaves JWT RSA256

Chave privada
```bash
openssl genpkey -algorithm RSA -out private_key.pem -pkeyopt rsa_keygen_bits:2048
```

Chave pública
```bash
openssl rsa -pubout -in private_key.pem -out public_key.pem
```

Tornando as chaves base64 (Ubuntu)

```bash
cat private_key.pem | base64 >> privete.txt
```

```bash
cat public_key.pem | base64 >> public.txt
```