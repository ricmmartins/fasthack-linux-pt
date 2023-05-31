# What The Hack - Fundamentos do Linux - Guia do Coach

## Introdução
Bem-vindo ao guia do treinador para o Linux Fundamentals Hackathon. Aqui você encontrará links para orientações específicas para treinadores para cada um dos desafios.

**NOTA:** Se você é um participante do Hackathon, este é o guia de respostas. Não se engane olhando para eles durante o hack! Vá aprender alguma coisa. :)

## Guias do treinador
* Desafio 01: **[Criar uma Máquina Virtual Linux](../Coach/Solution-01.md)**
   - Uma máquina virtual Linux é o pré-requisito para os desafios, então crie uma nova VM Ubuntu Linux
* Desafio 02: **[Manipulação de Diretórios](../Coach/Solution-02.md)**
   - Aprenda a executar operações de diretório comuns, como exibir seu diretório atual e listar o conteúdo do diretório.
* Desafio 03: **[Manipulação de Arquivos](../Coach/Solution-03.md)**
   - Aprenda comandos básicos sobre manipulação de arquivos, como criar, renomear, localizar e remover arquivos.
* Desafio 04: **[Conteúdo do arquivo](../Coach/Solution-04.md)**
   - Aprenda sobre manipulação de conteúdo de arquivo e descubra como contar linhas de arquivo, exibir linhas específicas de um arquivo e muito mais.
* Desafio 05: **[Permissões de arquivo padrão](../Coach/Solution-05.md)**
   - Aprenda sobre as permissões de arquivo padrão do Linux e entenda como trabalhar com permissão de arquivo em um ambiente Linux.
* Desafio 06: **[Gestão de Processos](../Coach/Solution-06.md)**
   - Seus objetivos envolverão gerenciamento de processo básico, como verificar processos em execução e identificar IDs de processo.
* Desafio 07: **[Gestão de Grupos e Usuários](../Coach/Solution-07.md)**
   - Neste desafio você aprenderá sobre a criação de usuários e grupos em um ambiente Linux.
* Desafio 08: **[Scripting](../Coach/Solution-08.md)**
   - Aprenda algumas coisas básicas sobre shell script e o uso de alguns comandos como echo, cut, read e grep.
* Desafio 09: **[Discos, Partições e Sistemas de Arquivos](../Coach/Solution-09.md)**
   - Você trabalhará com discos e partições e aprenderá sobre sistemas de arquivos Linux e comandos como fdisk, mkfs e mount.
* Desafio 10: **[Logical Volume Manager](../Coach/Solution-10.md)**
   - Descubra mais sobre o Logical Volume Manager no Linux e como usar comandos como pvcreate, vgcreate, lvrcreate e muito mais.
* Desafio 11: **[Gerenciamento de Pacotes](../Coach/Solution-11.md)**
   - Aprenda sobre gerenciamento de pacotes e atividades comuns, como atualizar listas de distribuição de pacotes, instalar e desinstalar pacotes.
* Desafio 12: **[Configurando um servidor Web](../Coach/Solution-12.md)**
   - Neste desafio vamos configurar um servidor web e implantar uma aplicação PHP simples nele. O uso de SSL pode ser uma vantagem.
* Desafio 13: **[Protegendo um Servidor](../Coach/Solution-13.md)**
   - Neste desafio vamos descobrir como usar Fail2Ban para proteger serviços em um ambiente Linux.
* Desafio 14: **[Running Containers](../Coach/Solution-14.md)**
   - Seu objetivo neste desafio será criar uma imagem de contêiner a partir de um aplicativo de amostra e executá-la usando o Docker.

## Pré-requisitos do treinador

Este hack tem pré-requisitos que um treinador é responsável por entender e/ou configurar ANTES de hospedar um evento.

O guia cobre as etapas comuns de preparação que um treinador precisa fazer antes do evento.

### Recursos do aluno

Antes do hack, é responsabilidade do Coach garantir que os alunos possam acessar o conteúdo da pasta \`/Student/Resources\`.

## Requisitos do Azure

Esse hack exige que os alunos tenham acesso a uma assinatura do Azure, onde podem criar e consumir recursos do Azure. Esses requisitos do Azure devem ser compartilhados com uma parte interessada na organização que fornecerá as assinaturas do Azure que serão usadas pelos alunos.

- Para o Desafio 01, será necessária uma assinatura do Azure com acesso de colaborador.
- Para todos os outros desafios, será necessário pelo menos um acesso de contribuidor a uma máquina virtual Ubuntu Linux 20.04 pré-criada.
- Para o desafio avançado opcional do Desafio 12, estes são os requisitos:
- Um IP público anexado à máquina virtual
- Acesso ao IP público da máquina virtual
- Acesso ao domínio do Azure App Service para obter um domínio ou acesso ao gerenciamento de DNS de um domínio existente

## Conteúdo do Repositório

- `./Coach/Soluções`
   - Arquivos de solução com respostas de exemplo concluídas para um desafio
- `./Estudante`
   - Guia do Desafio do Aluno
- `./Aluno/Recursos`
   - Arquivos de recursos, código de amostra, scripts, etc. destinados a serem fornecidos aos alunos. (Deve ser embalado pelo treinador e entregue aos alunos no início do evento)
