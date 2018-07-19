# crackpkcs8

#### A modified thread ready program (crackpkcs12)to run a dictionary attack on a certificate.

From http://sourceforge.net/projects/crackpkcs12/ or https://github.com/crackpkcs12/crackpkcs12/


#### Compile: (Need package libssl-dev to compile)

git clone https://github.com/j0nk0/crackpkcs8

cd crackpkcs8

gcc crackpkcs8.c -o crackpkcs8 -lssl -lcrypto -lpthread


#### To run and decrypt Superfish_CA.pem:(password komodia)(https://blog.erratasec.com/2015/02/exploiting-superfish-certificate.html)

openssl rsa -in Superfish_CA.pem -out Superfish_CA.key


