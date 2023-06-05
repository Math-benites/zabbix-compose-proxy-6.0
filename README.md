<h1 align="center">Zabbix - Compose - Proxy 6.0 </h1>

### Pré-requisitos

Antes de começar, você vai precisar ter instalado 
[Ubuntu 22.04 LTS ](https://releases.ubuntu.com/jammy/)

[Docker Compose version v2.3.3 igual ou superior]

[Docker Engine Version: 23.0.1 igual ou superior]



### 🪓 ( Preparando Estrutura )

```bash
# Criando diretorios
$ mkdir -p /opt/app/
```
```bash
# Acessando diretorio
$ cd /opt/app
```
```bash
# Fazendo Git do projeto
$ git clone https://github.com/Math-benites/zabbix-compose-proxy-6.0.git . 
```

### 🔧 ( Altere as Configuracoes para comecar a usar )

```bash
# Zabbix proxy.config
$ nano ./zabbix/env_vars/.env_prx
``` 

ZBX_SERVER_HOST= IP DO SERVER ZABBIX

ZBX_HOSTNAME = NOME PARA SEU PROXY

### 🎲 ( Rodando Compose )

```bash
$ docker compose up -d
``` 

<p float="left">
 <img src="https://github.com/Math-benites/zabbix-compose-proxy-6.0/blob/main/zabbix/Fotos/Captura%20de%20tela%202023-06-04%20220202.png" width="600" />
<p>

Adicione em ADMINISTRACAO > PROXIES > CRIAR PROXY

Insira em PROXY NAME o nome do seu proxy definido no arquivo .env_prx

Insira em PROXY ADDRESS o ip do seu proxy

