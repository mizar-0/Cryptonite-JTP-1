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

![L4-L5](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/d2dab941-5b6c-47ca-a9b2-4602c5183a3d)


## Level 5=>6: 
it was only required to use `find ./* -size 1033` to find the next password, even though the problem mentioned other requirements. P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU.

![L5-L6](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/e1145df8-6983-487e-b51c-8554515426f9)


## Level 6=>7: 
used `find` with options `-size` `-user` `-group` and `grep` to find files containing ‘password’
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

![L6-L7 A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/bac2339b-38a8-4523-adef-b9bec537c23d)

![L6-L7](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/d6455994-9133-4cd2-8267-fc7089e86645)

## Level 7 => Level 8: 
used `cat` to read data.txt, piped the output to `grep` to find the required word
TESKZC0XvTetK0S9xNwm25STk5iWrBvP

![L7-L8](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/b871f31f-8ac9-4e40-bf46-f90183c6f152)



## Level 8 => 9:
`uniq` filters only adjacent matching lines from the file. Hence, the lines need to be sorted before uniq is used.
EN632PlfYiZbn3PhVK3XOGSlNInNE00t

![L8-L9](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/9e520f3d-4618-40a2-ab95-b697191b63be)



## Level9 => Level10:
Used `strings` with `-e s` option to specify ASCII encoding and piped the o/p to `grep ==` . GREP stands for Global Regular Expressions Print.
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

![L9-L10](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/4e7f5554-2a71-495a-8252-fa90950e945c)



## Level 10=> Level 11: 
`<string> base64` can be used to encode string in base 64. The option `–decode` makes it possible to do the reverse.
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

![L10-L11](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/b289c9b0-1aa0-4fac-a8bf-fc4a03889bb8)



## Level 11 => 12: 
read man page for `tr`. Had to consult stackexchange to find the exact way to specify a rot13 cipher using `tr`. JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

![L11-L12](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/e30d2664-4d8c-44b0-83e9-9249c1fca05e)



# Week 2

## Level 12 => 13: 
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw. Consulted walkthrough. Learnt to decompress compressed files. The required password was obtained after multiple decompressions using `tar`, `bunzip2`, `gunzip`. 

## Level 13 => 14: 
Using the provided ssh private key, bandit14 can be logged into. (pw: fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq)

![L13-L14](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/16acee7c-59dd-4f93-a539-13ef24c5d23e)


## Level 14 => 15:
Attempted to establish an `ssh` connection. Failed. On closer inspection, question does not mention anything about `ssh`. Explored other commands and tried to connect. Finally had success using `telnet` and `nc`. (pw: jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt)

![L14-L15](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/20bb3ec6-f0c0-4202-a151-0801e1add563)

![L14-15A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/7ff9abe5-1aed-490c-b213-b43a1f8fce20)

## Level 15 => Level 16:
Read the man pages for `openssl` and `s_client`. Used `-connect hostname:port`  option and entered password. (pw: JQttfApK4SeyHwDlI9SXGR50qclOAil1)

![L15-L16A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/671cc073-2628-4135-aa58-e8d08b68b0d5)

![L15-L16B](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/cd16ac6c-3b6e-460a-a241-4ef3f1f369bb)

![L15-L16C](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/7a70e376-d6ef-42c2-bbb0-9b06f95880a7)

## Leve16 => Level 17:
