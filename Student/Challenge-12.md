# Desafio 12 - Configurando um servidor web

[< Desafio Anterior](./Challenge-11.md) - **[Home](../README.md)** - [Próximo Desafio >](./Challenge-13.md)

## Descrição

Neste desafio, configuraremos um servidor web e implantaremos uma aplicação PHP simples nele. Como um extra, você pode adicionar SSL para atender aos requisitos de segurança.

- Faça o download do aplicativo de exemplo [aqui](./resources/simple-php-app.tar.gz?raw=true) para o seu diretório pessoal
- Extraia o conteúdo do simple-php-app.tar.gz no seu diretório pessoal
- Instale o nginx-core
- Instale o php7.4-fpm
- Configure o Nginx

## Critério de Sucesso

1. Certifique-se de ter o arquivo simple-php-app.tar.gz em seu diretório `~`
2. Mostre o conteúdo do arquivo .tar.gz extraído em seu diretório `~`
3. Certifique-se de ter os pacotes nginx-core e php7.4-fpm instalados
4. Mostre que o Nginx está funcionando corretamente

## Dica

Se você instalar o Ubuntu 18.04 em vez do Ubuntu 20.04, a versão do php-fpm que será instalada será a 7.2 em vez da 7.4. Portanto, certifique-se de configurar corretamente o arquivo de configuração do Nginx.

## Recursos de Aprendizado

- [Como instalar o PHP 7.4 com Nginx no Ubuntu 20.04](https://www.rosehosting.com/blog/how-to-install-php-7-4-with-nginx-on-ubuntu-20-04/)
- [Como instalar o Linux, Nginx, MySQL, PHP (pilha LEMP) no Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-install-linux-nginx-mysql-php-lemp-stack-on-ubuntu-20-04)

## Desafio Avançado
*Se estiver se sentindo confortável e com vontade de fazer mais, tente este desafio adicional!*

- Adicione SSL

_Obs: Para este desafio avançado, você precisará acessar a máquina virtual usando um IP público devido ao uso de um certificado SSL._
