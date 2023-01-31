# 26 de Janeiro de 2023

## ATA 001/2023 - Revisão 001

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados da DIMNT"
    
        * Preparado por: Carlos Frederico Bastarz e Luiz Fernando Sapucci
        * 26 de Janeiro de 2023
        
        **Coordenação:** Luiz Fernando Sapucci
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 27/01/2023      | <ul> <li> Versão inicial </ul> </li> | 
        | R001    | 31/01/2023      | <ul> <li> Pequenos ajustes de normalização </ul> </li> | 
    
    === "Participações"
    
        * **INPE:**
          * Carlos Frederico Bastarz
          * Kleber Naccarato
          * Éder Paulo Vendrasco
          * Haroldo Fraga Campos Velho
          * João Gerd Zell de Mattos
          * José Antônio Aravéquia
          * Luciana Mira
          * Luiz Fernando Sapucci
          * Liviany Viana
          * Natália Ruddorf 
          * Renato Galante Negri
          * Sérgio Henrique Ferreira
        * **UFBA:**
          * Clemente Augusto Souza Tanajura
          * Felipe Bittencourt Costa

    === "Registro"
    
        **Local, Data e Hora**
        
        * Plataforma Google Meet
        * 26 de Janeiro de 2023, das 15:30 horas às 17:00 horas
        
![type:video](https://youtube.com/embed/dXW9ji1ub1o)

## Introdução

Luiz Sapucci inicia a reunião desejando a todos um bom início de ano. Anuncia a inclusão de dois novos membros da assimilação oceânica, [Felipe Bittencourt Costa](http://lattes.cnpq.br/5110599960453359) e [Clemente Augusto Souza Tanajura](http://lattes.cnpq.br/0765423133125301), ambos pesquisadores da Universidade Federal da Bahia ([UFBA](https://www.ufba.br/)). Aproveita a oportunidade para apresentar para os novos membros como o grupo de trabalho está organizado, com a participação de membros de outras divisões dentro do INPE. Comenta que as atas são registradas e algumas reuniões são gravadas. O grupo discute os desenvolimentos pertinentes à assimilação de dados, com foco para os desenvolvimentos do MONAN. 

Clemente Tananjura agradece a oportunidade de participação nas atividades do grupo, comenta sobre a importância da colaboração com INPE, tendo em vista o tamanho do seu grupo na UFBA. Comenta que o grupo dele tem trabalhado com métodos como Interpolação Ótima ([_Optimun Interpolation_ - OI](https://glossary.ametsoc.org/wiki/Optimum_interpolation#:~:text=Commonly%20known%20as%20OI%2C%20this,by%20a%20NWP%20model%20forecast.)), _Ensemble OI_ ([EnOI](http://www.cmar.csiro.au/staff/oke/pubs/Oke_et_al_2010_EnOI.pdf)) e que o objetivo é trabalhar com o _Enssemble Kalman Filter_ ([EnKF](https://en.wikipedia.org/wiki/Ensemble_Kalman_filter)) para a assimilação de dados oceânicos e que a colaboração com INPE deve viabilizar essa atividade. Comenta também que o grupo já possui acesso à máquina [Egeon](https://en.wikipedia.org/wiki/Ensemble_Kalman_filter) do CPTEC e que as atividades iniciais de desenvolvimento no novo ambiente já estão em curso. Luiz Sapucci complementa dizendo que o ambiente do grupo é propício para a troca de ideias, informações e também para a resolução de problemas práticos relacionados com os trabalhos em desenvolvimento.

## Pauta 

Sobre a pauta reunião, Luiz Sapucci cita os seguintes itens: 

1. Aspectos técnicos da assimilação na DIMNT;
1. Planejamento das atividades para 2023 e atualização dos planos de trabalho na DIMNT;
1. Status do processo de operacionalização da assimilação de dados atmosféricos no CPTEC;
1. Relatório dignóstico do SMNA V2.3.1 (pré-operacional);
1. Macrogrupo de dados de satélite para modelagem;
1. Status da implementação da assimilação de dados oceânica na Egeon;
1. Assimilação de dados utilizando Inteligência Artificial.

## Pauta 1 - Aspectos técnicos da assimilação de dados na DIMNT

José Aravéquia comenta sobre o trabalho em curso relacionado com a verificação da funcionalidade da inicialização do sistema _Gridpoint Statistical Interpolation_ ([GSI](https://dtcenter.org/community-code/gridpoint-statistical-interpolation-gsi)), componente de assimilação de dados do Sistema de Modelagem Numérica e Assimilação de Dados (SMNA). Cita que tem trabalhado com o sistema na máquina Egeon, realizando testes com o compilador Intel e que alguns problemas foram encontrados, incluindo problemas relacionados ao paralelismo. Acrescenta que os problemas encontradas não ocorrem com o compilador GNU e que este é um indicativo de que os problemas encontrados podem estar relacionados com a forma com que o paralelismo está implementado. Luiz Sapucci comenta que, embora o compilador Intel seja uma alternativa interessante devido ao desempenho ser melhor em comparação com o compilador GNU, parece coerente que possamos avançar na utilização da inicialização na assimilação usando a versão GNU e depois, oportunamente, procuraremos ajustar esse desenvolvimento para a versão Intel. José Aravéquia acrescenta que nem sempre isso é verificado e que, no caso do GSI, as diferenças de desempenho no tempo de processamento da análise, segundo os testes que realizou, não são grandes, portanto pode-se concluir que a melhor alternativa seja avançar mesmo com o método de inicialização no GSI com o compilador GNU.

Éder Vendrasco comenta sobre os desenvolvimentos relacionados com o pacote [`readDiag`](https://github.com/GAD-DIMNT-CPTEC/readDiag). Comenta que já fez algumas modificações no pacote para incluir alguns novos tipos de figuras (e.g., diagrama de Hovmöller) que permitem outros tipos de diagnósticos da assimilação de dados sejam feitos. Luiz Sapucci comenta que este é um trabalho importante, pois irá permitir que alguns desenvolvimentos realizados anteriormente sejam integralizados à versão atual do pacote `readDiag`. Luiz Sapucci sugere que alguns resultados sejam apresentados na próxima reunião do grupo DAS-DIMNT, ao que Éder Vendrasco concordou.

Sérgio Ferreira comenta sobre os desenvolvimentos realcionados com a implementação do pacote `BFGE` que prepara os dados para a assimilação utilizando os dados recebidos pelo CPTEC. Sérgio comenta que realizou com sucesso a compilação do pacote na máquina Egeon utilizando a [`bufrlib`](https://github.com/NOAA-EMC/NCEPLIBS-bufr) do _National Centers for Environmental Predictions_ ([NCEP](https://www.weather.gov/ncep/)). Sobre os testes realizados, cita que faltavam os dados não convencionais, mas que o Eduardo Barbosa disponibilizou os dados que estavam faltando. Cita que na Egeon os dados são gerados utilizando 1 nó na máquina (com 96 cores) e que o tempo de processamento dos dados observacionais leva menos do que 1 minuto. Comenta sobre o tempo de processamento de outros dados e dá outras informações. Luiz Sapucci comenta que esse é um processo importante e que é muito bom ter ele funcionando na Egeon. 

## Pauta 2 - Planejamento das atividades para 2023

Luiz Sapucci comenta que o Saulo Freitas não pôde participar da reunião por estar de licença. Cita que o Saulo Freitas solocitou que fosse feito o planejamento das atividades para 2023. Luiz Sapucci apresenta o roadmap do SMNA para a operação e comenta que o planejamento das atividades deverá ser feito de acordo com este planejamento. Cita que há três entregas da assimilação para a Divisão de Previsão de Tempo e Clima ([DIPTC](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct/divisao-de-previsao-de-tempo-e-clima-diptc)) e que estas versões incluem aprimoramentos importantes como a ampliação da base de dados, a aplicação de uma nova matriz de covariâncias e a assimilação de dados de superfície continental. Luiz Sapucci sugere e todos concordaram que é melhor retirar a versão da assimilação de superfície continental do readmap e preparar um outro documento específico sobre o planejamento da assimilação nas componentes de superfície continental e oceânica. Em relação à assimilação de dados oceânicos, Clemente Tanajura comenta que os desenvolvimentos estão no início que o estágio atual inclui a adaptação dos códigos para a máquina Egeon. Comenta que houve dificuldades para obter as contas de acesso, o que acarretou em alguns atrasos, mas que em breve proporão um cronograma de entregas. Cita que o objetivo é ter o mesmo domínio do modelo _Weather Research & Forecast_ ([WRF](https://www.mmm.ucar.edu/models/wrf)) sobre a parte oceânica. Luiz Sapucci comenta que é importante ter um planejamento de forma que seja possível ter uma expectativa de entregas e que permita que a chefia da Divisão de Modelagem Numérica do sistema Terrestre - ([DIMNT](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct/divisao-de-modelagem-numerica-do-sistema-terrestre-dimnt)) possa dar os meios necessários para o desenvolvimento dos trabalhos. Clemente Tanajura complementa dizendo que o EnKF deverá fazer parte desse planejamento, mas que será necessário contabilizar de forma criteriosa o seu custo computacional.
 
Luiz Sapucci comenta também sobre um plano que a DIMNT tem para implementar um sistema de gestão de atividades. Cita que o planejamento das atividades do grupo já deverá ser compatível com este sistema. 

## Pauta 3 - Status da operacionalização da assimilação de dados atmosféricos no CPTEC

Luiz Sapucci convida o João Gerd para fazer um relato sobre as atividades relacionadas com a implementação operacional do SMNA no CPTEC. João Gerd comenta sobre o problema de utilização dos dados a serem assimilados no ambiente operacional. Segundo ele, a versão do SMNA entregue para a DIPTC não utilizava os dados operacionais, mas uma solução já foi viabilizada pelo grupo de assimilação de dados e pré-processamento. Cita como principal problema do processo, a morosidade da DIPTC para consolidar a versão entregue no ambiente operacional. Comenta que já foi realizado um ciclo completo de assimilação de dados no ambiente, mas que esse ciclo ainda não entrou na rotina de realização dos modelos e sistemas operacionais do centro. Luiz Sapucci comenta também sobre a demora por parte daquela divisão na assinatura do documento de comprometimento de implementação operacional da assimilação de dados. Como justificativa, a DIPTC reportou que o documento não reflete as suas próprias necessidades, embora sejam eles próprios um dos autores. Apesar dos problemas recorrentes, Luiz Sapucci conclui que o importante é que esse processo está em andamento. De forma realista, João Gerd comenta que a sua expectativa é a de que a versão operacional do SMNA (i.e., o SMNA realizado de forma rotineira no ambiente operacional), deverá ficar pronta em março de 2023.

## Pauta 4 - Relatório dignóstico do SMNA V2.3.1 (pré-operacional)

Luiz Sapucci comenta sobre o relatório da versão V2.3.1 do SMNA com os diagnósticos dos desenvolvimentos realizados. Cita as diferentes componentes envolvidas na avaliação diagnóstica, entre elas, o desenvolvimento da matriz de covariâncias dos erros de previsão, a minimização da função custo variacional, a assimilação dos dados de radiâncias e a avaliação do desempenho do modelo BAM nas previsões a partir das análises do sistema GSI. 

Sobre o desenvolvimento da matriz de covariâncias dos erros de previsão do modelo, Carlos Bastarz comenta sobre os desenvolvimentos realizados. Cita que a matriz que está apresentada no relatório, já considera as previsões do modelo BAM em coordenada híbrida. Explica para os colegas que é utilizado o método _National Modeling Center_ ([NMC](https://www.ecmwf.int/sites/default/files/elibrary/2003/9404-background-error-covariance-modelling.pdf)), que utiliza pares de previsões de 24 e 48 horas do modelo. Para isto, foram utilizados 352 pares de previsões do modelo BAM V2.1.1, realizado para o ano de 2019. Acrescenta que há um software desenvolvido pelo grupo para fazer a validação da matriz calculada ([GSIBerror](https://github.com/GAD-DIMNT-CPTEC/GSIBerror)) e que as comparações são realizadas utilizando-se uma matriz de referência fornecida pelo _Developmental Testbed Center_ ([DTC](https://dtcenter.org/)). Cita que a matriz calculada, assim como outras versões baseadas no modelo BAM em coordenada sigma, apresenta problemas na representação das variáveis conteúdo de água líquida e ozônio. Para contornar este problema, as quantidades referentes ao desvio-padrão e comprimentos de escala horizontal e vertical, são copiados da matriz de referência. Finaliza dizendo que a versão do SMNA que está sendo operacionalizada, ainda não utiliza a matriz calculada devido à necessidade de se realizar testes e ajustes. Acrescenta que a matriz atualmente em uso, é a matriz fornecida pelo DTC.

## Pauta 5 - Macrogrupo de dados de satélite para modelagem

Luiz Sapucci convida Renato Galante para comentar sobre as propostas do macrogrupo de dados de satélites para a modelagem. Renato Galante cita que há atividades em andamento relacionadas com o uso dos sistemas de rastreamento dos satélites de órbita baixa, os quais se tem interesse para coletar dados e prepará-los para a assimilação. Luiz Sapucci agradece e comenta que alguns itens que ficaram para serem discutidos sobre a colaboração com a Divisão de Satélites e Sistemas Meteorológicos ([DISSM](http://satelite.cptec.inpe.br/home/index.jsp?i=br)), serão retomados este ano. 

## Pauta 6 - Status da implementação da assimilação de dados oceânica na Egeon

Luiz Sapucci comenta sobre o status de utilização das máquinas operacionais de pesquisa e operação do CPTEC, principalmente sobre a situação das máquinas XC50 e Egeon. Dentro deste assunto, Luiz Sapucci convida os novos membros Clemente Tanajura e Felipe Costa para comentarem sobre os desafios e os desenvolvimentos realizados no âmbito da implementação do sistema de assimilação de dados oceânicos. 

Clemente Tanajura comenta que o sistema de assimilação de dados oceânicos com o qual trabalham, o _Regional Ocean Data Assimilatiom System_ ([RODAS](https://link.springer.com/article/10.1007/s10236-019-01309-8)), é capaz de assimilar dados de temperatura da superfície do mar. Comenta que, devido às limitações de mão de obra, os dados de temperatura da superfície do mar assimilados são, de fato, provenientes de uma análise do _Operational Sea Surface Temperature and Ice Analysis_ ([OSTIA/MetOffice](https://ghrsst-pp.metoffice.gov.uk/ostia-website/index.html)), ao invés de dados de radiância como é feito em outros grupos como o _Global Modeling and Assimilation Office_ ([GMAO/NASA](https://gmao.gsfc.nasa.gov/)). Comenta que o grupo possui o próprio sistema de controle de qualidade dos dados para perfis verticais de temperatura e salinidade e que também conseguem assimilar dados altimétricos. O sistema com o qual trabalham é capaz também de produzir _superobs_. 

Sobre os trabalhos com a máquina Egeon, comenta que o Felipe Costa tem trabalhado com a implementação dos softwares na máquina e que já conseguiu compilar o sistema RODAS. Felipe Costa comenta que já conseguiram compilar o modelo e que já fizeram uma simulação de 3 anos completa, com o domínio sobre o oceano Atlântico inteiro. Cita que a assimilação testada do RODAS incluiu apenas os perfis verticais, mas que estão encontrando problemas com a reinicialização do modelo, que está apresentando instabilidades. Acrescenta que os próximos passos incluem a compilação do sistema EnKF para uso em um domínio regional. 

Clemente Tanajura comenta que é necessário utilizar como forçantes as análises e previsões produzidas pelo CPTEC (por meio dos modelos _Brazilian global Atmospheric Model_ - [BAM](https://journals.ametsoc.org/view/journals/wefo/31/5/waf-d-16-0062_1.xml) e WRF), ao invés das reanálises (do  _Climate Forecast System Reanalysis_ - [CFSR](https://climatedataguide.ucar.edu/climate-data/climate-forecast-system-reanalysis-cfsr)) que estão utilizando atualmente. Isto é importante para dar um primeiro passo no sentido de se acoplar os dois sistemas de modelagem e assimilação de dados (atmosférico e oceânico). Complementa dizendo que está confiante e que até o final do ano haverá muitos frutos a serem colhidos. 

Luiz Sapucci agradece a contribuição do Clemente Tanajura e do Felipe Costa e comenta sobre a importância da interação deles com o grupo de pré-processamento liderado pelo Eduardo Barbosa. Comenta que esse grupo deverá ser capaz de receber, processar e fornecer os dados de observações necessários para o funcionamento do RODAS. 

Clemente Tanajura cita outros desafios para a assimilação de dados oceânicos, como o gelo marinho, além da atualização do modelo para o _Modular Ocean Model_ 6 ([MOM6](https://github.com/mom-ocean/MOM6)) dentro do RODAS utilizando o EnOI. Cita que esta é uma alternativa para a comunidade de usuários do _Regional Ocean Modeling System_ ([ROMS](https://www.myroms.org/)) com o 4DVar, devido ao seu elevado custo computacional. Apesar disso, tem conhecimento sobre os planos com o _Joint Effort for Data assimilation Integration_ ([JEDI](https://www.jcsda.org/jcsda-project-jedi)) e o _Model for Ocean-laNd-Atmosphere PredictioN_ ([MONAN](https://monanadmin.github.io/monan_cc_docs/)) e que esse sistema também está sendo levado em consideração.

## Pauta 7 - Assimilação de dados utilizando Inteligência Artificial

Luiz Sapucci convida o pesquisador Haroldo Fraga para comentar sobre os avanços realizados no tema de assimilação de dados utilizando Inteligência Artificial. Luiz Sapucci comenta sobre a importância dessa atividade no contexto dos desenvolvimentos realizados pelo grupo e sobre a importância de sempre haver um representante desse tema nas reuniões.

Haroldo Fraga inicia a sua fala comentando sobre o avanço da habilidade de previsão dos modelos numéricos e a sua relação com o aumento significativo de dados disponíveis para assimilação. Essa é uma relação conhecida e demonstra a importância da assimilação de dados na melhoria da qualidade das previsões dos modelos, sobretudo, sobre o Hemisfério Sul. Haroldo Fraga realiza uma breve revisão do assunto que motiva as suas pesquisas mais recentes até chegar nos desenvolvimentos atuais sobre Inteligência Artificial.

Devido ao tempo limite da chamada do Google Meet, a reunião foi encerrada automaticamente. Com isso, deverá ser marcada uma nova reunião para que o Haroldo Fraga possa dar as suas contribuições sobre o assunto.  

## Lista de ações 

1. **DAS-DIMNT:** reiniciar as reuniões semanais do DAS-DIMNT e tratar dos pontos destacados e discutidos no inicio da reunião e reportar na próxima reunião mensal do DAS-INPE;
1. **Luiz Sapucci:** incluir o Felipe Costa na reunião semanal do DAS-DIMNT;
1. **Luiz Sapucci:** enviar para todos a versão do roadmap da assimilação atmosférica em 2023 para colher contribuições e posteriormente enviar para a chefia da DIMNT;
1. **João Gerd e Clemente Tanajura:** preparar um roadmap da assimilação de superfície para 2023 e enviar para a apreciação de todos;
1. **Grupo DAS-INPE e Luiz Sapucci:** dar andamento ao relatório da versão SMNA 2.3.1, com expectativa de se ter uma versão 80% finalizada no final de fevereiro;
1. **Eduardo Barbosa, Sergio Ferreira e João Gerd:** reiniciar as conversas visando a elaboração de um plano de trabalho para a implementação do controle de qualidade dos dados recebidos no CPTEC;
1. **Luiz Sapucci e Grupo DAS-DISSM:** retomar o documento sobre o macrogrupo de dados de satélites para a assimilação e encaminhar para aprovação;
1. **Felipe Costa e Clemente Tanajura:** avançar com a implementação na Egeon da assimilação oceânica usando o RODAS e reportar o status na próxima reunião;
1. **Felipe Costa, Clemente Tanajura e Eduardo Barbosa:** iniciar as conversas sobre o fluxo de dados requeridos pelo RODAS a ser avaliado a disponibilidade no pré-processamento do CPTEC e tratar de sua adequação;
1. **Haroldo Fraga e Luiz Sapucci:** marcar uma reunião especifica para tratar da assimilação global usando redes neurais para divulgar o andamento dos trabalhos nesse grupo;
1. **Carlos Bastarz e Luiz Sapucci:** preparar a memória dessa reunião e disponibilizá-la no git do DAS-MONAN.
