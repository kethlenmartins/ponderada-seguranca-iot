# Ponderada de programação - Grupo CIDA
## Segurança em Iot

&emsp;Este repositório contém a ponderada de programação da semana 09 desenvolvida pelo grupo C.I.D.A. Nessa atividade, foi necessário analisar as vulnerabilidades de segurança do projeto desenvolvido e entender como poderiam ser resolvidas, além de elencar os possíveis ataques ao protótipo.

## Vulnerabilidades do projeto e possíveis ataques


|Título do Ataque|Nível do Impacto|Nível de Risco
|----|----|----|
|Hacking do perfil administrador|Alto|Médio|
|Alteração da requisição do dashboard|Alto|Alto|
|Uso de wifi com mesmo ssid no ESP32|Médio|Alto|

#### Risco 1:
&emsp;Qualquer pessoa que descubra ou consiga, de forma maliciosa, os dados e credenciais do perfil administrador, poderá ter controle do sistema inteiro.

#### Risco 2:
&emsp;O servidor possui um armazenamento temporário das medições e não requere os dados diretamente da blockchain, Possibilidade de alteração dos dados de medição que aparecem no dashboard Qualquer pessoa com acesso ao servidor pode realizar esse ataque.

#### Risco 3:
&emsp;Ataques se utilizando de outra rede wi-fi com mesmo ssid podem ter controle dos dados que são enviados ao broker MQTT.

## Contribuições Individuais: 
* **Fernando:-**
* **Giacomo:-**
* **Kethlen: Registro de ataques ao armazenamento temporário do servidor**
* **Lucas: Registro de ataques na requisição e esp, ideação**
* **Nicolas: Registro de ataques ao armazenamento temporário do servidor**
* **Rafaela: Registro de ataques externos ao perfil administrador** 
