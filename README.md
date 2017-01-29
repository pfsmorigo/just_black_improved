# Google Chrome Theme Generator

 * Just run 'make'
 * It will create the key if necessary and the chrome_theme.crx file.

```
Creating key to be used by the theme...

openssl genrsa -out rsa.pem 768
Generating RSA private key, 768 bit long modulus
.++++++++
....++++++++
e is 65537 (0x10001)
openssl pkcs8 -topk8 -nocrypt -in rsa.pem -out key.pem
rm rsa.pem

Creating theme...

./crxmake chrome_theme key.pem
Wrote chrome_theme.crx
```
