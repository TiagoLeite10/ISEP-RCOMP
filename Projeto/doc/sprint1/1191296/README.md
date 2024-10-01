RCOMP 2022-2023 Project - Sprint 1 - Member 1191296 folder
===========================================

# Edificío E

### Medida do edifício:

- 30m × 30m = 900m²

## Piso 0

### Medida da escala:
- 5m (real) = 124px (escala)

### Medidas efetuadas e informações calculadas:
| Sala   | Comprimento (px) | Largura (px) | Comprimento (m) | Largura (m) | A (m²) | Quantidade de Outlets |
|--------|------------------|--------------|-----------------|-------------|--------|-----------------------|
| E.0.1  | 129              | 129          | 5.2             | 5.2         | 27.04  | 6                     |
| E.0.2  | 281              | 281          | 11.33           | 11.33       | 128.37 | 12*                   |
| E.0.3  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.4  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.5  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.6  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.7  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.8  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.9  | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.10 | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.11 | 165              | 80           | 6.65            | 3.23        | 21.48  | 6                     |
| E.0.12 | 81               | 96           | 3.27            | 3.87        | 12.65  | 0*                    |
*Sala com características especiais

### Plano Esquemático:
![1191296](./imagens/Piso%200.jpg)

### Legenda:
![1191296](./imagens/Legenda%20Piso%200.png)

### Justificações Relevantes:

#### Outlets
- A sala E.0.12 é uma área de armazenamento de um *cross-connect* e *hardware* de infraestrutura de rede, nenhum *outlet* 
  é necessária nesta sala, e o mesmo se aplica às casas de banho e às áreas comuns como *hall* de entrada e corredores.

- A sala E.0.2 tem uma finalidade específica e os únicos *outlets* necessários são dois perto de cada passagem de cabo
  do andar.

- A distribuição dos *outlets* foi feita tendo em conta os locais mais adequados para que o espaço da sala não fosse muito
  comprometido, evitando também a sua colocação perto de portas e de forma a permitir um uso mais fácil da área central da
  sala para trabalhar.

- Ao posicionar os *outlets*, também se considerou que a distância máxima entre eles seria de três metros, para que em qualquer
  parte da sala onde o equipamento do utilizador estivesse, pudesse ser facilmente ligado a um *outlet* com o cabo fornecido.

- A quantidade de *outlets* por sala foi determinada com base numa proporção de 2 *outlets* por cada 10 metros quadrados de área.
  Vale ressalvar que ao passar as marcas de 10 metros quadrados, é feito o arredondamento para o valor dos próximos 10 metros quadrados.
  Para explicar melhor esta situação, consideremos o seguinte exemplo: uma sala que contenha 25m², irá contar com 6 *outlets*, pois temos que
  10m² será 2 *outlets*, 20m² será 4 *outlets*, mas como 25m² está entre os 20m² e os 30m², fazemos o arredondamento para os 30m²,
  ficando então com 6 *outlets*.

- Para realizar a ligação de uma *outlet* ao *CP* correspondente, é feita atráves de passagem de cabos por baixo do chão, 
  até um ponto de saída identificado no plano esquemático.

#### Access Point (AP)
- Devido às dimensões do edifício, foi instalado apenas um *access* *point* no edifício.

- Conectado a um *outlet* por meio de um cabo de cobre *CAT7*, o *Access* *Point* oferece uma cobertura de cerca de 
  50 metros de diâmetro em formato de esfera.

##### Alcance do Access Point
![1191296](./imagens/Piso%200%20AP.jpg)

- Para a determinação do alcance do *access* *point* utilizou-se aproximadamente um diâmetro de 50 m.

#### Consolidation Points (CP)
- Ao todo neste piso colocou-se 3 *Consolidation* *Points*:
  1. Na sala E.0.2, que é responsável por controlar a sala E.0.1 e E.0.2, ficando responsável por 18 outlets; 
  2. Na sala E.0.5, que é responsável por controlar as salas E.0.3, E.0.4, E.0.5, E.0.6 e E.0.7 ficando responsável por 30 outlets; 
  3. Na sala E.0.10, que é responsável por controlar as salas E.0.8, E.0.9, E.0.10 e E.0.11 e pelo *outlet* para o *access* *point*, 
  ficando responsável por 25 outlets.

- A ligação do *HC* com os *CP's* é realizada por baixo do chão (underfloor cable raceway), em que é utilizada fibra ótica para a realização desta ligação, 
  por forma a obtermos maiores velocidades em relação a caso a ligação fosse feita com cabos de cobre CAT7.

#### Horizontal cross-connect (HC)
- Devido à sua ampla cobertura de cerca de 1000 metros quadrados, este piso possui somente um *HC*, mesmo que a área total 
  do edifício seja de apenas 900 metros quadrados.

- O *Horizontal* *cross-connect* está localizado na sala E.0.12 no mesmo armário técnico que o *Intermediate* *cross-connect*.

- O comprimento de cada cabo que sai deste HC é inferior a 90 m, não existindo problemas relacionados com o excesso de comprimento de cabo.

#### Intermediate cross-connect (IC)
- O *IC* recebe a conexão de fibra óptica do *MC* e distribui o sinal para os dois *HC's* deste edifício por meio de cabos de fibra óptica.
Estes dois *HC's* são o que se encontra no piso 0, e o que se encontra no piso 1.

- O *Intermediate* *cross-connect* está localizado na sala E.0.12 no mesmo armário técnico que o *Horizontal* *cross-connect*.

#### Cabos Utilizados e Respetivas Quantidades
- Para conectar os *CP's* aos *outlets* é utilizado o cabo de cobre CAT7.

- Por causa da inexistência de custos associados ao projeto e da possibilidade de alcançar uma transmissão de dados mais 
  rápida, decidiu-se utilizar um cabo de fibra óptica monomodo de 8 fios para interligar o *HC* e os *CP's*, levando em 
  conta também a redundância do sistema.

- Para a ligação do *IC* ao *HC* também utiliza-se fibra ótica monomodo de 8 fios.

##### Cabo de Cobre CAT7
###### Sala E.0.1
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.87                                                             |
| 2         | 11.29                                                            |
| 3         | 7.26                                                             |
| 4         | 9.68                                                             |
| 5         | 5.65                                                             |
| 6         | 7.66                                                             |
| **Total** | 50,41                                                            |

###### Sala E.0.2
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 3.02                                                             |
| 2         | 5.85                                                             |
| 3         | 2.62                                                             |
| 4         | 4.64                                                             |
| 5         | 7.66                                                             |
| 6         | 10.08                                                            |
| 7         | 12.10                                                            |
| 8         | 14.52                                                            |
| 9         | 16.13                                                            |
| 10        | 18.55                                                            |
| 11        | 20.16                                                            |
| 12        | 22.58                                                            |
| **Total** | 137.91                                                           |

###### Sala E.0.3
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 13.10                                                            |
| 2         | 11.29                                                            |
| 3         | 11.49                                                            |
| 4         | 9.48                                                             |
| 5         | 8.87                                                             |
| 6         | 6.85                                                             |
| **Total** | 61.08                                                            |

###### Sala E.0.4
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 9.68                                                             |
| 2         | 11.49                                                            |
| 3         | 8.06                                                             |
| 4         | 9.88                                                             |
| 5         | 5.65                                                             |
| 6         | 7.46                                                             |
| **Total** | 52.22                                                            |

###### Sala E.0.5
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 7.66                                                             |
| 2         | 6.05                                                             |
| 3         | 6.05                                                             |
| 4         | 4.44                                                             |
| 5         | 4.44                                                             |
| 6         | 2.22                                                             |
| **Total** | 30.86                                                            |

###### Sala E.0.6
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 7.66                                                             |
| 2         | 9.48                                                             |
| 3         | 5.85                                                             |
| 4         | 7.86                                                             |
| 5         | 3.23                                                             |
| 6         | 5.24                                                             |
| **Total** | 39.32                                                            |

###### Sala E.0.7
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 11.29                                                            |
| 2         | 12.90                                                            |
| 3         | 9.48                                                             |
| 4         | 11.29                                                            |
| 5         | 7.26                                                             |
| 6         | 9.27                                                             |
| **Total** | 61.49                                                            |

###### Sala E.0.8
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 12.82                                                            |
| 2         | 10.77                                                            |
| 3         | 11.29                                                            |
| 4         | 8.99                                                             |
| 5         | 8.79                                                             |
| 6         | 7.26                                                             |
| **Total** | 59.92                                                            |

###### Sala E.0.9
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 10.08                                                            |
| 2         | 7.86                                                             |
| 3         | 8.27                                                             |
| 4         | 6.25                                                             |
| 5         | 5.85                                                             |
| 6         | 3.83                                                             |
| **Total** | 42.14                                                            |

###### Sala E.0.10
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.06                                                             |
| 2         | 6.45                                                             |
| 3         | 6.45                                                             |
| 4         | 4.64                                                             |
| 5         | 4.03                                                             |
| 6         | 2.02                                                             |
| **Total** | 31.65                                                            |

###### Sala E.0.11
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.06                                                             |
| 2         | 9.88                                                             |
| 3         | 6.25                                                             |
| 4         | 8.47                                                             |
| 5         | 3.83                                                             |
| 6         | 5.85                                                             |
| **Total** | 42.35                                                            |

###### Access Point
| Quantidade de cabo CAT 7 necessário desde o outlet do AP até ao CP |
|--------------------------------------------------------------------|
| 15.12                                                              |

##### Cabo Fibra Ótica
| Ligação                            | Quantidade de cabo fibra ótica monomodo de 8 fios necessário (m) |
|------------------------------------|------------------------------------------------------------------|
| CP da sala E.0.2 até o HC do piso  | 65.52                                                            |
| CP da sala E.0.5 até o HC do piso  | 38.31                                                            |
| CP da sala E.0.10 até o HC do piso | 21.77                                                            |
| IC até ao HC do piso               | 2.42                                                             |
| IC até a saída do edifício         | 3.63                                                             |
| **Total**                          | 131.65                                                           |

#### Gabinetes de Telecomunicações

##### Sala E.0.2
- Considerando que existem 18 *outlets* envolvidos, será necessário instalar **um *patch* *panel* *CAT7*** com 24 portas,
  tendo um tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 2U de *patch* *panels*, adiciona-se outras 2U para os *switches* correspondentes esperados, perfazendo 4U, 
  e um dimensionamento adicional de 100%, perfazendo 8U. O tamanho disponível comercialmente acima de 6U é geralmente 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.0.5
- Considerando que existem 30 *outlets* envolvidos, será necessário instalar **dois *patch* *panels* *CAT7*** com 24 portas cada,
  tendo cada um destes o tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados, perfazendo 6U,
  e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.0.10
- Considerando que existem 25 *outlets* envolvidos, será necessário instalar **dois *patch* *panels* *CAT7*** com 24 portas cada,
  tendo cada um destes o tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados, perfazendo 6U,
  e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.0.12
- Considerando que o *HC* está ligado ao *IC* e a três *CP's* através de cabo de fibra ótica monomodo, é necessário utilizar 
  **um *fiber* *patch* *panel*** para realizar essas conexões, tendo este o tamanho de 1U.

- Como está a ser usado um único *patch* *panel* de 1U, adicionamos outra 1U para o *switch* correspondente esperado, totalizando 2U,
  e um dimensionamento adicional de 100%, perfazendo 4U. O tamanho disponível comercialmente começa em 6U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 6U**.

### Inventário total do Piso 0:
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Access Points                       | 1          |
| Copper Cable CAT7 (m)               | 624.47     |
| Copper Patch Cords (0.5m)           | 120        |
| Copper Patch Cords (5m)             | 72         |
| Copper Patch Panel 1U (24 entradas) | 5          |
| Fiber Optic Cable (m)               | 131.65     |
| Fiber Patch Cords (0.5m)            | 96         |
| Fiber Patch Panel 1U (24 entradas)  | 4          |
| Outlets                             | 73         |
| Telecommunication Enclosure 12U     | 3          |
| Telecommunication Enclosure 6U      | 1          |

## Piso 1

### Medida da escala:
- 5m (real) = 124px (escala)

### Medidas efetuadas e informações calculadas:
| Sala   | Comprimento (px) | Largura (px) | Comprimento (m) | Largura (m) | A (m²) | Quantidade de Outlets |
|--------|------------------|--------------|-----------------|-------------|--------|-----------------------|
| E.1.1  | 245              | 170          | 9.88            | 6.85        | 67.68  | 14                    |
| E.1.2  | 151              | 95           | 6.09            | 3.83        | 23.32  | 6                     |
| E.1.3  | 151              | 95           | 6.09            | 3.83        | 23.32  | 6                     |
| E.1.4  | 232              | 108          | 9.35            | 4.35        | 40.67  | 10                    |
| E.1.5  | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.6  | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.7  | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.8  | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.9  | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.10 | 163              | 95           | 6.57            | 3.83        | 25.16  | 6                     |
| E.1.11 | 150              | 108          | 6.05            | 4.35        | 26.32  | 6                     |
| E.1.12 | 150              | 108          | 6.05            | 4.35        | 26.32  | 6                     |
| E.1.13 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.14 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.15 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.16 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.17 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.18 | 135              | 95           | 5.44            | 3.83        | 20.84  | 6                     |
| E.1.19 | 81               | 46           | 3.27            | 1.85        | 6.05   | 0*                    |
| E.1.20 | 156              | 39           | 6.29            | 1.57        | 9.88   | 0*                    |
*Sala com características especiais

### Plano Esquemático:
![1191296](./imagens/Piso%201.jpg)

### Legenda:
![1191296](./imagens/Legenda%20Piso%201.png)

### Justificações Relevantes:

#### Outlets

- As salas E.1.19 e E.1.20 são áreas de armazenamento que são usadas para abrigar uma *cross-connect* e outro *hardware*
  de infraestrutura de rede, não são necessários *outlets*, e o mesmo se aplica às casas de banho e às áreas comuns como 
  *hall* de entrada e corredores.

- A distribuição dos *outlets* foi feita tendo em conta os locais mais adequados para que o espaço da sala não fosse muito
  comprometido, evitando também a sua colocação perto de portas e de forma a permitir um uso mais fácil da área central da
  sala para trabalhar.

- Ao posicionar os *outlets*, também se considerou que a distância máxima entre eles seria de três metros, para que em qualquer
  parte da sala onde o equipamento do utilizador estivesse, pudesse ser facilmente ligado a um *outlet* com o cabo fornecido.

- A quantidade de *outlets* por sala foi determinada com base numa proporção de 2 *outlets* por cada 10 metros quadrados de área.
  Vale ressalvar que ao passar as marcas de 10 metros quadrados, é feito o arredondamento para o valor dos próximos 10 metros quadrados.
  Para explicar melhor esta situação, consideremos o seguinte exemplo: uma sala que contenha 25m², irá contar com 6 *outlets*, pois temos que
  10m² será 2 *outlets*, 20m² será 4 *outlets*, mas como 25m² está entre os 20m² e os 30m², fazemos o arredondamento para os 30m², 
  ficando então com 6 *outlets*.

- Para realizar a ligação de uma *outlet* ao *CP* correspondente, é feita atráves de passagem de cabos por baixo do chão,
  até um ponto de saída identificado no plano esquemático.

#### Access Point (AP)
- Este piso não conta com a presença de um AP, pois o que se encontra no piso 0 consegue servir este andar.

##### Alcance do Access Point
![1191296](./imagens/Piso%201%20AP.jpg)

- O alcance do Access Point em termos de largura neste piso diminui um pouco devido a que o piso encontra-se um pouco mais 
  acima do AP do piso 0. Se imaginarmos uma esfera colocada no centro do piso 0, podemos observar que o piso 1 ficará num 
  local onde o raio entre o centro do piso 1 e a extremidade da esfera é menor.

#### Consolidation Points (CP)
- Ao todo neste piso colocou-se 5 *Consolidation* *Points*:
  1. Na sala E.1.1, que é responsável por controlar as salas E.1.1, E.1.2 e E.1.3, ficando responsável por 26 outlets; 
  2. Na sala E.1.4, que é responsável por controlar as salas E.1.4, E.1.5 e E.1.6, ficando responsável por 22 outlets; 
  3. Na sala E.1.8, que é responsável por controlar as salas E.1.7, E.1.8, E.1.9 e E.1.10, ficando responsável por 24 outlets; 
  4. Na sala E.1.13, que é responsável por controlar as salas E.1.11, E.1.12, E.1.13 e E.1.16 ficando responsável por 24 outlets; 
  5. Na sala E.0.14, que é responsável por controlar as salas E.0.14, E.0.15, E.0.17 e E.0.18 ficando responsável por 24 outlets.

#### Horizontal cross-connect (HC)
- Este piso só possui um *HC*, pois o edifício tem apenas 900 metros quadrados de área e a norma exige que haja 1 *HC* por 
  cada 1000 metros quadrados de área bruta.

- O *HC* está situado na sala E.1.20, dentro de um armário técnico, pois o cliente indicou que esta sala poderia ser utilizada 
  para abrigar um *cross-connect*, sendo originalmente uma área de armazenamento.

- O comprimento de cada cabo que sai deste HC é inferior a 90 m, não existindo problemas relacionados com o excesso de comprimento de cabo.

#### Cabos Utilizados e Respetivas Quantidades
- Para conectar os *CP's* *aos *outlets* é utilizado o cabo de cobre CAT7.

- Por causa da inexistência de custos associados ao projeto e da possibilidade de alcançar uma transmissão de dados mais
  rápida, decidiu-se utilizar um cabo de fibra óptica monomodo de 8 fios para interligar o *HC* e os *CP's*, levando em
  conta também a redundância do sistema.

- Para a ligação do *IC* ao *HC* também utiliza-se fibra ótica monomodo de 8 fios.

##### Cabo de Cobre CAT7
###### Sala E.1.1
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 4.44                                                             |
| 2         | 2.42                                                             |
| 3         | 7.26                                                             |
| 4         | 5.65                                                             |
| 5         | 3.63                                                             |
| 6         | 8.87                                                             |
| 7         | 7.26                                                             |
| 8         | 5.65                                                             |
| 9         | 11.29                                                            |
| 10        | 9.68                                                             |
| 11        | 7.66                                                             |
| 12        | 13.31                                                            |
| 13        | 11.69                                                            |
| 14        | 9.68                                                             |
| **Total** | 108.69                                                           |

###### Sala E.1.2
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 7.46                                                             |
| 2         | 9.88                                                             |
| 3         | 5.65                                                             |
| 4         | 11.49                                                            |
| 5         | 7.46                                                             |
| 6         | 15.52                                                            |
| **Total** | 57.46                                                            |

###### Sala E.1.3
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 10.48                                                            |
| 2         | 12.50                                                            |
| 3         | 12.10                                                            |
| 4         | 14.52                                                            |
| 5         | 14.11                                                            |
| 6         | 16.53                                                            |
| **Total** | 80.24                                                            |

###### Sala E.1.4
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 12.10                                                            |
| 2         | 10.08                                                            |
| 3         | 10.08                                                            |
| 4         | 8.06                                                             |
| 5         | 8.06                                                             |
| 6         | 6.05                                                             |
| 7         | 6.05                                                             |
| 8         | 4.03                                                             |
| 9         | 4.84                                                             |
| 10        | 2.02                                                             |
| **Total** | 71.37                                                            |

###### Sala E.1.5
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.06                                                             |
| 2         | 11.09                                                            |
| 3         | 6.05                                                             |
| 4         | 9.07                                                             |
| 5         | 4.03                                                             |
| 6         | 7.06                                                             |
| **Total** | 45.36                                                            |

###### Sala E.1.6
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 12.50                                                            |
| 2         | 14.92                                                            |
| 3         | 10.48                                                            |
| 4         | 12.90                                                            |
| 5         | 8.47                                                             |
| 6         | 10.89                                                            |
| **Total** | 70.16                                                            |

###### Sala E.1.7
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 10.89                                                            |
| 2         | 13.31                                                            |
| 3         | 8.87                                                             |
| 4         | 11.29                                                            |
| 5         | 6.85                                                             |
| 6         | 9.27                                                             |
| **Total** | 60.48                                                            |

###### Sala E.1.8
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 6.05                                                             |
| 2         | 8.47                                                             |
| 3         | 4.03                                                             |
| 4         | 6.45                                                             |
| 5         | 2.02                                                             |
| 6         | 4.44                                                             |
| **Total** | 31.46                                                            |

###### Sala E.1.9
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 10.89                                                            |
| 2         | 12.90                                                            |
| 3         | 8.87                                                             |
| 4         | 11.29                                                            |
| 5         | 6.85                                                             |
| 6         | 9.27                                                             |
| **Total** | 60.07                                                            |

###### Sala E.1.10
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 14.92                                                            |
| 2         | 17.34                                                            |
| 3         | 12.90                                                            |
| 4         | 15.32                                                            |
| 5         | 11.29                                                            |
| 6         | 13.31                                                            |
| **Total** | 85.08                                                            |

###### Sala E.1.11
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 20.97                                                            |
| 2         | 18.55                                                            |
| 3         | 18.95                                                            |
| 4         | 16.53                                                            |
| 5         | 16.94                                                            |
| 6         | 14.52                                                            |
| **Total** | 106.46                                                           |

###### Sala E.1.12
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 16.13                                                            |
| 2         | 13.71                                                            |
| 3         | 14.11                                                            |
| 4         | 11.69                                                            |
| 5         | 12.10                                                            |
| 6         | 9.68                                                             |
| **Total** | 77.42                                                            |

###### Sala E.1.13
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 0.60                                                             |
| 2         | 3.02                                                             |
| 3         | 2.62                                                             |
| 4         | 5.04                                                             |
| 5         | 4.64                                                             |
| 6         | 7.06                                                             |
| **Total** | 22.98                                                            |

###### Sala E.1.14
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 4.03                                                             |
| 2         | 1.61                                                             |
| 3         | 6.05                                                             |
| 4         | 3.63                                                             |
| 5         | 8.06                                                             |
| 6         | 5.65                                                             |
| **Total** | 29.03                                                            |

###### Sala E.1.15
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 4.23                                                             |
| 2         | 6.65                                                             |
| 3         | 6.25                                                             |
| 4         | 8.67                                                             |
| 5         | 8.27                                                             |
| 6         | 10.69                                                            |
| **Total** | 44.76                                                            |

###### Sala E.1.16
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 7.46                                                             |
| 2         | 9.88                                                             |
| 3         | 5.44                                                             |
| 4         | 7.86                                                             |
| 5         | 3.43                                                             |
| 6         | 5.85                                                             |
| **Total** | 39.92                                                            |

###### Sala E.1.17
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.67                                                             |
| 2         | 6.25                                                             |
| 3         | 6.65                                                             |
| 4         | 4.23                                                             |
| 5         | 4.64                                                             |
| 6         | 2.22                                                             |
| **Total** | 32.66                                                            |

###### Sala E.1.18
| Outlet    | Quantidade de cabo CAT 7 necessário desde o CP até ao outlet (m) |
|-----------|------------------------------------------------------------------|
| 1         | 8.67                                                             |
| 2         | 11.09                                                            |
| 3         | 6.65                                                             |
| 4         | 9.07                                                             |
| 5         | 4.64                                                             |
| 6         | 7.06                                                             |
| **Total** | 47.18                                                            |

##### Cabo Fibra Ótica
| Ligação                            | Quantidade de cabo fibra ótica monomodo de 8 fios necessário (m) |
|------------------------------------|------------------------------------------------------------------|
| CP da sala E.1.2 até o HC do piso  | 32.46                                                            |
| CP da sala E.1.4 até o HC do piso  | 53.83                                                            |
| CP da sala E.1.8 até o HC do piso  | 38.71                                                            |
| CP da sala E.1.13 até o HC do piso | 21.57                                                            |
| CP da sala E.1.14 até o HC do piso | 13.91                                                            |
| IC do piso 0 até o HC do piso 1    | 8.27                                                             |
| **Total**                          | 168.75                                                           |

#### Gabinetes de Telecomunicações

##### Sala E.1.1
- Considerando que existem 26 *outlets* envolvidos, será necessário instalar **dois *patch* *panels* *CAT7*** com 24 portas cada,
  tendo cada um destes o tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados, perfazendo 6U, 
  e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.1.4
- Considerando que existem 22 *outlets* envolvidos, será necessário instalar **um *patch* *panel* *CAT7*** com 24 portas,
  tendo um tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 2U de *patch* *panels*, adiciona-se outras 2U para os *switches* correspondentes esperados,
  perfazendo 4U, e um dimensionamento adicional de 100%, perfazendo 8U. O tamanho disponível comercialmente acima de 6U é geralmente 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.1.8 - Sala E.1.13 - Sala E.1.14
- Considerando que existem 24 *outlets* envolvidos, será necessário instalar **dois *patch* *panels* *CAT7*** com 24 portas cada,
  tendo cada um destes o tamanho de 1U.

- Como a conexão entre o *HC* e o *CP* é realizada com cabo de fibra ótica monomodo será necessário **um *fiber* *patch* *panel***,
  tendo este o tamanho de 1U.

- Como está a ser usado 3U de *patch* *panels*, adiciona-se outras 3U para os *switches* correspondentes esperados, perfazendo 6U, 
  e um dimensionamento adicional de 100%, perfazendo 12U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 12U**.

##### Sala E.1.20
- Considerando que o *HC* está ligado ao *IC* que encontra-se no piso 0 e a cinco *CP's* através de cabo de fibra ótica monomodo, 
  é necessário utilizar **um *fiber* *patch* *panel*** para realizar essas conexões, tendo este o tamanho de 1U.

- Como está a ser usado um único *patch* *panel* de 1U, adicionamos outra 1U para o *switch* correspondente esperado, totalizando 2U, 
  e um dimensionamento adicional de 100%, perfazendo 4U. O tamanho disponível comercialmente começa em 6U.
  Posto isto, **o tamanho total para este gabinete de telecomunicações será de 6U**.

### Inventário total do Piso 1:
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Copper Cable CAT7 (m)               | 1070.78    |
| Copper Patch Cords (0.5m)           | 216        |
| Copper Patch Cords (5m)             | 120        |
| Copper Patch Panel 1U (24 entradas) | 9          |
| Fiber Optic Cable (m)               | 168.75     |
| Fiber Patch Cords (0.5m)            | 144        |
| Fiber Patch Panel 1U (24 entradas)  | 6          |
| Outlets                             | 120        |
| Telecommunication Enclosure 12U     | 5          |
| Telecommunication Enclosure 6U      | 1          |

## Inventário total do Edifício:
| Equipamento                         | Quantidade | 
|-------------------------------------|------------|
| Access Points                       | 1          |
| Copper Cable CAT7 (m)               | 1695.25    |
| Copper Patch Cords (0.5m)           | 336        |
| Copper Patch Cords (5m)             | 192        |
| Copper Patch Panel 1U (24 entradas) | 14         |
| Fiber Optic Cable (m)               | 300.40     |
| Fiber Patch Cords (0.5m)            | 240        |
| Fiber Patch Panel 1U (24 entradas)  | 10         |
| Outlets                             | 193        |
| Telecommunication Enclosure 12U     | 8          |
| Telecommunication Enclosure 6U      | 2          |

## Informações gerais relevantes e importantes
- *Patch* *Cords* *CAT7* de cobre e fibra óptica necessários para cada gabinete de telecomunicações é igual ao número de 
  portas do patch panel em cada um. *Patch* *cords* devem ter comprimento curto, geralmente 0,5 metros é suficiente.

- Para os *outlets*, devem ser fornecidos *patch* *cords* mais longos, até 5 metros de comprimento.

## Aplicações gerais importante
- Os CP's devem conter junto de cada entrada uma identificação do cabo que está inserido, ou seja, deve ser possível saber 
  a qual sala e outlet pertence aquele cabo lá inserido. Desta forma deve existir uma identificação com o seguinte formato: 
  sala_número_da_outlet, exemplo: E.0.1_1, sabemos que o cabo ligado àquela entrada está a fazer ligação com a outlet número 1 da sala E.0.1.

- Em cada entrada dos HC, deve também estar devidamente identificado o que está lá conectado, se for um cabo direto a uma outlet, 
  deve seguir o mesmo padrã explicado no ponto anterior, caso seja a ligação a um CP, deve existir a identificação da sala à qual 
  aquele cabo está a fazer a ligação, por exemplo, E.0.3.