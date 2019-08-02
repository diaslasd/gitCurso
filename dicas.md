### Clone
git clone https://github.com/diaslasd/gitCurso.git

### Proxy git config

```
git config --global http.proxy http://username:password@proxiURL:proxiPort
git config --global https.proxy http://username:password@proxiURL:proxiPort
```

Remover parametro do git config
```
git config --global --unset http.proxy
git config --global --unset https.proxy
```

### Proxy terminal linux

```bash
export HTTP_PROXY='http://username:password@proxiURL:proxiPort'
export HTTPS_PROXY='http://username:password@proxiURL:proxiPort'
```

#### Para tornar esta configuração permanente, há duas formas: 

1. por usuário, usando o usuário logado como exemplo, acrescente a configuração ao arquivo **~/.bashrc**, ou ao arquivo **~/.bash_profile**. 

2. é no sistema, acrescente a configuração no arquivo **/etc/profile**. 

#### Diferença entre .bash_profile e .bashrc
- **.bash_profile** é executado quando é feito o _login_ via _console_ ou _ssh_
- **.bashrc** é executado ao abrir _novo terminal_ o executar o comando _/bin/bash_
- O **~/.bash_profile** seria usado uma vez, no login. O script **~/.bashrc** é lido toda vez que um shell é iniciado

#### A diferença entre su e su –
- scripts de login
```
/etc/profile
~/.bash_profile
/etc/bashrc
~/.bashrc
```
- **su -** todos são executados
- **su** apenas os 2 primeiros são executados

### Special Characters
OnlineConvert
https://unicode-table.com (or) http://unicodelookup.com

Reference: conversion of password **"p@s#w:E"** to unicode will be as follows,
```
@ = %40
$ = %24
# = %23
: = %3A
p@s#w:E = p%40s%23w%3AE
```