# Hackathon - Fundamentos do Linux

## Introdução

Este é um recurso de aprendizado criado para ajudar pessoas interessadas a adquirir habilidades em Linux e entender conceitos básicos de linha de comando usando o Azure para construir e aprender. Porém não está restrito ao uso do Azure e você pode executar estre hackathon em qualquer máquina virtual usando o Ubuntu Linux.

<img align="right" src="./Student/resources/images/linuxpenguin.png" width="250"/>

> Nota: Este Hackathon foi incorporado ao Microsoft What The Hack, como o 1º "Hackathon" Linux da Microsoft! Saiba mais em [http://aka.ms/wth](http://aka.ms/wth)

## História do Linux

Linux é uma família de sistemas operacionais de código aberto e livre baseados no kernel Linux. Sistemas operacionais baseados em Linux são conhecidos como distribuições ou distros Linux. Exemplos incluem Debian, Ubuntu, Fedora, CentOS, Gentoo, Arch Linux e muitos outros.

O kernel Linux tem sido desenvolvido ativamente desde 1991 e tem se mostrado extremamente versátil e adaptável. Você pode encontrar computadores que executam Linux em uma ampla variedade de contextos ao redor do mundo, desde servidores web até celulares. Hoje, 90% de toda a infraestrutura em nuvem e 74% dos smartphones do mundo são alimentados pelo Linux.

Para ler mais sobre a história do Linux, distribuições Linux e kernel Linux, [clique aqui](./Student/resources/linux-history.md).


## Objetivos de aprendizado
Neste hack, você será desafiado com algumas tarefas comuns de um cenário do mundo real em tarefas de administração do Linux, tais como:

1. Criar uma Máquina Virtual Linux no Azure
2. Manipular arquivos e diretórios
3. Manipular o conteúdo de arquivos
4. Trabalhar com permissões padrão do Linux
5. Coletar informações sobre processos Linux em seu ambiente
6. Gerenciamento de usuários e grupos
7. Scripting básico de shell
8. Trabalhar com discos, partições e gerenciador de volumes lógicos
9. Gerenciamento de pacotes do Linux
10. Implementar um servidor web básico

## Desafios

Com exceção do desafio 01, que resulta em uma Máquina Virtual Linux necessária para todos os outros desafios, cada desafio pode ser feito separadamente e eles não são interdependentes. O nível de complexidade aumenta de acordo com o número do desafio.

* Desafio 01: **[Criar uma Máquina Virtual Linux](Student/Challenge-01.md)**
  - Uma máquina virtual Linux é um pré-requisito para os desafios, portanto, crie uma nova VM Linux do Ubuntu.
* Desafio 02: **[Manipulação de Diretórios](Student/Challenge-02.md)**
  - Aprenda a realizar operações comuns em diretórios, como exibir o diretório atual e listar o conteúdo do diretório.
* Desafio 03: **[Manipulação de Arquivos](Student/Challenge-03.md)**
  - Aprenda comandos básicos sobre manipulação de arquivos, como criar, renomear, encontrar e remover arquivos.
* Desafio 04: **[Conteúdo de Arquivos](Student/Challenge-04.md)**
  - Aprenda sobre manipulação de conteúdo de arquivos e descubra como contar linhas de arquivo, exibir linhas específicas de um arquivo e muito mais.
* Desafio 05: **[Permissões de Arquivos Padrão](Student/Challenge-05.md)**
  - Aprenda sobre as permissões de arquivo padrão do Linux e entenda como trabalhar com permissões de arquivo em um ambiente Linux.
* Desafio 06: **[Gerenciamento de Processos](Student/Challenge-06.md)**
  - Seus objetivos envolverão o gerenciamento básico de processos, como verificar processos em execução e identificar IDs de processos.
* Desafio 07: **[Gerenciamento de Grupos e Usuários](Student/Challenge-07.md)**
  - Neste desafio, você aprenderá sobre a criação de usuários e grupos em um ambiente Linux.
* Desafio 08: **[Scripting](Student/Challenge-08.md)**
  - Aprenda algumas coisas básicas sobre scripting de shell e o uso de comandos como echo, cut, read e grep.
* Desafio 09: **[Discos, Partições e Sistemas de Arquivos](Student/Challenge-09.md)**
  - Você trabalhará com discos e partições e aprenderá sobre sistemas de arquivos do Linux e comandos como fdisk, mkfs e mount.
* Desafio 10: **[Gerenciador de Volume Lógico](Student/Challenge-10.md)**
  - Descubra sobre o Gerenciador de Volume Lógico no Linux e como usar comandos como pvcreate, vgcreate, lvcreate e mais.
* Desafio 11: **[Gerenciamento de Pacotes](Student/Challenge-11.md)**
  - Aprenda sobre o gerenciamento de pacotes e atividades comuns, como atualizar listas de distribuição de pacotes, instalar e desinstalar pacotes.
* Desafio 12: **[Configurando um Servidor Web](Student/Challenge-12.md)**
  - Neste desafio, vamos configurar um servidor web e implantar uma aplicação PHP simples nele. O uso de SSL pode ser um diferencial.
* Desafio 13: **[Protegendo um Servidor](Student/Challenge-13.md)**
  - Neste desafio, vamos descobrir como usar o Fail2Ban para proteger serviços em um ambiente Linux.
* Desafio 14: **[Executando Containers](Student/Challenge-14.md)**
  - Seu objetivo neste desafio será implantar um contêiner Nginx e acessá-lo. Se você quiser ir mais a fundo, há outra opção de implantar uma aplicação PHP simples.

## Pré-requisitos
- Para rodar este hackathon no Azure e utilizar o Azure Cloud Shell, você irá precisar de uma assinatura do Azure com acesso de colaborador para o Desafio 01 ou acesso de colaborador a uma Máquina Virtual Azure pré-criada para todos os outros desafios. Para executar este hackathon em qualquer outro provedor de nuvem ou mesmo localmente, você precisa apenas de uma máquina virtual com o Ubuntu Linux.
- Acesso a um terminal. Os termos "terminal", "shell" e "interface de linha de comando" são frequentemente usados ​​de forma intercambiável, mas existem diferenças sutis entre eles:

	* Um terminal é um ambiente de entrada e saída que apresenta uma janela somente de texto executando um shell.
	* Um shell é um programa que expõe o sistema operacional do computador a um usuário ou programa. Em sistemas Linux, o shell apresentado em um terminal é um interpretador de linha de comando.
	* Uma interface de linha de comando é uma interface de usuário (gerenciada por um programa interpretador de linha de comando) que processa comandos para um programa de computador e gera os resultados.
Quando alguém se refere a um desses três termos no contexto do Linux, geralmente significa um ambiente de terminal onde você pode executar comandos e ver os resultados impressos no terminal.

		Tornar-se um especialista em Linux requer que você se sinta à vontade ao usar um terminal. Qualquer tarefa administrativa, incluindo manipulação de arquivos, instalação de pacotes e gerenciamento de usuários, pode ser realizada por meio do terminal. O terminal é interativo: você especifica os comandos a serem executados e o terminal gera os resultados desses comandos. Para executar qualquer comando, você o digita no prompt e pressiona ENTER.

		Para nossas atividades, é recomendável usar o [Azure Cloud Shell](http://shell.azure.com/).

- Existem alguns conceitos básicos que serão úteis se você os tiver. Se você quiser dar uma olhada, eles estão [listados aqui](./Student/resources/concepts.md).
- Conceitos sobre o Padrão de Hierarquia do Sistema de Arquivos (FHS) do Linux são recomendados, para que você possa obter mais detalhes sobre isso [aqui](./Student/resources/fhs.md).
- Em relação aos comandos do Linux, apenas como referência, [aqui está](./Student/resources/commands.md) um bom guia de referência rápida.
- As páginas de manual do Linux são suas melhores amigas. Certifique-se de usá-las da melhor maneira possível.

## Recursos de Aprendizado

* [Linux Journey](https://linuxjourney.com/)
* [Linux Upskill Challenge](https://linuxupskillchallenge.org/)
* [Guia para Iniciantes em Linux - Tecmint](https://www.tecmint.com/free-online-linux-learning-guide-for-beginners/)
* [Preparação para o Linux Foundation Certified System Administrator](https://github.com/Bes0n/LFCS)
* [Notas do Linux Foundation Certified System Administrator (LFCS)](https://github.com/simonesavi/lfcs)
* [O Projeto de Documentação do Linux](https://tldp.org/)
* [Introdução ao Linux - do TLPD](https://tldp.org/LDP/intro-linux/intro-linux.pdf)
* [Notas de Comandos do Linux para Profissionais](https://goalkicker.com/LinuxBook/LinuxNotesForProfessionals.pdf)
* [Introdução ao Linux - Curso gratuito da Linux Foundation](https://training.linuxfoundation.org/training/introduction-to-linux/)

## Guia do Instrutor

No diretorio [coach](./Coach/) estão as orientações para caso você esteja executando o Hackathon em um evento e seja um instrutor, assom como também estão as soluções para os desafios propostos. Se você está praticando o Hackathon como estudante, não se engane olhando para as soluções durante o hack! Vá aprender alguma coisa. :)

## Contribuições
Contribuições na forma de erros, solicitações de recursos e PRs são sempre bem-vindas. Siga estas etapas antes de enviar um PR:

* Crie uma issue descrevendo o erro ou solicitação de recurso.
* Clone o repositório e crie um branch de tópico.
* Faça alterações, adicionando novos testes para novas funcionalidades.
* Envie um PR.

## Mostre seu apoio
Dê uma ⭐️ se este conteúdo foi útil para você!

