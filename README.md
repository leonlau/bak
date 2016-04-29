# bak
bakup

tar -zcvf - test|openssl des3 -salt -k secretpassword | dd of=test.des3


dd if=test.des3 |openssl des3 -d -k secretpassword|tar zxf -
