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

![L4-L5](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/ca12ac5d-2522-42bc-8a95-1a9f1a32f6e4)

## Level 5=>6: 
it was only required to use `find ./* -size 1033` to find the next password, even though the problem mentioned other requirements. P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU.

![L5-L6](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/8882669c-f208-4efe-825a-35fe861547f2)

## Level 6=>7: 
used `find` with options `-size` `-user` `-group` and `grep` to find files containing ‘password’
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

![L6-L7 A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/c4c0f305-3df1-45c3-801b-6e98bbc1e6c7)

![L6-L7](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/34338776-2fb8-4a71-aa52-f1583e55eea7)

## Level 7 => Level 8: 
used `cat` to read data.txt, piped the output to `grep` to find the required word
TESKZC0XvTetK0S9xNwm25STk5iWrBvP

![L7-L8](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/cda427b5-981b-4805-ac1a-ec8b5d6de774)


## Level 8 => 9:
`uniq` filters only adjacent matching lines from the file. Hence, the lines need to be sorted before uniq is used.
EN632PlfYiZbn3PhVK3XOGSlNInNE00t

![L8-L9](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/2da5a083-067a-4c25-b562-9ef88eab2367)


## Level9 => Level10:
Used `strings` with `-e s` option to specify ASCII encoding and piped the o/p to `grep ==` . GREP stands for Global Regular Expressions Print.
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

![L9-L10](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/042abead-540d-4f89-9bfc-04f692f51371)


## Level 10=> Level 11: 
`<string> base64` can be used to encode string in base 64. The option `–decode` makes it possible to do the reverse.
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

![L10-L11](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/7f864612-1789-4364-8299-262425785c65)


## Level 11 => 12: 
read man page for `tr`. Had to consult stackexchange to find the exact way to specify a rot13 cipher using `tr`. JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

![L11-L12](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/cc535df6-3c8b-4e62-95ec-6206bc87b972)


# Week 2

## Level 12 => 13: 
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw. Consulted walkthrough. Learnt to decompress compressed files. The required password was obtained after multiple decompressions using `tar`, `bunzip2`, `gunzip`. 

## Level 13 => 14: 
Using the provided ssh private key, bandit14 can be logged into. (pw: fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq)

![L13-L14](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/ec9e2bd2-9553-4cfa-9219-48aaab3f8417)

## Level 14 => 15:
Attempted to establish an `ssh` connection. Failed. On closer inspection, question does not mention anything about `ssh`. Explored other commands and tried to connect. Finally had success using `telnet` and `nc`.

![L14-L15](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/20bb3ec6-f0c0-4202-a151-0801e1add563)

![L14-15A](https://github.com/mizar-0/Cryptonite-JTP-1/assets/76529146/7ff9abe5-1aed-490c-b213-b43a1f8fce20)



