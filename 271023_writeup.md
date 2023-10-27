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
read man page for `tr`. Had to consult stackexchange to find the exact way to implement a rot13 cipher using `tr`. JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

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

## Level 16 => Level 17:
using `nmap -p 31000-32000 localhost -sV` to scan for open ports in the given range with `service` option, port 31790 was found to satisfy the given criteria.

![L16-17A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/e2ac9c34-3024-45fd-b5e9-55216d22b7bc)


As required, current level pw was submitted to the prompt obtained from `openssl s_client -connect localhost:31790` which led to an RSA Private Key. 

![L16-17B](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/63a218ee-631b-4854-a1a2-f81d9041aa8f)

Saved the RSA private key. Tried to `ssh` into bandit17. Permissions 0644 too open error was thrown. 
Changed the permissions to `600` which is the required mode for SSH Private Keys.
`chmod 600 L17.private`

![L16-17C](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/d1147bcd-72a7-4cc8-a45f-c94866d6c844)

![L16-17D](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/57bb5142-b43c-4985-a88a-795fc7c0648a)

## Level 17 => Level 18:
used `diff` to find the required line. As writeen in the prompt, we get a byebye message.(pw: )

![L17-L18](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/a98456a4-048e-4077-8841-583b5b285afe)

![L17-18B](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/354c545f-4236-4441-83c0-eb903f540d5b)

## Level 18 => Level 19
Consulted walkthrough. `ssh` usually works by allocating a pseudoterminal on the remote server, which triggers the `.bashrc` file.
It is given that `.bashrc` has been modified to close our ssh connection as soon as it is established. Therefore we run the commands `ls` and `cat` directly with the `ssh` command so the `.bashrc` file is not triggered. (pw: awhqfNnAbc1naukrpqDYcF95h7HoMTrC)

![L18-L19](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/ab31f6cc-8073-4e0f-9dd5-c73adee163e5)

## Level 19 => Level 20
As seen below, the execution bit for the given binary has been replaced with an `s` which makes it a setuid binary. This means that running a command with this binary will elevate our privileges to the privileges of the owner for the command that follows. (pw: VxCazJaVykI6W36BkBU0mJTCM8rR95XT)
[Why use `./` to run an executable](https://www.baeldung.com/linux/execute-file-using-dot-slash)

![L19-L20](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/7cc00b35-aa7a-40ab-9d20-9b5a490769df)

## Level 20 => Level 21
Consulted walkthrough. In this level, we set up a server on one terminal by asking `nc` to listen on a random port.Then, using the binary file on another terminal,  we establish a connection with said port on localhost. Through the first terminal we send the pw for current level to suconnect which verifies and returns the next pw.(pw: NvEJF7oVjkddltPSrdKEFOllh9V1IBcq)

![L20-21A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/2a42943a-f96f-4d32-8b55-4b5600ceddd4)

![L20-21B](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/a137db97-fa90-479a-888a-1d56ad122b85)

## Level 21 => Level 22



