# Desafio 02 - Manuseio de diretórios - Guia do Coach

[<Solução anterior](./Solution-01.md) - **[Home](./README.md)** - [Próxima solução >](./Solution-03.md)

## Notas e Orientações
1. Exiba seu diretório atual

`student@vm01:~$ pwd`

```bash
/home/student
```

2. Vá para o diretório pai do diretório atual

`student@vm01:~$ cd ..`

3. Vá para o diretório raiz

`student@vm01:~$ cd /`

4. Listando o conteúdo do diretório raiz

`student@vm01:~$ ls`

```bash
bin boot dev etc home lib lib32 lib64 libx32 mídia perdida+encontrada mnt opt proc root run sbin snap srv sys tmp usr var
```

5. Exibir uma longa lista do diretório raiz

`student@vm01:~$ ls -l`

```bash
total 64
lrwxrwxrwx 1 root root 7 de abril 4 21:39 bin -> usr/bin
drwxr-xr-x 4 root root 4096 4 de abril 21:57 inicialização
drwxr-xr-x 18 root root 4100 7 de abril 01:04 dev
drwxr-xr-x 102 root root 4096 7 de abril 06:18 etc
drwxr-xr-x 4 root root 4096 6 de abril 15:06 home
lrwxrwxrwx 1 root root 7 de abril 4 21:39 lib -> usr/lib
lrwxrwxrwx 1 root root 9 de abril 4 21:39 lib32 -> usr/lib32
lrwxrwxrwx 1 root root 9 de abril 4 21:39 lib64 -> usr/lib64
lrwxrwxrwx 1 root root 10 de abril 4 21:39 libx32 -> usr/libx32
drwx------ 2 root root 16384 4 de abril 21:42 perdido+encontrado
drwxr-xr-x 2 root root 4096 4 de abril 21:39 mídia
drwxr-xr-x 5 root root 4096 6 de abril 16:08 mnt
drwxr-xr-x 5 root root 4096 6 de abril 15:06 opt
dr-xr-xr-x 183 root root 0 7 de abril 00:28 proc
drwx------ 5 root root 4096 6 de abril 15:12 root
drwxr-xr-x 26 root root 940 8 de abril 00:09 executar
lrwxrwxrwx 1 root root 8 de abril 4 21:39 sbin -> usr/sbin
drwxr-xr-x 6 root root 4096 4 de abril 21:41 snap
drwxr-xr-x 2 root root 4096 4 de abril 21:39 srv
dr-xr-xr-x 12 root root 0 7 de abril 00:28 sys
drwxrwxrwt 12 root root 4096 8 de abril 00:00 tmp
drwxr-xr-x 14 root root 4096 4 de abril 21:40 usr
drwxr-xr-x 13 root root 4096 4 de abril 21:41 var
```

6. Fique onde está e liste o conteúdo de ~

`student@vm01:~$ ls ~`

7. Liste todos os arquivos (incluindo arquivos ocultos) em seu diretório pessoal

`student@vm01:~$ ls -al ~`

```bash
total 40
drwxr-xr-x 4 student student 4096 8 de abril 00:12 .
drwxr-xr-x 4 root root 4096 6 de abril 15:06 ..
-rw------- 1 student student 2201 8 de abril 00:09 .bash_history
-rw-r--r-- 1 student student 220 25 de fevereiro de 2020 .bash_logout
-rw-r--r-- 1 student student 3771 25 de fevereiro de 2020 .bashrc
drwx------ 2 student student 4096 6 de abril 15:03 .cache
-rw-r--r-- 1 student student 807 25 de fevereiro de 2020 .profile
drwx------ 2 student student 4096 6 de abril 15:02 .ssh
-rw-r--r-- 1 student student 0 6 de abril 15:05 .sudo_as_admin_successful
-rw------- 1 student student 786 7 de abril 22:10 .viminfo
-rw-rw-r-- 1 student student 252 8 de abril 00:01 .wget-hsts
```

8. Use um único comando para criar a seguinte árvore de diretórios `~/folder1/folder2/folder3` (folder3 é um subdiretório da pasta2 e folder2 é um subdiretório da pasta1)

`student@vm01:~$ mkdir -p ~/pasta1/pasta2/pasta3`

9. Liste recursivamente o conteúdo do seu ~

`student@vm01:~$ ls -R`

```bash
/home/student:
dir1

/home/student/dir1:
dir2

/home/student/dir1/dir2:
dir3

/home/student/dir1/dir2/dir3:
```

10. Encontre os diretórios dentro de sua pasta pessoal

`student@vm01:~$ find ~ -type d`

```bash
/home/student
/home/student/.cache
/home/student/.ssh
/home/student/dir1
/home/student/dir1/dir2
/home/student/dir1/dir2/dir3
```
