# Desafio 05 - Permissões de arquivo padrão - Guia do treinador

[< Solução anterior](./Solution-04.md) - **[Home](./README.md)** - [Próxima solução >](./Solution-06.md)

## Notas e Orientações
1. Como usuário comum (estudante), crie um diretório ~/permissions.

`student@vm01:~$ mkdir ~/permissions`

2. Crie um arquivo chamado `myfile.txt` em `~permissions`.

`student@vm01:~$ touch ~/permissions/myfile.txt`

3. Liste as propriedades do arquivo `/var/log/waagent.log`. Em seguida, copie este arquivo para seu diretório de permissões. Quem é o novo proprietário deste arquivo agora?

`student@vm01:~$ ls -l /var/log/waagent.log`

```bash
-rw-r--r-- 1 root root 192274 Apr 11 17:07 /var/log/waagent.log
```

`student@vm01:~$ cp /var/log/waagent.log ~/permissions/`

`student@vm01:~$ ls -ls ~/permissions/`

```bash
-rw-r--r-- 1 student student      0 Apr  8 14:55 myfile.txt
-rw-r--r-- 1 student student 195022 Apr 11 19:51 waagent.log
```

4. Como root, crie um arquivo chamado `rootfile.txt` no diretório `/home/student/permissions`.

`student@vm01:~$ sudo su`

`root@vm01:/# touch /home/student/permissions/rootfile`

5. Como usuário regular (estudante), verifique a quem pertence este arquivo criado pelo root.

`root@vm01:/# exit`

`student@vm01:~$ ls -l ~/permissions`

```bash
total 4
-rw-rw-r-- 1 student student   0 Apr  8 14:55 myfile.txt
-rw-r--r-- 1 root      root        0 Apr  8 14:58 rootfile
-rw-r--r-- 1 student student 195022 Apr 11 19:51 waagent.log
```

6. Altere a propriedade de todos os arquivos em `/home/student/permissions` para você mesmo (aluno).
`student@vm01:~$ chown student ~/permissions/*`

```bash
chown: changing ownership of '/home/student/permissions/rootfile': Operation not permitted
```

Observe que você não pode se tornar proprietário do arquivo que pertence ao root.

7. Certifique-se de que você (aluno) tem todos os direitos sobre os arquivos dentro de `~`, e outros só podem ler

`student@vm01:~$ find ~ -type d -exec chmod 755 {} \; `

`student@vm01:~$ find ~ -type f -exec chmod 644 {} \; `

```bash
chmod: changing permissions of '/home/student/permissions/rootfile': Operation not permitted
```

Observe que você não pode alterar as permissões do arquivo que pertence ao root.
