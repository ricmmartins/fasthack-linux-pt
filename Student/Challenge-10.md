# Desafio 10 - Logical Volume Manager

[< Desafio Anterior](./Challenge-09.md) - **[Home](../README.md)** - [Próximo Desafio >](./Challenge-11.md)

## Pré-requisitos

- Crie um disco de dados com 5GB
- Adicione-o à Máquina Virtual

## Descrição

Este desafio proporcionará uma compreensão sobre o Gerenciador de Volume Lógico (LVM) no Linux, e conhecimento sobre os comandos `pvcreate`, `vgcreate`, `lvcreate` e mais.

- Crie um Volume Físico (`PV`) com o disco adicionado
- Verifique se o `PV` foi criado
- Crie um Grupo de Volumes (VG) usando o PV criado
- Verifique se o VG foi criado
- Crie um Volume Lógico (LV) usando metade do disco (2,5GB)
- Crie um LV usando 10% do disco (500MB)
- Verifique se os LVs foram criados
- Formate os dois LVs como `ext4`
- Monte os LVs nos diretórios criados anteriormente em `/mnt`
- Redimensione o LV menor para ocupar mais 20% do disco (1GB)
- Verifique:
    - Se o LV foi redimensionado
    - Se houve reflexo no sistema de arquivos
- Redimensione o sistema de arquivos

## Critério de Sucesso

1. Valide a criação do Volume Físico
2. Valide a criação do Grupo de Volumes
3. Valide a criação do Volume Lógico
4. Certifique-se de que ambos os volumes lógicos foram criados com os tamanhos esperados
5. Certifique-se de que ambos os volumes lógicos foram formatados com o sistema de arquivos `ext4`
6. Confirme se ambos os volumes lógicos foram montados corretamente em `/mnt`
7. Mostre o redimensionamento do volume lógico e do sistema de arquivos

## Recursos de Aprendizado

- [LVM (Logical Volume Manager)](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/5/html/deployment_guide/ch-lvm)
- [Guia LVM](https://linuxhandbook.com/lvm-guide/)
- [O que é LVM (Logical Volume Management) e quais são seus benefícios?](https://linuxhint.com/whatis_logical_volume_management/)
- [Tutorial do Linux Logical Volume Manager (LVM)](https://linuxconfig.org/linux-lvm-logical-volume-manager)
- [Guia do iniciante para LVM](https://www.howtoforge.com/linux_lvm)
