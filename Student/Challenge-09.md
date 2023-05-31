# Desafio 09 - Discos, Partições e Sistemas de Arquivos

[< Desafio Anterior](./Challenge-08.md) - **[Home](../README.md)** - [Próximo Desafio >](./Challenge-10.md)

## Pré-requisitos

- Crie um disco de dados com o tamanho de 5GB
- Adicione o disco à máquina virtual

## Descrição

Neste desafio, você trabalhará com discos e partições. Será uma oportunidade de aprender sobre sistemas de arquivos Linux e comandos como `fdisk`, `mkfs` e `mount`.

- Identifique o novo disco adicionado à máquina
- Edite a tabela de partições do disco:
    - Adicione uma nova partição com 500MB
    - Liste e identifique a partição criada no sistema operacional
    - Apague a partição
    - Verifique no sistema operacional se a partição foi removida
    - Adicione duas novas partições com uma partição nativa do Linux (83), uma com 500MB e outra com 100MB
    - Verifique no sistema operacional se as partições foram criadas
- Crie um sistema de arquivos em cada uma das partições criadas
- Crie um diretório para cada uma das partições dentro do diretório `/mnt`
- Monte cada uma das partições no respectivo diretório
- Verifique se as partições estão montadas corretamente dentro do sistema operacional
- Escreva arquivos dentro de uma das partições
- Desmonte as partições
- Remova as partições existentes

## Critério de Sucesso

1. Verifique se o disco foi adicionado à máquina virtual
2. Certifique-se de que você criou as partições conforme o esperado
3. Valide em ambas as partições o sistema de arquivos criado
4. Certifique-se de que você criou os respectivos diretórios dentro do diretório `mnt`
5. Verifique se as partições estão montadas corretamente
6. Certifique-se de que você pode criar arquivos nas partições
7. Certifique-se de que você desmontou as partições e as removeu corretamente

## Recursos de Aprendizado

- [Hierarquia de Sistemas de Arquivos](https://linuxjourney.com/lesson/filesystem-hierarchy)
- [Diretório /dev](https://linuxjourney.com/lesson/dev-directory)
- [Como particionar um disco no Linux](https://opensource.com/article/18/6/how-partition-disk-linux)
- [Como listar as partições de disco no Linux](https://www.cyberciti.biz/faq/linux-list-disk-partitions-command/)
- [Como listar as partições de disco no Linux](https://ostechnix.com/how-to-list-disk-partitions-in-linux/)
