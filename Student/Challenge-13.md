# Desafio 13 - Protegendo um servidor

[< Desafio Anterior](./Challenge-12.md) - **[Home](../README.md)** - [Próximo Desafio >](./Challenge-14.md)


## Descrição

Em um servidor, especialmente aqueles diretamente expostos à Internet, como servidores web, é muito comum receber milhares de tentativas de autenticação. Se você verificar o arquivo /var/log/auth.log, poderá constatar isso.

Essas tentativas são baseadas em ataques de dicionário, que infelizmente têm sucesso em alguns % dos casos. Você tem certeza de que sua senha e as senhas de todos os usuários do seu sistema são fortes o suficiente para resistir a um ataque desses? É por isso que o uso de chaves SSH é uma alternativa melhor do que a abordagem de usuário/senha para autenticação.

Este desafio abordará algumas opções para minimizar esses problemas:

1. Instale o Fail2Ban
2. Altere a porta SSH padrão
3. Habilite as chaves SSH em vez de usuário/senha

A ideia por trás do Fail2Ban é muito simples: bloquear temporariamente ou permanentemente um IP que tenha executado várias ações indesejadas, como autenticação malsucedida, acesso a uma área restrita, etc. Originalmente, foi desenvolvido para detectar tentativas ilegais de login SSH, mas depois cresceu para se tornar um conjunto de ferramentas facilmente personalizável para reagir rapidamente a eventos registrados nos arquivos de log.

Alterar a porta SSH padrão reduz o número desses ataques. Portanto, para este exercício, vamos alterar a porta de 22 para 2222. Lembre-se de abrir a porta 2222 no seu NSG.

- Instale o pacote fail2ban
- Valide o arquivo de configuração /etc/fail2ban/jail.conf
- Certifique-se de que o Fail2Ban esteja funcionando corretamente
- Faça alterações na porta padrão do SSH e configure chaves SSH

## Critérios de Sucesso

1. Certifique-se de que as listas de distribuição estão atualizadas
2. Garanta a instalação do pacote fail2ban
3. Certifique-se de que o Fail2Ban iniciará automaticamente durante a inicialização da VM
4. Certifique-se de que o Fail2Ban esteja ativado para proteger o serviço SSH
5. Altere a porta padrão do SSH de 22 para 2222
6. Configure chaves SSH para melhorar o método de conexão com o servidor

## Recursos de Aprendizado

- [How Fail2Ban Works to Protect Services on a Linux Server](https://www.digitalocean.com/community/tutorials/how-fail2ban-works-to-protect-services-on-a-linux-server)
- [Using Fail2ban to Secure Your Server](https://www.linode.com/docs/guides/using-fail2ban-to-secure-your-server-a-tutorial/)
- [How to Install and Configure Fail2ban on Ubuntu 20.04](https://linuxize.com/post/install-configure-fail2ban-on-ubuntu-20-04/)
- [Change SSH Port](https://linuxhandbook.com/change-ssh-port/)
- [Configure SSH Key based authentication on a Linux Server](https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server)
- [Set up SSH public key authentication to connect to a remote system](https://kb.iu.edu/d/aews#:~:text=The%20corresponding%20public%20key%20will%20be%20generated%20using,characters%2C%20and%20then%20press%20Enter%20or%20Return.%20)
