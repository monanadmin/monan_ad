# 23 de Fevereiro de 2023

## ATA 002/2023 - Revisão 001

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados da DIMNT"
    
        * Preparado por: Carlos Frederico Bastarz
        * 23 de Fevereiro de 2023
        
        **Coordenação:** João Gerd Zell de Mattos
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 24/02/2023      | <ul> <li> Versão inicial </ul> </li> | 
        | R001    | 27/02/2023      | <ul> <li> Adicionada lista de artigos </li> <li> Revisão geral </li> </ul> | 
    
    === "Participações"
    
        * **INPE:**
          * Carlos Frederico Bastarz
          * Éder Paulo Vendrasco
          * Haroldo Fraga Campos Velho
          * João Gerd Zell de Mattos
          * José Antônio Aravéquia
          * Luiz Fernando Sapucci
          * Renato Galante Negri
          * Sérgio Henrique Ferreira
          * Aurelienne Aparecida Souza Jorge

    === "Registro"
    
        **Local, Data e Hora**
        
        * Plataforma Google Meet
        * 23 de Fevereiro de 2023, das 15:30 horas às 17:00 horas
        
![type:video](https://youtube.com/embed/OkwdL2XrZlc)

## Introdução

João Gerd agradece a presença dos colaboradores e lembra a todos sobre a função e a importância das reuniões mensais do grupo no contexto de desenvolvimento da assimilação de dados para o _Model for Ocean-laNd-Atmosphere predictioN_ ([MONAN](https://monanadmin.github.io/monan_cc_docs/)). Em seguida, apresenta os itens da pauta da reunião. 

## Pauta 

Sobre a pauta reunião, João Gerd cita os seguintes itens: 

1. Preparação do roadmap da assimilação de superfície (continental e oceânica) em 2023;
2. Reinício das tratativas para a elaboração de um plano de trabalho do controle de qualidade dos dados recebidos no CPTEC;
3. Início das tratativas para o fluxo de dados requerido pelo RODAS e a disponibilidade da equipe de pré-processamento do CPTEC;
4. O uso de machine learning na assimilação de dados para a resolução de problemas reais no contexto do INPE;
5. Outros assuntos.

## Pauta 1 - Preparação do roadmap da assimilação de superfície (continental e oceânica) em 2023;

Devido à ausência dos membros Clemente Tanajura e Felipe Costa, João Gerd deixa a discussão desse item a pauta para a próxima reunião do grupo.

## Pauta 2 - Reinício das tratativas para a elaboração de um plano de trabalho do controle de qualidade dos dados recebidos no CPTEC

Sobre este item da pauta, João Gerd comenta sobre alguns dos desenvolvimentos que já se encontram em andamento. Comenta sobre as tratativas iniciadas com a equipe de pré-processamento do CPTEC, liderada pelo Eduardo Barbosa e cita também os trabalhos realizados pelo Sérgio Ferreira. Luiz Sapucci relembra as ações acordadas na última reunião e comenta sobre a necessidade de se concluir a apresentação do Haroldo Fraga. Luiz Sapucci acrescenta que ficou de marcar uma reunião para concluir a apresentação. Sobre este assunto, João Gerd comenta que, a partir da apresentação do Haroldo Fraga, houveram discussões dentro do grupo de assimilação de dados sobre o uso de redes neurais e quais aplicações reais podem ser realizadas. Cita que é necessário começar a aplicar as ideias e os conceitos nos trabalhos do grupo e que devem ser criados subgrupos de trabalho para tratar desse tema com mais detalhes, de forma que as discussões no escopo do grupo atual sejam mais resumidas. Haroldo Fraga faz comentários sobre a sua visão para o estabelecimento da assimilação de dados para o MONAN. Comenta que primeiro, é necessário eleger um método de assimilação de dados e que é necessário conhecer todos os detalhes da sua implementação e todos os seus aspectos. Isso é necessário para que o grupo adquira confiança e saiba quais testes realizar. Acrescenta que, outro aspecto importante, é saber qual dado será assimilado. Questiona se já se sabe qual metodologia de controle de qualidade dos dados será utilizada para a assimilação. Comenta que o problema de não se ter isso definido, é que corre-se o risco de se ter dados e não assimilá-los. Além disso, cita que é necessário também saber como será determinada a matriz dos erros de observação (a matriz dos erros dos sensores). Comenta que os americanos e os europeus possuem uma política de monitoramento e troca de informações sobre a qualidade dos dados. João Gerd comenta que atualmente o CPTEC tem utilizado o sistema _Gridpoint Statitical Interpolation_ ([GSI](https://dtcenter.org/community-code/gridpoint-statistical-interpolation-gsi)) que possui alguns algoritmos de assimilação de dados, dentre eles, o [3DVar](https://twister.caps.ou.edu/OBAN2019/3DVAR.pdf) _First Guess at Appropriate Time_ (FGAT) que está sendo efetivamente utilizado pelo grupo de assimilação de dados. Cita que no futuro próximo, o grupo deverá começar a usar a metodologia 3DEnVar, que considera o _Ensemble Kalman Filter_ ([EnKF](https://en.wikipedia.org/wiki/Ensemble_Kalman_filter)) para atualizar a matriz de covariância dos erros de previsão. 

Outro ponto importante a ser discutido, são as observações. Sobre esse assunto João Gerd comenta sobre a elaboração de um plano de trabalho para o controle de qualidade dos dados recebidos pelo centro. Cita algumas ferramentas com as quais o grupo de assimilação de dados já trabalhou, mas que devido à falta de recursos humanos, tiveram o seu desenvolvimento interrompido (_obsProc_). Em conjunto com o grupo de pré-processamento e banco de dados do centro, está sendo discutido o uso das ferramentas _Interface for Observational Data Access_ ([IODA](https://jointcenterforsatellitedataassimilation-jedi-docs.readthedocs-hosted.com/en/latest/inside/jedi-components/ioda/index.html)) e _Unified Forward Operator_ ([UFO](https://jointcenterforsatellitedataassimilation-jedi-docs.readthedocs-hosted.com/en/latest/inside/jedi-components/ufo/index.html)), que tem a função de padronizar o formato dos dados e realizar o seu controle de qualidade, respectivamente. Sérgio Ferreira pergunta como o software _paqc_ (um software de controle de qualidade das observações em desenvolvimento pelo grupo) pode ser utilizado. João Gerd comenta que é necessário haver linhas de trabalho nestes dois softwares. Acrescenta que a intenção do grupo é adotar o sistema _Joint Effort for Data Assimilation Integration_ ([JEDI](https://jointcenterforsatellitedataassimilation-jedi-docs.readthedocs-hosted.com/en/latest/index.html)), mas que por enquanto, os desenvolvimentos em assimilação de dados são realizados com o GSI. Nesse sentido, os dados provenientes do _paqc_ são efetivamente utilizados pelo GSI para a assimilação e, por esse motivo, esse desenvolvimento não pode ser interrompido. Por outro lado, comenta que é necessário investir nas ferramentas que serão necessárias para o uso do JEDI. 

Outra questão pertinente colocada pelo Sérgio Ferreira é sobre o formato dos arquivos dos dois sistema de controle de qualidade. João Gerd comenta que o GSI trabalha com um formato próprio, o [PrepBUFR](https://www.nco.ncep.noaa.gov/sib/decoders/BUFRLIB/toc/prepbufr/) e que o JEDI utiliza o formato [NetCDF](https://www.unidata.ucar.edu/software/netcdf/). As ferramentas IODA e UFO estão preparadas para ler qualquer formato de arquivo e preparam as observações para o formato utilizado pelo JEDI. Acrescenta que esta discussão está em curso com o Eduardo Barbosa para que seja possível ter ambas as ferramentas em uso. Sérgio Ferreira acrescenta sobre a importância de se discutir um cronograma de trabalho sobre os sistemas e Eduardo Barbosa concorda com a proposição, de forma que ambos os sistemas, GSI e JEDI, possam ser contemplados nos trabalhos do grupo. 

## Pauta 3 - Início das tratativas para o fluxo de dados requerido pelo RODAS e a disponibilidade da equipe de pré-processamento do CPTEC

Devido à ausência dos membros Clemente Tanajura e Felipe Costa, João Gerd deixa a discussão desse item a pauta para a próxima reunião do grupo.

## Pauta 4 - O uso de machine learning na assimilação de dados para a resolução de problemas reais no contexto do INPE

Devido à ausência do membro Haroldo Fraga (que se ausentou da reunião devido a um outro compromisso), as discussões sobre o tema foram postergadas para um momento em que o Haroldo Fraga possa participar também. No entanto, João Gerd sugere que o grupo pense em formas de se utilizar redes neurais para resolver partes específicas do problema de assimilação de dados, e não necessariamente a análise como um todo. Cita como exemplo a utilização de redes neurais dentro do processo de controle de qualidade das observações e solicita a todos que, para a próxima reunião, sejam sugeridas ideias de como as redes neurais podem ser utilizadas dentro das suas especialidades. Luiz Sapucci sugere que reuniões específicas sejam marcadas para que os interessados possam participar e trocar ideias. Sugere também que uma lista de artigos seja enviada para que todos possam se inteirar sobre o que se tem feito atualmente sobre o tema.

Uma lista de artigos sugeridos para a aplicação de redes neurais na assimilação de dados e modelagem:

* [Data assimilation or machine learning?](https://www.ecmwf.int/en/newsletter/167/meteorology/data-assimilation-or-machine-learning)
* [Opportunities and challenges for machine learning in weather and climate modelling: hard, medium and soft AI](https://royalsocietypublishing.org/doi/10.1098/rsta.2020.0083)
* [Machine learning for weather and climate modelling](https://royalsocietypublishing.org/toc/rsta/2021/379/2194?twclid=2-53fyedntpomgduqbxtrlvygem)
* [Neural Networks for Postprocessing Ensemble Weather Forecasts](https://journals.ametsoc.org/view/journals/mwre/146/11/mwr-d-18-0187.1.xml)
* [A Neural-Network Based MPAS—Shallow Water Model and Its 4D-Var Data Assimilation System](https://www.mdpi.com/2073-4433/14/1/157)
* [Statistical modelling of 2m temperature and 10m wind speed forecast errors](https://www.ecmwf.int/sites/default/files/elibrary/2022/20342-statistical-modelling-2m-temperature-and-10m-wind-speed-forecast-errors.pdf)
* [The digital revolution of Earth-system science](https://www.nature.com/articles/s43588-021-00023-0) | ([link](https://drive.google.com/file/d/1EPJ7YVudJnOd1vI537QJt5cWwFo96AcX/view?usp=share_link))

Ainda sobre o tema, José Aravéquia acrescenta que as questões colocadas pelo Haroldo Fraga são muito amplas para serem discutidas no escopo das reuniões do macro grupo de assimilação de dados. Comenta que na Europa e nos Estados Unidos, há centros e entidades organizadas e especializadas no controle e no monitoramento de satélites e do uso de dados de satélites. Cita como exemplos a _European Organisation for the Exploitation of Meteorological Satellites_ ([EUMETSAT](https://www.eumetsat.int/)) na Eurupa e o _National Environmental Satellite, Data, and Information Service_ ([NESDIS](https://www.nesdis.noaa.gov/)) nos Estados Unidos. Acrescenta que, no caso do Brasil, provavelmente o Laboratório de Instrumentação Meteorológica ([LIM](http://lim1.cptec.inpe.br/)) do INPE seja o responsável por cumprir com o papel de prover as informações sobre a calibração e o erro dos instrumentos de medição. Luiz Sapucci concorda com o José Aravéquia e lembra que a Divisão de Satélites e Sistemas Ambientais ([DISSM](http://satelite.cptec.inpe.br)) também tem esse papel em relação aos dados de satélites. Renato Galante concorda com a colocação dos colegas e reforça o papel da DISSM no desenvolvimento de métodos, validação de produtos e na participação de experimentos de campo. Comenta que estas atividades eram mais intensas há alguns anos quando a divisão possuía mais recursos humanos. 

## Outros assuntos

José Aravéquia sugere que, para a próxima reunião, sejam apresentadas demandas de uso de machine learning para que os especialistas da área possam se manifestar sobre como essas demandas podem ser abordadas. Como exemplo, cita a demanda pelo uso de redes neurais para a construção de operadores de observação. Comenta que atualmente as informações relacionadas com os dados de satélites (e.g., viés do ângulo de satélites) são tabelados e fixos e acrescenta que o machine learning pode ser usado para contornar isso, inclusive com melhores resultados. Como um outro exemplo, João Gerd acrescenta que o servidor Eduardo Khamis havia sugerido o artigo [A Neural-Network Based MPAS - Shallow Water Model and Its 4D-Var Data Assimilation System](https://www.mdpi.com/2073-4433/14/1/157) em que redes neurais foram utilizadas para substituir o modelo inverso em uma aplicação de assimilação de dados. Na mesma linha, Carlos Bastarz sugere a todos a participação no _Massive Open Online Course_ ([MOOC](https://lms.ecmwf.int/?redirect=0)) do ECMWF como um primeiro curso prático de machine learning aplicado às ciências atmosféricas, incluindo a assimilação de dados.

## Ações Para a Próxima Reunião 

1. **João Gerd, Eduardo Barbosa e Sérgio Ferreira:** marcar reunião para tratar sobre o planejamento do controle de qualidade dos dados;
2. **João Gerd:** enviar email para os membros do macro grupo DAS-MONAN solicitando demandas pelo uso de inteligência artificial em problemas relacionados com a assimilação de dados;
3. **João Gerd, Clemente Tanajura e Felipe Costa:** dar sequência à preparação do roadmap da assimilação de superfície (continental e oceânica) em 2023;
4. **João Gerd, Haroldo Fraga e interessados:** marcar reunião para tratar das demandas do uso de inteligência artificial em problemas específicos da assimilação de dados;
5. **João Gerd e Luiz Sapucci:** enviar uma lista com artigos sugeridos sobre o tema inteligência artificial;
6. **Todos:** trazer demandas pelo uso de inteligência artificial em suas respectivas especialidades para discussão.
