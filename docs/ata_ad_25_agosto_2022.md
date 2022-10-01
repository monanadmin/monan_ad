# 25 de Agosto de 2022

## ATA 001/2022 - Revisão 001

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados para o MONAN"
    
        * Preparado por: Carlos Frederico Bastarz
        * 25 de Agosto de 2022
        
        **Coordenação:** João Gerd Zell de Mattos e Luiz Fernando Sapucci
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 25/08/2022      | <ul> <li> Versão inicial </li> </ul> |
        | R001    | 01/10/2022      | <ul> <li> Revisão do texto e inclusão de links </li> </ul> |
    
    === "Participações"
    
        * **INPE:** 
        * Carlos Frederico Bastarz
        * Dirceu Luis Herdies
        * Éder Paulo Vendrasco
        * Eduardo Barbosa
        * Haroldo Fraga Campos Velho
        * João Gerd Zell de Mattos
        * José Antônio Aravéquia
        * Luciana Mira
        * Luiz Fernando Sapucci
        * Liviany Viana
        * Natália Rudorff
        * Renato Galante Negri
        * Sergio Henrique Ferreira
        
    === "Registro"
    
        **Local, Data e Hora**
        
        * Plataforma Google Meet
        * 25 de Agosto de 2022, das 15:30 horas às 17:00 horas
        
        **Repositório das apresentações**
        
        * [https://drive.google.com/drive/folders/1X8JHL6ZvT3aQOPwFzsiuGRNEaDrUVbBs?usp=sharing](https://drive.google.com/drive/folders/1X8JHL6ZvT3aQOPwFzsiuGRNEaDrUVbBs?usp=sharing)

## Pauta 1 - Organização do modo operante do grupo DAS-MONAN introdução e visão geral

Luiz Sapucci faz uma introdução sobre o escopo das reuniões da assimilação de dados dentro do contexto do _Model for Ocean-laNd-Atmosphere predictioN_ ([MONAN](https://monanadmin.github.io/monan_cc_docs/)). Dá as boas vindas a todos e demonstra a sua satisfação com esta integração entre os componentes das várias divisões do [INPE](https://www.gov.br/inpe/pt-br). Assinala que existe a necessidade de se integrar as divisões para que a assimilação de dados possa funcionar bem. Destaca que a proposta do MONAN é um projeto nacional, contextualizado dentro da Rede Nacional de Meteorologia e que esta é uma ótima oportunidade para que as atividades em assimilação de dados possam se organizar melhor dentro do INPE. Cita como atividades próximas os workshops entre as divisões da [CGCT](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct) e da assimilação de dados. Abre a palavra para a contribuição de todos para externarem as suas percepções. 

Luiz Sapucci destaca que o servidor do INPE [Kleber Naccarato](http://lattes.cnpq.br/6324293045209180), especialista em raios e eletricidade atmosférica, mostrou bastante interesse em participar do grupo de desenvolvimentos em assimilação de dados para o MONAN e que ele já deverá estar integrado ao grupo até a próxima reunião. Apesar de o MONAN ainda estar em um estágio inicial de desenvolvimentos, a qual ainda não envolve a escala convectiva, destaca que nesse ínterim, deverá haver outros tipos de interações com o Kleber Naccarato sobre a assimilação de dados de raios (ou descargas elétricas) em outros trabalhos.

Sobre a dinâmica de interação do grupo, comenta que o ideal seria já haver um processo operacional do MONAN, mas que, por outro lado, isso favorece as discussões do grupo no sentido de ser um fórum de discussões. Nesse sentido, relata sobre o planejamento de um possível concurso onde deverá haver vagas para a assimilação de dados. Comenta sobre a ideia de vagas casadas, de forma que possa haver vagas em outras divisões mas que tenham foco em assimilação de dados, pensando de forma integrada ao contrário da forma particionada vigente.

## Pauta 2 - O status da assimilação no MONAN

Sobre o processo pré-operacional da assimilação de dados no CPTEC, Luiz Sapucci comenta que a expectativa para o workshop entre as 3 divisões do CPTEC é o entendimento de que a atividade de assimilação de dados é importante por ser o alicerce para o MONAN. Nesse sentido, destaca que a Divisão de Tempo e Clima ([DIPTC](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct)) deve ter um processo pré-operacional para que seja possível exercitar todo o processo de avaliação da assimilação de dados, incluindo a interação com a equipe de desenvolvimento do modelo e a avaliação do impacto dos dados assimilados. Destaca que isso foi exposto para o diretor do INPE e mostrou que isso é importante para o desenvolvimento do MONAN, de forma que o _Joint Effort for Data Assimilation Integration_ ([JEDI](https://www.jcsda.org/jcsda-project-jedi)) possa também passar por esse ambiente. Por outro lado, a justificadiva da DIPTC é a restrição de uso das máquinas, mas que a implementação da assimilação está na lista da DIPTC. Comenta que o [Clézio de Nardin](http://lattes.cnpq.br/8030262077949409) (diretor do INPE) foi convidado para o workshop para falar sobre a importância da assimilação de dados e falar sobre a importância da operacionalização da assimilação de dados no centro.

Luiz Sapucci destaca que as atividades deste grupo será olhar para os macro prolemas e que os micro problemas serão abordados no dia a dia. 

## Pauta 3 - Status do pré para a assimilação

Seguindo a pauta, Luiz Sapucci faz uma introdução ao trabalho do Eduardo Barbosa sobre o processamento dos dados. Comenta que esse trabalho está relacionado com a organização de uma base de dados para a assimilação de dados. Cita que os trabalhos anteriores nesse assunto não consideravam um pré-processamento específico para a assimilação de dados, o que inclui padronização, checagem por dados duplicados entre outros aspectos diferentes, o que é mais adequado para as atividades de assimilação de dados do centro. Destaca também o trabalho da Luciana Mira sobre a recepção, organização e manutenção de um histórico sobre os dados recebidos do [NCEP](https://www.ncep.noaa.gov/) para uso no CPTEC.

Eduardo Barbosa inicia a sua apresentação agradecendo a introdução feita pelo Luiz Sapucci. Complementa dizendo que esse trabalho é do time de dados, que é composto por várias pessoas. Continua a apresentação com uma discussão sobre o estado do pré-processamento. Em relação ao fluxo de dados, comenta que os trabalhos são divididos entre recepção, pré-processamento e armazenamento. Na entrada de dados, cita que um canal é o _Global Telecommunication System_ ([GTS](https://public.wmo.int/en/programmes/global-telecommunication-system)), por meio do [INMET](https://portal.inmet.gov.br/), e um canal redundante chamado _Internet Data Distribution_ ([IDD](https://www.unidata.ucar.edu/projects/idd/iddgeneral.html)). Quando necessário, essa passagem de um canal para outro é feita manualmente, mas de forma transparente. O padrão dos dados inclui ASCII, BUFR e também o [PrepBUFR](https://www.ecmwf.int/sites/default/files/elibrary/2012/17420-bufr-data-and-metview.pdf). Alguns dados são armazenados em bando de dados relacional ([PostgreSQL](https://www.postgresql.org/)) e tem como usuários os grupo de clima e a web do CPTEC. Os dados utilizados pela assimilação de dados são utilizados diretamente a partir do sistema de arquivos, o que significa que a parte do pré-processamento gerada pelo grupo de dados não é completamente utilizada. No banco de dados há uma série de dados que incluem a garantia da qualidade dos dados de precipitação, temperaturas máxima e mínima. As demais variáveis não passam por um sistema de controle de qualidade. Cita que, a partir dos dados do GTS, é possível separar os dados em convencionais e não convencionais. Sobre as estatísticas provenientes do pré-processamento, cita como exemplos os dados de aeronaves, dados convencionais de superfície da Terra onde é possível identificar diferentes tipos de dados (mensagens sinóticas, e.g., METAR, SYNOP, SHIP entre outros). A partir desta exposição, mostra os diferentes padrões de coberturas e tipos separados por cores diferentes. Cita que ainda há algumas dificuldades na identificação de alguns satélites a partir dos dados brutos provenientes do GTS. Sobre as redes regionais do país (além do GTS), cita o Instituto Agronômico de Campinas ([IAC](https://www.iac.sp.gov.br/)), INPE e outra, as quais também tem recepção no CPTEC e apresenta mapas com a sua distribuição. Ainda sobre o pré-processamento, cita que são realizadas as seguintes atividades: agrupamento, eliminação de inconsistências, homogenização dos padrões e armazenamento. Sobre o controle de qualidade, cita que há dois formatos _Traditional Alphanumeric Codes_ ([TAC](https://community.wmo.int/activity-areas/operational-information-service/migration-tac-tdcf)) e BUFR, os quais precisam ser agrupados a partir do que são identificadas duplicidades para as quais são tratadas as redundâncias. Esta seria a primeira etapa do controle de qualidade, eliminar as duplicidades dando preferência pelo formato binário (BUFR) e eliminando o formato tradicional (TAC). Cita que são testados também os limites das variáveis, de forma elementar, verificando se os valores reportados pelas observações estão dentro de um intervalo consistente. Cita que a _World Meteorological Organization_ ([WMO](https://public.wmo.int/en)) indica quais são estes limites e que eles foram implementados pelo grupo. A consistência interna também é feita de forma que as variaveis de uma estação são comparadas com outras variáveis de uma mesma estação (e.g., intensidade X direção do vento - nesse caso, se pelo menos uma quantidade for inconsistente, ambas são descartadas). Finalizando, cita que a partir de Julho de 2022, haverá o aumento da quantidade e da qualidade das observações adquiridas, com vistas para a operacionalização da assimilação de dados.

Luiz Sapucci ressalta a importância do trabalho realizado pelo grupo do Eduardo Barbosa e ressalta também o fato de que os dados já estavam armazenados no centro, mas que não tinham a revisão do grupo e que este grupo tem se debruçado sobre os dados e que isso tem dado resultados, com a adequada triagem dos dados para a assimilação de dados. Eduardo Barbosa complementa dizendo que essa atividade foi possível a partir dos manuais de decodificação dos dados providos pela WMO e que ainda sim, existe uma dificuldade na identificação dos dados, mas que isso está avançado. Ressalta que é importante a ajuda dos especialista em dados para a identificação dos dados, cita a colaboração com a [Rosio Camayo](http://lattes.cnpq.br/1788219937327281), que ajuda muito nesse aspecto quanto ao uso dos dados oceanográficos. Eduardo Barbosa comenta que os dados de satélite não são armazenados e tratados pelo grupo para a assimilação, mas que os dados de radar sim.

Luiz Sapucci comenta que é importante o envolvimento dos especialistas em dados em apoio do grupo do Eduardo Barbosa. Comenta que a sua atuação, quanto aos dados de rádio ocultação, é importante e deve se comprometer com o grupo do Eduardo Barbosa, a exemplo da Rosio Camayo. 

## Pauta 4 - Geração do dados PrepBUFR de radiância em paralelo

Luiz Sapucci convida o Sérgio para a apresentação dele sobre a geração dos dados PrepBUFR com processamento paralelo. Durante a sua apresentação, Sergio Ferreira cita que iniciou o trabalho em Março de 2020. Mostra gráficos comparando o tempo de decodificação dos dados em termos do volume de dados. Mostra que o tempo de processamento é bem menor, aproximadamente 5 min em comparação com os 20 min anteriores (para os dados convencionais). Cita que fez testes mais extensivos (nos últimos dois anos), considerando aproximadamente 10 milhões de observações (considerando dados convencionais e não convencionais) e que o tempo de processamento dos dados do _Advanced Microwave Sounding Unit_ ([AMSU](https://en.wikipedia.org/wiki/Advanced_microwave_sounding_unit)) - a maior quantidade, não é muito diferente dos demais dados. Comenta que o tempo de processamento obtido é bastante adequado para a assimilação operacional. Para os dados do _Infrared Atmospheric Sounding Interferometer_ ([IASI](https://en.wikipedia.org/wiki/Infrared_atmospheric_sounding_interferometer)), por outro lado, cita que o tempo de processamento é muito alto (aproximadamente 40 min) e que isso se deve à complexidade da estrutura de dados do IASI. Comenta que o algoritmo para a decodificação desses dados acaba sendo mais complexa e que isso faz com que os dados sejam processados em um tempo maior. 

Sérgio Ferreira parabeniza o Eduardo Barbosa sobre a sua apresentação. Pergunta se os procedimentos de controle de qualidade são aplicados aos TACs e BUFRs, Eduardo Barbosa responde que sim, em ambos. Eduardo Barbosa complementa dizendo que, após o controle de qualidade, as observações são marcadas com _flags_ do controle de qualidade e, em caso de inconsistências, as observações são marcadas como _missing_, mas que as _flags_ não são alteradas dentro do BUFR - nesse caso, o dado é considerado como _missing_, ou seja, o valor da observação é alterado para um valor indefinido e o BUFR. O controle de qualidade é aplicado apenas para os dados de superfície.

Luiz Sapucci agradece o Sergio Ferreira e comenta que esse é um trabalho muito importante. Comenta que é necessário contextualizar o trabalho para a apresentação no workshop da assimilação de dados.

## Pauta 5 - Assimilação redes neurais global no CPTEC

Na próxima apresentação, Luiz Sapucci convida o Haroldo Fraga para falar sobre o seu trabalho com a assimilação de dados utilizando [redes neurais](https://pt.wikipedia.org/wiki/Rede_neural_artificial). Haroldo Fraga inicia a sua apresentação e comenta sobre os trabalhos que tem realizado na área de problemas inversos, aplicados em diversas áreas. Cita que o seu interesse em redes neurais artificiais começou com um problema inverso na área de meteorologia, com perfis recuperados de temperatura. Faz uma rápida revisão sobre diversos métodos de assimilação de dados e aspectos das teorias destes métodos. Chega ao [Filtro de Kalman](https://pt.wikipedia.org/wiki/Filtro_de_Kalman), discute alguns aspectos importantes. Luiz Sapucci agradece a apresentação do Haroldo Fraga, enaltece a sua importância e reconhece que as suas atividades são importantes para o desenvolvimento da assimilação de dados no contexto do MONAN. Comenta que na área científica, há muitas parcerias que são profícuas e que em algum momento elas devem ser traduzidas para a área operacional. No ambiente técnico no grupo, Luiz Sapucci pergunta como esses desenvolvimento podem ser traduzidos em produtos. Aproveita a oportunidade para expressar interesse nos seus desenvolvimentos e que este é o ambiente para que o Haroldo Fraga possa também desenvolver os seus produtos. Cita que e emulação da análise do NCEP é feita utilizando os dados que são recebidos pelo CPTEC, é também de interesse do centro. 

## Pauta 6 - Workshop em assimilação de dados a ser realizado em Outubro

Luiz Sapucci faz uma rápida apresentação sobre o cronograma inicial do workshop da assimilação de dados. Explica para os participantes a estratégia de organização das apresentações e convida a todos para darem as suas contribuições.

??? example "Anexos"

    * [Slides Sérgio Henrique](https://drive.google.com/file/d/128spvtgMrYscPtXdR1rFzfoRPHc1mtx-/view?usp)
    * [Slides Eduardo Barbosa](https://drive.google.com/file/d/1akVdQh_r8edNxE8W8QfED2C0ZbmOcwV6/view?usp)
    * [Slides Haroldo Campos Velho](https://drive.google.com/file/d/1-lEwRxFiefP413xgmAhVcH3ZDxjWL5dJ/view?usp)
