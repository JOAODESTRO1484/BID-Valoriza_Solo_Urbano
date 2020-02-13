### MODELOS DE VALORIZAÇÃO DA INTERVENÇÃO PÚBLICA A NÍVEL MUNICIPAL

O modelo desenvolvido prediz a valorização continua de terrenos próximos a uma obra pública a partir de amostras de preços de mercado. 

Para o desenvolvimento foram utilizados dados dos observatórios de mercado imobiliário levantados antes e depois da obra, utilizando dados próximos e até o limite da evidencia de sua influência.
Depois de realizar o tratamento dos dados brutos, procedeu-se o cálculo do semivariograma e as superfícies de variação para cada época, representando-as em formato RASTER. 

A partir dos dois mapas, determinou-se o “mapas das diferenças”, identificando-se os píxeis com alteração no valor. Foram estabelecidas faixas de valores em função da distância dos imóveis até a obra e estes valores foram introduzidos no plugin para permitir que outros municípios tenham condições de efetuar ou prever a valorização dos imóveis em torno de uma obra similar.

### Guía de usuário

1) Para os cálculos, deverão estar na pasta, os dados referentes a MALHA_URBANA, OBRA_PAVIM_LINHA e o arquivo LOTES.QML (que define automaticamente as cores do temático);

2) Quando o arquivo de MALHA_URBANA contiver muitos lotes, acima de 30.000, recomenda selecionar os lotes próximos a obra, cuidando
	 para a seleção exceder os 300m, afim de diminuir a massa de dados a processar e salvar a seleção como LOTES.SHP;

#### IMPORTANTE: Os arquivos deverão ter o mesmo Sistema de Referencia	Cartográfica - SRC.

Após a copia dos arquivos para os devidos locais, carregar o QGIS e abrir o projeto CALCULO_VALORIZA_SOLO.qgs contido na pasta  c:\BID_Valoriza_Solo_Urbano. Serão mostrados os arquivos conforme figura abaixo. Seguir os próximos passos.

![SLIDE_101](https://user-images.githubusercontent.com/60671104/74444983-69f36680-4e54-11ea-920c-1e256ccce5f6.png)

Ao salvar o arquivo de MALHA_URBANA como LOTES, o temático será carregado, conforme figura abaixo. 

![SLIDE_201](https://user-images.githubusercontent.com/60671104/74446463-afb12e80-4e56-11ea-9b2f-1461cdf89657.png)

Para o cálculo, chamar o plugin:

![SLIDE_301](https://user-images.githubusercontent.com/60671104/74447992-f738ba00-4e58-11ea-83e4-9ce4f540c8ea.png)

1-Selecionar o tipo de OBRA ( como ainda tem-se somente um tipo de obra valorada, então já estará selecionada).

2-Selecionar o arquivo da OBRA.

3-Selecionar o arquivo de LOTES.

4-Dar OK (aguardar resultado do cálculo).

### Primeiro Resultado - Resumo dos Totais Envolvidos: 

> - número de lotes, 

> - área dos lotes, 

> - incremento na valorização e

> - de tributo para uma alíquota de 2%.

![SLIDE_401](https://user-images.githubusercontent.com/60671104/74448430-b55c4380-4e59-11ea-9cf9-0c0919eb0586.png)

### Segundo Resultado - Mapa temático com os intervalos de valores. 

![SLIDE_501](https://user-images.githubusercontent.com/60671104/74449594-89da5880-4e5b-11ea-8ee2-cdfbf84828cf.png)

### Terceiro Resultado - Tabela com campos e dados calculados. 

![SLIDE_601](https://user-images.githubusercontent.com/60671104/74449985-26045f80-4e5c-11ea-86eb-7069dd5cd3c3.png)

Campos:

> - INDFISC : Índice Fiscal do lote.

Serão gerados:

> - AREA : Área do lote.

> - DISTOBRA : distancia do lote até a obra.

> - VALOR : valor da faixa.

> - VALTOT : incremento do valor do lote após a materialização da obra (a ser acrescido ao valor cadastral).

-------------------------------------------------
final do guia do usuário novo
-------------------------------------------------
### Guía de instalação

O roteiro contendo informações com relação ao ambiente e software necessário para a utilização do plugin desenvolvido encontra-se descrito no arquivo MANUAL_BID_VALORIZA.PDF. 
https://github.com/JOAODESTRO1484/BID-Valoriza_Solo_Urbano/blob/master/MANUAL_BID_VALORIZA.pdf

O arquivo BID_VALORIZA_DADOS.rar contem a pasta do plugin e a pasta com dados para a simulação de cálculo.

O plugin roda no QGIS versão 2.18.26.

### Instituições
Prefeitura Municipal de Aracaju, Belo Horizonte e Fortaleza.
Universidade Federal de Santa Catarina - Florianópolis - Brasil

### Autores

•	João Norberto Destro - joaodestro@gmail.com

•	Diego Alfonso Erbas - diegoerba@gmail.com

•	Everton da Silva - everton.silva@ufsc.br
