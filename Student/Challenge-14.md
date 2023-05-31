# Desafio 14 - Executando Containers

[< Desafio Anterior](./Challenge-13.md) - **[Home](./README.md)**

## Descrição

Containers são unidades executáveis de software nas quais o código do aplicativo é empacotado, juntamente com suas bibliotecas e dependências, de maneira comum para que possa ser executado em qualquer lugar, seja em desktops, infraestruturas tradicionais ou na nuvem.

Para fazer isso, os containers aproveitam uma forma de virtualização do sistema operacional (SO), na qual recursos do SO (no caso do kernel Linux, como os recursos de namespaces e cgroups) são utilizados para isolar processos e controlar a quantidade de CPU, memória e disco que esses processos têm acesso.

Os containers são pequenos, rápidos e portáteis porque, ao contrário de uma máquina virtual, eles não precisam incluir um sistema operacional convidado em cada instância e podem, em vez disso, simplesmente aproveitar os recursos e recursos do sistema operacional host.

Os containers surgiram pela primeira vez há décadas, com versões como FreeBSD Jails e AIX Workload Partitions, mas a maioria dos desenvolvedores modernos se lembra de 2013 como o início da era moderna dos containers com a introdução do [Docker](https://www.docker.com/).

O Docker é uma plataforma para desenvolver, enviar e executar aplicativos. Vamos analisar essa declaração. O Docker permite aos usuários construir novas imagens de container, enviar essas imagens para o Docker Hub e também baixar essas imagens do Docker Hub. O Docker Hub atua como uma biblioteca de imagens de container e hospeda as imagens de container construídas pelos usuários. Também existem algumas alternativas ao Docker, como o [Podman](https://podman.io/).

O Podman é um mecanismo de contêiner sem daemon para desenvolver, gerenciar e executar Contêineres OCI (Open Containers Initiative) no seu sistema Linux. Ao contrário do Docker, o Podman não requer um processo daemon para iniciar e gerenciar contêineres. Essa é uma diferença importante entre os dois projetos.

O Podman busca melhorar algumas das desvantagens do Docker. Por exemplo, o Podman não requer a execução de um daemon como root. Na verdade, os contêineres do Podman são executados com as mesmas permissões do usuário que os iniciou. Isso aborda uma preocupação significativa com a segurança, embora ainda seja possível executar contêineres com permissões de root, se você realmente quiser.

O Podman busca ser uma substituição direta do Docker no que diz respeito à CLI. Os desenvolvedores afirmam que a maioria dos usuários pode simplesmente usar alias docker=podman e continuar executando os mesmos comandos familiares. O formato de imagem de contêiner também é totalmente compatível entre o Docker e o Podman, portanto, os contêineres existentes construídos em arquivos Dockerfile funcionarão com o Podman.

Outra diferença fundamental é que, ao contrário do Docker, o Podman não é capaz de construir imagens de contêiner (a ferramenta [Buildah](https://buildah.io/) é usada para isso). Isso mostra que o Podman não foi projetado para ser monolítico.

Ele lida com a execução de contêineres (entre outras coisas), mas não com a construção deles. O objetivo aqui é ter um conjunto de padrões de contêiner aos quais qualquer aplicativo possa ser desenvolvido para oferecer suporte, em vez de depender de um único aplicativo monolítico como o Docker para executar todas as tarefas.

Este desafio permitirá que você tenha seu primeiro contato com contêineres. Você irá:

- Instalar o tempo de execução do Docker
- Executar um contêiner Nginx
- Acessar o site padrão em sua máquina virtual

Se você quiser tentar um desafio avançado, tente este:

- Faça o download deste aplicativo de exemplo [daqui](/Student/resources/simple-php-app.tar.gz) para o seu diretório pessoal
- Crie um Dockerfile para instalar o Nginx, PHP e executar este aplicativo PHP
- Construa a imagem
- Teste a execução do contêiner
- Publique a imagem no Docker Hub

## Critérios de sucesso

1. Certifique-se de que o tempo de execução do Docker foi instalado com sucesso
2. Garanta que seu contêiner Nginx esteja sendo executado corretamente
3. Acesse o site padrão do Nginx através do IP público de sua máquina virtual

Se você decidiu aceitar o desafio avançado:

1. Certifique-se de que o aplicativo de exemplo tenha sido baixado para a máquina virtual
6. Tenha o aplicativo em execução por meio de um contêiner e acessível pelo navegador
7. Valide que a imagem do contêiner foi publicada no Docker Hub

## Recursos de aprendizagem

- [O que é um container?](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-a-container/)
- [Introdução a Contêineres e Docker](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/container-docker-introduction)
- [Guia do iniciante para Docker - como criar seu primeiro aplicativo Docker](https://www.freecodecamp.org/news/a-beginners-guide-to-docker-how-to-create-your-first-docker-application-cc03de9b639f/)
