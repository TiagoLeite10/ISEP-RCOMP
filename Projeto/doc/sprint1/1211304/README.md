RCOMP 2022-2023 Project - Sprint 1 - Member 1211304 folder
===========================================

# Edificío A

### Medida do edifício:

- 20m × 20m = 400m²

## Piso 0

### Medidas calculadas

| Sala   | Comprimento (px) | Largura (px) | Comprimento (m) | Largura (m) | A (m²) | Outlets |
|--------|------------------|--------------|-----------------|-------------|--------|---------|
| A.0.1  | 174              | 166          | 5.2             | 4.9         | 25.48  | 6       |
| A.0.2  | 118              | 166          | 3.5             | 4.9         | 17.15  | 4       |
| A.0.3  | 156              | 166          | 4.6             | 4.9         | 22.54  | 6       |
| A.0.4  | 166              | 240          | 4.9             | 7.1         | 34.79  | 8       |
| A.0.5  | 195              | 147          | 5.8             | 4.4         | 25.52  | 6       |
| A.0.6  | 195              | 240          | 5.8             | 7.1         | 41.18  | 10      |

### Plano Esquemático
![1211304](./imagens/Piso%200.jpg)

### Alcance do Access Point
![1211304](./imagens/Piso%200%20AP.jpg)

### Legenda
![1211304](./imagens/Legenda%20Piso%200.jpg)

### Justificações Relevantes

#### Construção
- O piso 0 tem uma calha de cabos sob o piso conectada à vala técnica externa.

- Acesso a calha sob o piso está disponível em pontos marcados sobre a planta na imagem abaixo.

- Além disso, passagens para o andar acima estão disponíveis.

- A altura do teto neste piso é de 4 metros. Áreas comuns, como o hall de entrada, casas de banho e escadas,
não requerem outlets.

#### Outlets
- A distribuição dos *outlets* foi feita tendo em conta os locais mais adequados para que o espaço da sala não fosse muito
  comprometido, evitando também a sua colocação perto de portas e de forma a permitir um uso mais fácil da área central da
  sala para trabalhar.

- Ao posicionar os *outlets*, também se considerou que a distância máxima entre eles seria de três metros, para que em qualquer
  parte da sala onde o equipamento do utilizador estivesse, pudesse ser facilmente ligado a um *outlet* com o cabo fornecido.

- A quantidade de *outlets* por sala foi determinada com base numa proporção de 2 *outlets* por cada 10 metros quadrados de área.

- Todos os outlets devem ser considerados como colocados nas paredes, apesar da representação do esquemático.

#### Cabos de cobre
- Todos os cabos de cobre devem ser considerados montados na parede, apesar da representação do esquemático.

#### Access Point
- Devido às dimensões do edifício, não foi instalado um *access* *point* neste andar.

- Conectados a um *outlet* por meio de um cabo de cobre *CAT7*, os *Access* *Points* oferecem uma cobertura de cerca de 
  50 metros de diâmetro em formato circular.

#### Consolidation Points (CP)
- Ao todo neste piso colocou-se 3 *Consolidation* *Points*:
  1. Na sala A.0.4, que é responsável por controlar a sala A.0.1, A.0.2, A.0.3, A.0.5, A.0.6, ficando responsável por 40 outlets; 

- O *underfloor* *cable* *raceway* realiza a ligação do *HC* com os *CP's*.

#### Horizontal cross-connect (HC)
- Este piso só possui um *HC*, pois o edifício tem apenas 400 metros quadrados de área e a norma exige que haja 1 *HC* por 
  cada 1000 metros quadrados de área bruta.

- O *HC* está situado na sala A.0.4, dentro de um armário técnico, pois o cliente indicou que esta sala poderia ser utilizada 
  para abrigar um *cross-connect*, sendo originalmente uma área de armazenamento.

- O comprimento de cada cabo é inferior a 90 m.

### Tipo de cabos Utilizados
- Para conectar os *CP's* aos *outlets* é utilizado o cabo de cobre CAT7.

- Por causa da inexistência de custos associados ao projeto e da possibilidade de alcançar uma transmissão de dados mais 
  rápida, decidiu-se utilizar um cabo de fibra óptica monomodo de 8 fios para interligar o *HC* e os *CP's*, levando em 
  conta também a redundância do sistema.

- Para a ligação do *IC* ao *HC* também se utiliza fibra ótica monomodo de 8 fios.

### Respetivas Quantidades

#### Cabo de Cobre CAT7

##### Outlet

###### Sala A.0.1
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 22.70                                                            |
| 2         | 18.30                                                            |
| 3         | 18.13                                                            |
| 4         | 20.30                                                            |
| 5         | 23.63                                                            |
| 6         | 25.80                                                            |
| **Total** | 128.86                                                           |

###### Sala A.0.2
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 14.10                                                            |
| 2         | 11.43                                                            |
| 3         | 7.73                                                             |
| 4         | 10.40                                                            |
| **Total** | 43.66                                                            |

###### Sala A.0.3
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 9.80                                                             |
| 2         | 7.96                                                             |
| 3         | 7.63                                                             |
| 4         | 2.84                                                             |
| 5         | 3.34                                                             |
| 6         | 8.0                                                              |
| **Total** | 39.57                                                            |

###### Sala A.0.4
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 2.84                                                             |
| 2         | 0.40                                                             |
| 3         | 0.50                                                             |
| 4         | 1.84                                                             |
| 5         | 8.34                                                             |
| 6         | 14.76                                                            |
| 7         | 14.60                                                            |
| 8         | 17.17                                                            |
| **Total** | 60.45                                                            |

###### Sala A.0.5
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 22.0                                                             |
| 2         | 18.37                                                            |
| 3         | 14.24                                                            |
| 4         | 15.64                                                            |
| 5         | 23.21                                                            |
| 6         | 19.98                                                            |
| **Total** | 113.44                                                           |

###### Sala A.0.6
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 23.34                                                            |
| 2         | 20.39                                                            |
| 3         | 21.27                                                            |
| 4         | 22.99                                                            |
| 5         | 28.10                                                            |
| 6         | 28.26                                                            |
| 7         | 31.08                                                            |
| 8         | 34.77                                                            |
| 9         | 35.93                                                            |
| 10        | 37.18                                                            |
| **Total** | 283.31                                                           |

#### Cabo Fibra Ótica

##### Consolidation Point
| CP        | Quantidade de cano fibra ótica monomodo de 8 fios necessário desde o CP até ao HC do piso (m) |
|-----------|-----------------------------------------------------------------------------------------------|
| A.0.4     | 1.90                                                                                          |

##### Horizontal cross-connect
| Quantidade de cabo fibra ótica monomodo de 8 fios necessário desde o HC do piso até ao IC (m) |
|-----------------------------------------------------------------------------------------------|
| 5.52                                                                                          |

#### Gabinetes de Telecomunicações

##### Sala A.0.4
- Considerando que existem 40 *outlets* envolvidos, será necessário instalar dois *patch* *panel* *CAT7* com 24 portas,
  tendo um tamanho de 2U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário um *fiber* *patch* *panel*,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados, perfazendo 6U,
  e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

### Inventário total do Piso 0
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Copper Cable CAT7 (m)               | 669.29     |
| Copper Patch Cords (0.5m)           | 48         |
| Copper Patch Cords (5m)             | 40         |
| Copper Patch Panel 1U (24 entradas) | 2          |
| Fiber Optic Cable (m)               | 7.42       |
| Fiber Patch Cords (0.5m)            | 48         |
| Fiber Patch Panel 1U (24 entradas)  | 1          |
| Outlets                             | 40         |
| Telecommunication Enclosure 12U     | 1          |

## Piso 1

### Medidas calculadas

| Sala   | Comprimento (px) | Largura (px) | Comprimento (m) | Largura (m) | A (m²) | Outlets |
|--------|------------------|--------------|-----------------|-------------|--------|---------|
| A.1.1  | 118              | 240          | 3.5             | 7.1         | 24.85  | 6       |
| A.1.2  | 118              | 240          | 3.5             | 7.1         | 24.85  | 6       |
| A.1.3  | 118              | 240          | 3.5             | 7.1         | 24.85  | 6       |
| A.1.4  | 258              | 240          | 7.7             | 7.1         | 54.67  | 12*     |
| A.1.5  | 184              | 146          | 5.5             | 4.4         | 24.20  | 6       |
| A.1.6  | 194              | 241          | 5.8             | 7.2         | 41.76  | 10      |
| A.1.7  | 194              | 156          | 5.8             | 4.6         | 26.68  | 6       |
* Salas com caracteristicas especiais

### Plano Esquemático
![1211304](./imagens/Piso%201.jpg)

### Alcance do Access Point
![1211304](./imagens/Piso%201%20AP.jpg)

### Legenda:
![1211304](./imagens/Legenda%20Piso%201.jpg)

### Justificações Relevantes:

#### Construção
- A altura do teto neste piso é de 3 metros, no entanto há um teto falso, colocado 2,5
metros do chão, cobrindo todo o piso. O espaço sobre o teto caído é perfeito para instalar
pistas de cabo e pontos de acesso sem fio, este piso não tem pistas de cabos sob o piso.

- Não são necessárias saídas de rede em casas de banho e áreas comuns, como corredores e salões. Em outros lugares, em
cada sala identificada, o número padrão de tomadas de rede por tarifa de área deve ser honrado.

- Nas salas A.1.1, A.1.2, A.1.3, A.1.6 e A.1.7 as calhas que sobem para o teto falso estão montadas no canto superior direito, das respetivas salas, pela vista do esquemático apresentado.

- Na sala A.1.5 as calhas que sobem para o teto falso estão montadas no canto superior esquerdo, das respetivas salas, pela vista do esquemático apresentado.

- Na sala A.1.4 entre os outlets 6 e 7 o cabo de cobre passa por cima da porta (parte-se do principio que aporta tem 2m de altura).

#### Outlets
- A distribuição dos *outlets* foi feita tendo em conta os locais mais adequados para que o espaço da sala não fosse muito
  comprometido, evitando também a sua colocação perto de portas e de forma a permitir um uso mais fácil da área central da
  sala para trabalhar.

- Ao posicionar os *outlets*, também se considerou que a distância máxima entre eles seria de três metros, para que em qualquer
  parte da sala onde o equipamento do utilizador estivesse, pudesse ser facilmente ligado a um *outlet* com o cabo fornecido.

- A quantidade de *outlets* por sala foi determinada com base numa proporção de 2 *outlets* por cada 10 metros quadrados de área.

- Este edifício contém o datacentre (sala A.1.4), contendo também o *MC* para o sistema de cabeamento estruturado.

- Todos os outlets devem ser considerados como colocados nas paredes, apesar da representação do esquemático.

#### Cabos de cobre
- Todos os cabos de cobre devem ser considerados montados na parede, apesar da representação do esquemático.

#### Access Point
- Devido às dimensões do edifício, foi instalado apenas um *access* *point* neste andar.

- Conectados a um *outlet* por meio de um cabo de cobre *CAT7*, os *Access* *Points* oferecem uma cobertura de cerca de 
  50 metros de diâmetro em formato circular.

#### Consolidation Points (CP)
- Ao todo neste piso colocou-se 3 *Consolidation* *Points*:
  1. Na sala A.1.4, que é responsável por controlar a sala A.1.1, A.1.2, A.1.3, ficando responsável por 30 outlets;
  2. Na sala A.1.5, que é responsável por controlar a sala A.1.6, A.1.7 e pelo *outlet* para o *access* *point*, ficando responsável por 23 outlets; 

- O *underfloor* *cable* *raceway* realiza a ligação do *HC* com os *CP's*.

#### Horizontal cross-connect (HC)
- Este piso só possui um *HC*, pois o edifício tem apenas 400 metros quadrados de área e a norma exige que haja 1 *HC* por 
  cada 1000 metros quadrados de área bruta.

- O *HC* está situado na sala A.1.4, dentro de um armário técnico, pois o cliente indicou que esta sala poderia ser utilizada 
  para abrigar um *cross-connect*, sendo originalmente uma área de armazenamento.

- O comprimento de cada cabo é inferior a 90 m.

#### Intermediate cross-connect (IC)
- O *IC* recebe a conexão de fibra óptica do *MC* e distribui o sinal para os dois *HC's* deste edifício por meio de cabos de fibra óptica.

- O *Intermediate* *cross-connect* está localizado na sala A.1.4.

#### Main cross-connect (MC)
- O *MC* recebe a conexão de fibra óptica do exterior e distribui o sinal para os 5 *IC's*, um em cada prédio, por meio de cabos de fibra óptica.

- O *Main* *cross-connect* está localizado na sala A.1.4.

### Cabos Utilizados e Respetivas Quantidades
- Para conectar os *CP's* aos *outlets* é utilizado o cabo de cobre CAT7.

- Por causa da inexistência de custos associados ao projeto e da possibilidade de alcançar uma transmissão de dados mais 
  rápida, decidiu-se utilizar um cabo de fibra óptica monomodo de 8 fios para interligar o *HC* e os *CP's*, levando em 
  conta também a redundância do sistema.

- Para a ligação do *IC* ao *HC* também utiliza-se fibra ótica monomodo de 8 fios.

### Respetivas Quantidades

#### Cabo de Cobre CAT7

##### Outlet

###### Sala A.1.1
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 20.13                                                            |
| 2         | 17.66                                                            |
| 3         | 14.84                                                            |
| 4         | 10.46                                                            |
| 5         | 13.73                                                            |
| 6         | 16.29                                                            |
| **Total** | 93.11                                                            |

###### Sala A.1.2
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 16.09                                                            |
| 2         | 13.62                                                            |
| 3         | 10.56                                                            |
| 4         | 6.85                                                             |
| 5         | 9.69                                                             |
| 6         | 12.38                                                            |
| **Total** | 69.19                                                            |

###### Sala A.1.3
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 11.73                                                            |
| 2         | 9.23                                                             |
| 3         | 6.35                                                             |
| 4         | 2.44                                                             |
| 5         | 5.34                                                             |
| 6         | 7.94                                                             |
| **Total** | 43.03                                                            |

###### Sala A.1.4
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 25.30                                                            |
| 2         | 23.85                                                            |
| 3         | 21.34                                                            |
| 4         | 19.31                                                            |
| 5         | 17.39                                                            |
| 6         | 15.82                                                            |
| 7         | 7.41                                                             |
| 8         | 4.88                                                             |
| 9         | 2.13                                                             |
| 10        | 1.83                                                             |
| 11        | 3.97                                                             |
| 12        | 6.19                                                             |
| **Total** | 149.42                                                           |

###### Sala A.1.5
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 2.28                                                             |
| 2         | 1.83                                                             |
| 3         | 3.97                                                             |
| 4         | 7.50                                                             |
| 5         | 10.97                                                            |
| 6         | 12.50                                                            |
| **Total** | 39.05                                                            |

###### Sala A.1.6
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 14.38                                                            |
| 2         | 12.24                                                            |
| 3         | 12.43                                                            |
| 4         | 14.36                                                            |
| 5         | 14.64                                                            |
| 6         | 17.83                                                            |
| 7         | 19.75                                                            |
| 8         | 23.67                                                            |
| 9         | 25.33                                                            |
| 10        | 27.00                                                            |
| **Total** | 182.0                                                            |

###### Sala A.1.7
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 25.61                                                            |
| 2         | 22.69                                                            |
| 3         | 18.58                                                            |
| 4         | 16.72                                                            |
| 5         | 12.31                                                            |
| 6         | 13.69                                                            |
| **Total** | 109.6                                                            |

##### Access Point
| Quantidade de cabo CAT 7 necessário desde o AP até ao CP (m) |
|--------------------------------------------------------------|
| 7.0                                                          |

#### Cabo Fibra Ótica

##### Consolidation Point
| CP        | Quantidade de cano fibra ótica monomodo de 8 fios necessário desde o CP até ao HC do piso (m) |
|-----------|-----------------------------------------------------------------------------------------------|
| A.1.4     | 3.0                                                                                           |
| A.1.5     | 4.20                                                                                          |
| **Total** | 7.20                                                                                          |

##### Horizontal cross-connect
| Quantidade de cabo fibra ótica monomodo de 8 fios necessário desde o HC do piso até ao IC (m) |
|-----------------------------------------------------------------------------------------------|
| 1.84                                                                                          |

##### Intermediate cross-connect
| Quantidade de cabo fibra ótica monomodo de 8 fios necessário desde o IC até ao MC (m) |
|---------------------------------------------------------------------------------------|
| 3.40                                                                                  |
  
##### Main cross-connect
| Quantidade de cabo fibra ótica monomodo de 8 fios necessário desde o MC até á saida do prédio (m) |
|---------------------------------------------------------------------------------------------------|
| 3.70                                                                                              |

#### Gabinetes de Telecomunicações

##### Sala A.1.4
- Considerando que existem 30 *outlets* envolvidos, será necessário instalar dois *patch* *panel* *CAT7* com 24 portas,
  tendo um tamanho de 2U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário um *fiber* *patch* *panel*,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados,
  perfazendo 6U, e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U.**

##### Sala A.1.5
- Considerando que existem 23 *outlets* envolvidos, será necessário instalar um *patch* *panel* *CAT7* com 24 portas,
  tendo um tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário um *fiber* *patch* *panel*,
  tendo este o tamanho de 1U.

- Como está a ser usado 2U de *patch* *panels*, adiciona-se outras 2U para os *switches* correspondentes esperados,
  perfazendo 4U, e um dimensionamento adicional de 100%, perfazendo 8U. O tamanho disponível comercialmente acima de 6U é geralmente 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U.**

### Inventário total do Piso 1
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Access Points                       | 1          |
| Copper Cable CAT7 (m)               | 692.4      |
| Copper Patch Cords (0.5m)           | 72         |
| Copper Patch Cords (5m)             | 52         |
| Copper Patch Panel 1U (24 entradas) | 3          |
| Fiber Optic Cable (m)               | 15.14      |
| Fiber Patch Cords (0.5m)            | 72         |
| Fiber Patch Panel 1U (24 entradas)  | 2          |
| Outlets                             | 53         |
| Telecommunication Enclosure 12U     | 2          |

## Inventário total do Edifício
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Access Points                       | 1          |
| Copper Cable CAT7 (m)               | 1361.69    |
| Copper Patch Cords (0.5m)           | 120        |
| Copper Patch Cords (5m)             | 92         |
| Copper Patch Panel 1U (24 entradas) | 5          |
| Fiber Optic Cable (m)               | 22.56      |
| Fiber Patch Cords (0.5m)            | 120        |
| Fiber Patch Panel 1U (24 entradas)  | 3          |
| Outlets                             | 93         |
| Telecommunication Enclosure 12U     | 3          |

## Outras informações
* Escala: 168px ⇔ 5m

* Real = [(imagem) * 5] / 168

* Outlets = (Área / 10) * 2

* O número de outlets deve ser sempre arredondado, por cima, para as unidades e no caso do valor resultante ser impar, deve ser subido para o seguinte número par.