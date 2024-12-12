# Ponderada de programação - Grupo CIDA
## Segurança em Iot

&emsp;Este repositório contém a ponderada de programação da semana 09 desenvolvida pelo grupo C.I.D.A. Nessa atividade, foi necessário analisar as vulnerabilidades de segurança do projeto desenvolvido e entender como poderiam ser resolvidas, além de elencar os possíveis ataques ao protótipo.

## Vulnerabilidades do projeto e possíveis ataques


|Título do Ataque|Nível do Impacto|Nível de Risco
|----|----|----|
|Hacking do perfil administrador|Alto|Médio|
|Alteração da requisição do dashboard|Alto|Alto|
|Uso de wifi com mesmo ssid no ESP32|Médio|Alto|

### Definição e detalhamento de cada ataque

#### Risco 1:
- Qualquer pessoa que descubra ou consiga, de forma maliciosa, os dados e credenciais do perfil administrador, poderá ter controle do sistema inteiro.

#### Risco 2:
- O servidor possui um armazenamento temporário das medições e não requere os dados diretamente da blockchain, Possibilidade de alteração dos dados de medição que aparecem no dashboard Qualquer pessoa com acesso ao servidor pode realizar esse ataque.

#### Risco 3:
- Ataques se utilizando de outra rede wi-fi com mesmo ssid podem ter controle dos dados que são enviados ao broker MQTT.

## Plano de ação:

#### Risco 1: 
- Implementar autenticação em 2 fatores para maior segurança do perfil administrador do sistema.

#### Risco 2:
- Alteração da lógica para retirar os dados diretamente da blockchain em vez de utilizar um armazenamento temporário.

#### Risco 3:
- Verificar o endereço MAC, pois ele é único, independentemente do ssid de redes diferentes ser igual.

## Contribuições Individuais: 
* **Fernando: Não participou/agregou à discussão em grupo**
* **Giacomo: Não participou/agregou à discussão em grupo**
* **Kethlen: Registro de ataques ao armazenamento temporário do servidor**
* **Lucas: Registro de ataques na requisição e esp, ideação**
* **Marcelo: Registro de ataques externos ao perfil administrador**
* **Nicolas: Registro de ataques ao armazenamento temporário do servidor**
* **Rafaela: Registro de ataques externos ao perfil administrador** 
