# Desafio 01 - Criar uma Máquina Virtual Linux

**[Página inicial](../README.md)** - [Próximo Desafio >](./Challenge-02.md)

## Pré-requisitos 

- Uma assinatura ativa do Azure.

## Descrição

Para acompanhar este desafio, você precisará de acesso a um servidor executando um sistema operacional baseado em Linux. Observe que este hackathon foi validado usando um servidor Linux executando o Ubuntu 20.04 ([LTS](https://ubuntu.com/about/release-cycle)), mas os exemplos fornecidos devem funcionar em qualquer distribuição Linux. Veja abaixo os passos a seguir para criar sua Máquina Virtual Linux no Azure e escolha aquela com a qual você está mais familiarizado.

Durante o processo de criação da VM, certifique-se de usar **student** como nome de usuário com privilégios de root sobre a máquina virtual, apenas para facilitar durante os desafios.

### Aviso

Abrir a porta 22 para a internet pública é uma prática ruim. Recomendamos fortemente o uso do Azure Bastion ou a criação de uma regra de NSG que limite o acesso ao endereço IP doméstico do aluno (ou à instância do Azure Cloud Shell).

## Critério de Sucesso

* Verificar se você foi capaz de criar com sucesso sua Máquina Virtual Linux **Ubuntu 20.04**
* Confirmar se você pode acessar por SSH

## Recursos de Aprendizado

* [Criar uma máquina virtual Linux no portal do Azure](https://docs.microsoft.com/pt-br/azure/virtual-machines/linux/quick-create-portal)
* [Criar uma máquina virtual Linux com o Azure CLI](https://docs.microsoft.com/pt-br/azure/virtual-machines/linux/quick-create-cli)
* [Criar uma máquina virtual Linux no Azure com o PowerShell](https://docs.microsoft.com/pt-br/azure/virtual-machines/linux/quick-create-powershell)
* [Conectar-se a uma VM Linux](https://docs.microsoft.com/pt-br/azure/virtual-machines/linux-vm-connect?tabs=Linux)
