# SSL Cryptography

### Generate a 2048-bit RSA private key
- `openssl genrsa -out ssl_key.pri 2048`

### Generate a public key using a private key
- `openssl rsa -in ssl_key.pri -pubout -out ssl_key.pub`


### Encrypt File
- `openssl pkeyutl -encrypt -inkey /path/to/public_key -pubin -in <file.txt> -out
  <file.enc>`

### Decrypt File  
- `openssl pkeyutl -decrypt -inkey /path/to/private_key -in /path/to/<file.enc>`


