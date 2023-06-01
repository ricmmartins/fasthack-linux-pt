
# Challenge 01 - Criar uma Máquina Virtual Linux - Guia do Coach 

\[Home](./README.md)\ - \[Próxima Solução >](./Solution-02.md)\

## Notas e Orientações
 
Para criar a Máquina Virtual Linux Ubuntu 20.04, siga as etapas abaixo usando o Azure CLI no shell da nuvem:

- Crie o grupo de recursos:

\```bash
az group create --name rg-linux-fundamentals --location eastus
\```

- Crie a Máquina Virtual:

\```bash
az vm create \
  --resource-group rg-linux-fundamentals \
  --name myVM \
  --image Canonical:0001-com-ubuntu-server-focal:20_04-lts:latest \
  --admin-username student \
  --generate-ssh-keys
\```

- Conecte-se à máquina virtual:

\```bash
ssh student@[public-ip]
\```
