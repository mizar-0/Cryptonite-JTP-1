# Week 1.
## Installation
Had to enable WSL in Control Panel>Programmes>Turn windows features on and off

## Level 0:
learnt to use `ssh` command to log into remote server

## Level 0 => 1: 
learnt `cat` command. Tried logging into bandit1 from bandit0. Request was blocked. Solved by exiting bandit0 and logging in from own computer.

## Level 1 => 2: 
`-` is a special character because it is used to specify tags. Hence, path must be specified for file names starting with `-`.

## Level 2 =>3: 
used `‘’` to specify that filename with spaces was one filename and not many

## Level 3 => 4: 
files can be hidden by preceding filename with `.`. Use `ls -a` to list all files of directory.

## Level 4 => 5: 
used `file` command to determine type of all files. Used `./*` to specify all files. lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
<img src="https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L4-L5.png" width="800" />

## Level 5=>6: 
it was only required to use `find ./* -size 1033` to find the next password, even though the problem mentioned other requirements. P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU.
![L5](Images/L5-L6.png)

## Level 6=>7: 
used `find` with options `-size` `-user` `-group` and `grep` to find files containing ‘password’
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
![L6](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L6-L7.A.png)
![L6](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L6-L7.png)

## Level 7 => Level 8: 
used `cat` to read data.txt, piped the output to `grep` to find the required word
TESKZC0XvTetK0S9xNwm25STk5iWrBvP
![L7](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L7-L8.png)

## Level 8 => 9:
`uniq` filters only adjacent matching lines from the file. Hence, the lines need to be sorted before uniq is used.
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
![L8](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L8-L9.png)

## Level9 => Level10:
Used `strings` with `-e s` option to specify ASCII encoding and piped the o/p to `grep ==` . GREP stands for Global Regular Expressions Print.
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
![L9](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L9-L10.png)

## Level 10=> Level 11: 
`<string> base64` can be used to encode string in base 64. The option `–decode` makes it possible to do the reverse.
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
![L10](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L10-L11.png)

## Level 11 => 12: 
read man page for `tr`. Had to consult stackexchange to find the exact way to specify a rot13 cipher using `tr`. JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
![L11](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L11-L12.png)

# Week 2

## Level 12 => 13: 
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw. Consulted walkthrough. Learnt to decompress compressed files. The required password was obtained after multiple decompressions using `tar`, `bunzip2`, `gunzip`. 
![L12]()

## Level 13 => 14: 
This level only requires us to obtain the private key to be used in the next level.



-----BEGIN RSA PRIVATE KEY-----
MIIEpAIBAAKCAQEAxkkOE83W2cOT7IWhFc9aPaaQmQDdgzuXCv+ppZHa++buSkN+
gg0tcr7Fw8NLGa5+Uzec2rEg0WmeevB13AIoYp0MZyETq46t+jk9puNwZwIt9XgB
ZufGtZEwWbFWw/vVLNwOXBe4UWStGRWzgPpEeSv5Tb1VjLZIBdGphTIK22Amz6Zb
ThMsiMnyJafEwJ/T8PQO3myS91vUHEuoOMAzoUID4kN0MEZ3+XahyK0HJVq68KsV
ObefXG1vvA3GAJ29kxJaqvRfgYnqZryWN7w3CHjNU4c/2Jkp+n8L0SnxaNA+WYA7
jiPyTF0is8uzMlYQ4l1Lzh/8/MpvhCQF8r22dwIDAQABAoIBAQC6dWBjhyEOzjeA
J3j/RWmap9M5zfJ/wb2bfidNpwbB8rsJ4sZIDZQ7XuIh4LfygoAQSS+bBw3RXvzE
pvJt3SmU8hIDuLsCjL1VnBY5pY7Bju8g8aR/3FyjyNAqx/TLfzlLYfOu7i9Jet67
xAh0tONG/u8FB5I3LAI2Vp6OviwvdWeC4nOxCthldpuPKNLA8rmMMVRTKQ+7T2VS
nXmwYckKUcUgzoVSpiNZaS0zUDypdpy2+tRH3MQa5kqN1YKjvF8RC47woOYCktsD
o3FFpGNFec9Taa3Msy+DfQQhHKZFKIL3bJDONtmrVvtYK40/yeU4aZ/HA2DQzwhe
ol1AfiEhAoGBAOnVjosBkm7sblK+n4IEwPxs8sOmhPnTDUy5WGrpSCrXOmsVIBUf
laL3ZGLx3xCIwtCnEucB9DvN2HZkupc/h6hTKUYLqXuyLD8njTrbRhLgbC9QrKrS
M1F2fSTxVqPtZDlDMwjNR04xHA/fKh8bXXyTMqOHNJTHHNhbh3McdURjAoGBANkU
1hqfnw7+aXncJ9bjysr1ZWbqOE5Nd8AFgfwaKuGTTVX2NsUQnCMWdOp+wFak40JH
PKWkJNdBG+ex0H9JNQsTK3X5PBMAS8AfX0GrKeuwKWA6erytVTqjOfLYcdp5+z9s
8DtVCxDuVsM+i4X8UqIGOlvGbtKEVokHPFXP1q/dAoGAcHg5YX7WEehCgCYTzpO+
xysX8ScM2qS6xuZ3MqUWAxUWkh7NGZvhe0sGy9iOdANzwKw7mUUFViaCMR/t54W1
GC83sOs3D7n5Mj8x3NdO8xFit7dT9a245TvaoYQ7KgmqpSg/ScKCw4c3eiLava+J
3btnJeSIU+8ZXq9XjPRpKwUCgYA7z6LiOQKxNeXH3qHXcnHok855maUj5fJNpPbY
iDkyZ8ySF8GlcFsky8Yw6fWCqfG3zDrohJ5l9JmEsBh7SadkwsZhvecQcS9t4vby
9/8X4jS0P8ibfcKS4nBP+dT81kkkg5Z5MohXBORA7VWx+ACohcDEkprsQ+w32xeD
qT1EvQKBgQDKm8ws2ByvSUVs9GjTilCajFqLJ0eVYzRPaY6f++Gv/UVfAPV4c+S0
kAWpXbv5tbkkzbS0eaLPTKgLzavXtQoTtKwrjpolHKIHUz6Wu+n4abfAIRFubOdN
/+aLoRQ0yBDRbdXMsZN/jvY44eM+xRLdRVyMmdPtP8belRi2E2aEzA==
-----END RSA PRIVATE KEY-----
![L13](https://github.com/mizar-0/Cryptonite-JTP-1/blob/main/Images/L13-L14.png)
