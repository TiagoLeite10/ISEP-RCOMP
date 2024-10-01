`RCOMP 2022-2023 Project - Sprint 2 - Member 1210805 folder
`===========================================

# Edificío D

## *VLAN* *database* e rede *IPv4*

![1210805](./imagens/IPv4%20.png)

|              | ID da VLAN | Nome da VLAN | Total de nodes | IP da rede       | Primeiro host | Último host   | Broadcast     | Máscara de sub-rede |
|--------------|------------|--------------|----------------|------------------|---------------|---------------|---------------|---------------------|
| Wi-Fi        | 568        | Dwifi        | 80             | 10.81.150.0/25   | 10.81.150.1   | 10.81.150.126 | 10.81.150.127 | 255.255.255.128     |
| First Floor  | 567        | Dfloorone    | 60             | 10.81.150.128/26 | 10.81.150.129 | 10.81.150.190 | 10.81.150.191 | 255.255.255.192     |
| Ground Floor | 566        | Dgroundfloor | 25             | 10.81.150.192/27 | 10.81.150.193 | 10.81.150.222 | 10.81.150.223 | 255.255.255.224     |
| VoIP         | 570        | Dvoip        | 13             | 10.81.150.224/28 | 10.81.150.225 | 10.81.150.238 | 10.81.150.239 | 255.255.255.240     |
| DMZ          | 569        | Ddmz         | 10             | 10.81.150.240/28 | 10.81.150.241 | 10.81.150.254 | 10.81.150.255 | 255.255.255.240     |

### Justificações Relevantes
- As redes foram organizadas em ordem decrescente de nodes, preenchendo assim o maior número possível de endereços sem eles serem desperdiçados.

- Apesar da distribuição de endereços de rede *IPv4* ser adequada, existem ainda *IP's* que podem ser atribuídos a novos nodes
  que podem ser introduzidos no futuro. Podemos então observar a seguinte contagem de endereços disponíveis em cada *VLAN*:

| VLAN         | Total de nodes disponíveis |
|--------------|----------------------------|
| Wi-Fi        | 46                         |
| First Floor  | 2                          |
| Ground Floor | 5                          |
| VoIP         | 1                          |
| DMZ          | 4                          |


## Simulação no *Packet* *Tracer*
![1210805](./imagens/Edificio_D.png)

### Justificações Relevantes
- A abordagem adotada está conforme o que foi estabelecido no *Sprint 1*.

- Conforme solicitado, a simulação permite a comunicação entre as diferentes *VLANs* e a comunicação com o *ISP*.
  Cada *router* encaminha qualquer endereço desconhecido para o *router* presente no MC e este encaminha para cada edifício
  ou para o *ISP* através de um *modem* *DSL*.

- Todos os *switches* foram configurados para ter o número de portas necessário para estabelecer as conexões especificadas
  no enunciado (portas *FFE* para cabos de fibra óptica e portas *CFE* para cabos de cobre).

- Todas as conexões entre *switches* foram alteradas para o modo trunk, o domínio *VTP* alterado para o domínio fornecido (rc23dig3)
  e o *switch* MC configurado no modo servidor, os restantes foram configurados no modo cliente, permitindo que todos os
  *switches* em todos os edifícios tenham na sua base de dados *VLAN* todas as *VLANs* configuradas.

- O *IP* do *laptop* foi configurado, mas mesmo ao salvar o projeto, ele é apagado. Por isso, é preciso definir sempre que iniciamos o projeto.
  Portanto, esta é uma representação da configuração utilizada para ele:

|           | Gateway     | Endereço IPv4 | Máscara de sub-rede |
|-----------|-------------|---------------|---------------------|
| Laptop1_D | 10.81.150.1 | 10.81.150.2   | 255.255.255.128     |

- Todos os equipamentos que possuem locais para instalação de módulos (como por exemplo, o local do switch onde é possível instalar um módulo PT-SWITCH-NM-1FFE), no caso dos que se encontravam sem qualquer tipo de instalação, foram coladas placas de cobertura de forma a proteger os componentes eletrónicos internos. Estas placas também ajudam a manter o resfriamento adequado ao normalizar o fluxo de ar.

## Configuração de Rede
### *Backbone*
- O *backbone* do *campus* é representado na simulação por meio do *switch* MC_A (correspondente ao principal *cross-connect* do *campus*),
  pelos vários *switches* IC de todos os edifícios do *campus* e pelo *router* do edifício D, uma vez que é o responsável pela comunicação entre os vários edifícios do *campus*.

- Assim como no 1º Sprint, a transmissão de dados para os edifícios foi realizada por meio de uma conexão *inter-cross* *connects*,
  representada pelo *switch* IC_D, pelos *horizontal* *connects*, representados pelos *switches* HC1_D e HC2_D, e destes para os CPs ou dispositivos finais.

- Deve-se notar que as conexões MC-IC, IC-HC, HC-HC, HC-CP foram feitas usando cabo de fibra óptica, sendo necessário o uso
  de adaptadores *FFE* nos *switches* e no *router* R_D, que está conectado a IC_D. A conexão entre os dispositivos finais e os CPs e HCs foi feita usando cabo de cobre.

### Conexão de Internet
- A representação da conexão com a *Internet* é feita através de uma *Cloud*, um *router* *ISP* e um *Modem*, respeitando
  a configuração mostrada na *PL3*. Possui apenas 2 endereços válidos (além dos reservados para identificação de rede e *broadcasting*),
  sendo o primeiro associado ao *router* do *ISP*, e o segundo associado ao *router* *MC*.

### Especificações
- A implementação dos requisitos propostos para o edifício D começa a partir do *switch* com nome de *host* IC_D, que estabelece
  uma conexão com outros dois *switches* representando os andares 0 e 1 (HC1_D e HC2_D, respectivamente).

- Todas as portas que não estão conectadas a dispositivos finais são configuradas no modo *trunk*, sendo o tipo de porta indicado para estabelecer conexões com várias *VLANs*.
  Por outro lado, as portas que se conectam a dispositivos finais são configuradas no modo *access*, uma vez que se conectam apenas a uma única *VLAN*.

- Nas configurações dos dois HC's do edifício, as seguintes VLANs foram associadas aos dispositivos finais:

| VLAN | Dispositivo (exemplo) |
|------|-----------------------|
| 566  | PC1_D                 |
| 567  | PC2_D                 |
| 568  | Laptop1_D             |
| 569  | Server1_D             |
| 570  | ipPhone1_D            |

- Visto que o principal objetivo do *sprint* é apresentar um plano de implementação lógica para a rede e por questões de
  interpretação, optou-se por não apresentar a quantidade total de *nodes* indicados no enunciado.
  Assim, cada dispositivo final apresentado na simulação representa a totalidade dos dispositivos que seriam necessários:

| Dispositivo | Total de nodes |
|-------------|----------------|
| PC1_D       | 60             |
| PC2_D       | 25             |
| Laptop1_D   | 80             |
| Server1_D   | 10             |
| ipPhone1_D  | 13             |

### Pings
- Para confirmar que tudo funciona corretamente, são exibidas várias imagens que mostram o sucesso dos testes de *ping*
  entre dispositivos finais no mesmo edifício e entre edifícios diferentes, incluindo o ISP.

#### Entre o *PC1* e o edifício D
![1210805](./imagens/pings/PC1_D.png)

#### Entre o *PC2* e o edifício D
![1210805](./imagens/pings/PC2_D.png)

#### Entre o *laptop* e o edifício D
![1210805](./imagens/pings/Laptop_D.png)

#### Entre o *server* e o edifício D
![1210805](./imagens/pings/Server_D.png)

#### Entre o *router* e o edifício D
![1210805](./imagens/pings/Router_D.png)

#### Entre o *PC1* do edifício D e os outros edifícios, incluindo o *ISP*
![1210805](./imagens/pings/PC1_outros_D.png)

#### Entre o *PC2* do edifício D e os outros edifícios, incluindo o *ISP*
![1210805](./imagens/pings/PC2_outros_D.png)

#### Entre o *laptop* do edifício D e os outros edifícios, incluindo o *ISP*
![1210805](./imagens/pings/Laptop_outros_D.png)

#### Entre o *server* do edifício D e os outros edifícios, incluindo o *ISP*
![1210805](./imagens/pings/Server_outros_D.png)

#### Entre o *router* do edifício D e os outros edifícios, incluindo o *ISP*
![1210805](./imagens/pings/R_outros_D.png)

### Ficheiros de configuração de *switches* e *routers*
- Os arquivos de configuração de todos os *switches* e *routers* necessários para o correto funcionamento do projeto de
  cabeamento estruturado do edifício E podem ser encontrados neste *link*: [Pasta de ficheiros de configuração](config%20files)

### Tabelas de Roteamento
#### Edifício A MC - R_A (10.81.151.6/25)
| Edifício | Rede           | Máscara         | Próximo *Hop*  |
|----------|----------------|-----------------|----------------|
| A        | 10.81.144.0/23 | 255.255.254.0   | 10.81.151.1    |
| B        | 10.81.148.0/24 | 255.255.255.0   | 10.81.151.2    |
| C        | 10.81.149.0/24 | 255.255.255.0   | 10.81.151.3    |
| D        | 10.81.150.0/24 | 255.255.255.0   | 10.81.151.4    |
| E        | 10.81.146.0/24 | 255.255.255.0   | 10.81.151.5    |
| E        | 10.81.147.0/26 | 255.255.255.192 | 10.81.151.5    |
| Internet | 0.0.0.0/0      | 0.0.0.0         | 121.60.202.181 |

#### Edifício D - R_D (10.81.151.4/25)
| Rede      | Máscara | Próximo *Hop* |
|-----------|---------|---------------|
| 0.0.0.0/0 | 0.0.0.0 | 10.81.151.6   |

#### ISP - R-ISP (15.203.47.93/30) ###
| Rede           | Máscara       | Próximo *Hop*  |
|----------------|---------------|----------------|
| 10.81.144.0/21 | 255.255.248.0 | 121.60.202.182 |