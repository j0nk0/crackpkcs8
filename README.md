# crackpkcs8

I needed to check a dictionary of passwords for a certificate. Linear approach was insufficient, so I modified a thread ready program from http://sourceforge.net/projects/crackpkcs12/ or https://github.com/crackpkcs12/crackpkcs12/

Compile:

gcc crackpkcs8.c -o crackpkcs8 -lssl -lcrypto -lpthread

Note: You would need libssl-dev as requirement to compile


Decrypt Superfish_CA.pem:(password komodia)(https://blog.erratasec.com/2015/02/exploiting-superfish-certificate.html)

 openssl rsa -in Superfish_CA.pem -out Superfish_CA.key
