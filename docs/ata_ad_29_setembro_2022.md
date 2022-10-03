# 29 de Setembro de 2022

## ATA 002/2022 - Revisão 001

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados para o MONAN"
    
        * Preparado por: Carlos Frederico Bastarz
        * 29 de Setembro de 2022
        
        **Coordenação:** João Gerd Zell de Mattos e Luiz Fernando Sapucci
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 29/09/2022      | <ul> <li> Versão inicial </li> </ul> |
        | R001    | 01/10/2022      | <ul> <li> Revisão do texto e inclusão de links </li> </ul> |
    
    === "Participações"
    
        * **INPE:** 
        * Carlos Frederico Bastarz
        * Dirceu Luis Herdies
        * Éder Paulo Vendrasco
        * Eduardo Barbosa
        * João Gerd Zell de Mattos
        * José Antônio Aravéquia
        * Kleber Naccarato
        * Luciana Mira
        * Luiz Fernando Sapucci
        * Liviany Viana
        * Natália Rudorff
        * Renato Galante Negri
        * Sergio Henrique Ferreira
        
    === "Registro"
    
        **Local, Data e Hora**
        
        * Plataforma Google Meet
        * 29 de Setembro de 2022, das 15:30 horas às 16:30 horas
        
## Abertura

Luiz Sapucci inicia a reunião citando os assuntos a serem tratados durante a reunião, citando a inclusão de novos membros, o status da assimilação no _Model for Ocean-laNd-Atmosphere predictioN_ ([MONAN](https://monanadmin.github.io/monan_cc_docs/)), as atividades do grupo de pré-processamento, atividades de assimilação com métodos não convencionais, as contribuições da Divisão de Satélites e Sistemas Meteorológicos ([DISSM](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct)) e o workshop da assimilação.

Luiz Sapucci pergunta se alguém gostaria de incluir mais algum item. Aprovada a pauta, Luiz Sapucci prossegue para a pauta 1, com a apresentação do novo membro, o pesquisador [Kleber Naccarato](http://lattes.cnpq.br/6324293045209180) da DISSM.

## Pauta 1 - Inclusão de novos membros

Kleber Naccarato inicia a sua fala e agradece a oportunidade. Faz um breve relato sobre a sua trajetória, cita que entrou no [INPE](https://www.gov.br/inpe/pt-br) em 2013 ainda no antigo Centro de Ciências do Sistema Terrestre ([CCST](http://www.ccst.inpe.br/)) e que a sua expertise sempre foi a física de raios. Seu interesse está nas técnicas de observação  e monitoramento de raios. Comenta que os estudos estão, em boa parte, relacionados com a climatologia dos raios, mas que atualmente tem crescido o interesse no estudo e na detecção de raios a partir e nano-satélites. Em relação ao MONAN, comenta que há o interesse de se utilizar os dados de observação de raios para a assimilação, na transformação dos dados de raio em parâmetros que podem ser utilizados para a correção de parâmetros específicos do modelo. Acrescenta que este procedimento tem potencial para melhorar a representação da convecção, da chuva e outros parâmetros do modelo.

Luiz Sapucci agradece as contribuições do Kleber Naccarato. Comenta que a intenção é importante, mas que ainda está longe de se chegar ao ponto em que as observações de raios possam ser utilizadas na assimilação, mas que haverá um momento certo para o desenvolvimento das linhas de trabalho para essa área. Luiz Sapucci complementa dizendo que a atitude e o interesse do Kleber Naccaratosão bastante entusiasmantes. 

## Pauta 2 - Status da assimilação no MONAN

Luiz Sapucci cita que, em relação ao status da assimilação para o MONAN, a primeira tarefa é colocar o modelo _Brazilian Atmospheric Model_ ([BAM](https://journals.ametsoc.org/view/journals/wefo/31/5/waf-d-16-0062_1.xml)) e o sistema _Gridpoint Statistical Interpolation_ ([GSI](https://dtcenter.org/community-code/gridpoint-statistical-interpolation-gsi)) operacionais no CPTEC e, a segunda, é a atualização do RoadMap das versões do MONAN com a assimilação, de qual será a sequência de desenvolvimentos entre a versão a ser operacionalizada da assimilação de dados do CPTEC (i.e., o Sistema de Modelagem Numérica e Assimilação ([SNMA](http://mtc-m21c.sid.inpe.br/ibi/sid.inpe.br/mtc-m21c/2019/05.16.15.18?metadatarepository=sid.inpe.br/mtc-m21c/2019/05.16.15.18.01&ibiurl.backgroundlanguage=pt-BR&ibiurl.requiredsite=mtc-m21c.sid.inpe.br+806&requiredmirror=urlib.net/www/2017/11.22.19.04.03&searchsite=bibdigital.sid.inpe.br:80&searchmirror=sid.inpe.br/bibdigital@80/2006/04.07.15.50.13&searchinputvalue=sistema+de+modelagem+num%E9rica+e+assimila%E7%E3o&parentidentifiercitedby=6qtX3pFwXQZ4iE8KMKjdY/KFQ6T&forcerecentflag=0)), composto pelo BAM e GSI) e a primeira versão de assimilação de dados do MONAN). A terceira ação, é a validação do experimento 18 da assimilação de dados (i.e., um dos últimos experimentos realizados pelo grupo de assimilação de dados do CPTEC, envolvendo a suíte SMNA), como avaliação diagnóstica. Estes são os 3 pontos a serem tratados pelo grupo de assimilação de dados para o próximo mês.

## Pauta 3 - Atividades de pré-processamento

Seguindo a pauta, Luiz Sapucci comenta que o Eduardo Barbosa deverá relatar as atividades e os avanços das atividades do pré-processamento (observações).

Eduardo Barbosa cita, dentre as atividades realizadas, a configuração dos novos receptores de dados, a migração da recepção de dados de radar para serem recebidos pela Divisão de Tempo e Clima ([DIPTC](https://www.gov.br/inpe/pt-br/composicao/diretoria/coordenacao-geral-de-ciencias-da-terra-cgct)) e algumas manutenções de scripts de triagem para a separação de dados. Cita que foram detectadas algumas inconsistências e que estas estão sendo tratadas. 

Luiz Sapucci agradece as contribuições do Eduardo Barbosa e comenta que no workshop da assimilação de dados, a ser realizado na a próxima semana, será uma boa oportunidade de conversar sobre esse assunto. Comenta que é importante que os grupos possam dominar todos os processos envolvidos, frente a importância deles ao INPE e ao MONAN.

## Pauta 4 - Atividades de assimilação com métodos não-convencionais 

Prosseguindo, Luiz Sapucci avançá para a próxima pauta com a apresentação do Haroldo Fraga, que não pôde comparecer à reunião. Luiz Sapucci informa que o grupo do Haroldo Fraga tem reuniões semanais com o pessoal do modelo global BAM e que esse é o tema que ele apresentaria. Luiz Sapucci comenta que se houver alguma demanda que esse grupo deve ajudar, então eles deverão trazer para a discussão na reunião.

## Pauta 5 - Contribuições da DISSM

Luiz Sapucci convida Renato Galante para fazer o seu relato sobre as atividades da DISSM no âmbito da assimilação de dados para o MONAN.

Renato Galante comenta sobre algumas novidades, que envolvem uma força tarefa junto com o [Saulo Freitas](http://lattes.cnpq.br/9873289111461387), onde foram indicados o Thiago Biscaro e o Rogério Batista. Na lista, comenta que ele a [Izabelly Costa](http://lattes.cnpq.br/0647725719729152) e outros colaboradores devem revisar os dados do banco de dados para identificar o que está faltando. Também, cita sobre as instabilidades da antena da _Direct Broadcast Network_ ([DBNET](https://community.wmo.int/activity-areas/wmo-space-programme-wsp/dbnet)), situada em Cuiabá/MT. Comenta que há várias pessoas envolvidas nas demandas e que as ações estão sendo tomadas para que seja possível termos a versão operacional do BAM com a assimilação de dados.

Luiz Sapucci comaneta, sobre a DBNET, que a assimilação ajudará nesse tema porque trata-se dos dados provenientes de uma antena que está com problemas e que isso deve ser devidamente tratado para a sua resolução. Comenta que participou da reunião da _World Meteorological Organization_ ([WMO](https://public.wmo.int/en)), que contou também com a participação do [Diego Souza](http://lattes.cnpq.br/3645067978235955) da DISSM, e que ficou clara a importância da DISSM e que isso deve ser preservado. 

Renato Galante acrescenta que, com a demanda pelo dado, consequentemente haverá a intenção de se consertar a antena para a recepção e uso dessess dados. Luiz Sapucci acrescenta que é necessário fazer as ocorrências e reportar os problemas para que eles sejam evidenciados e devidamente tratados. 

## Pauta 6 - Workshop da assimilação de dados

Luiz Sapucci, em relação à pauta do workshop da assimilação de dados a ser realizado nos dias 6 e 7 de Outubro de 2022, comenta sobre ajustes na programação. Cita que uma das mudanças é a alteração do horário da apresentação do Kleber Naccarato. Kleber Naccarato comenta sobre a quantidade de atividades desenvolvidas dentro da assimilação e que é importante a gravação do workshop para que ele possa se inteirar sobre essas atividades. Luiz Sapucci cita a inclusão da [Flávia Pinheiro](http://lattes.cnpq.br/2782043473646574) da Marinha do Brasil ([MB](https://www.marinha.mil.br/)) na mesa redonda. Cita que a [Brunna Romero](http://lattes.cnpq.br/5396636443614215) da MB também participará, mas como ouvinte. Luiz Sapucci comenta sobre as especialidades delas, que são os sensores a bordo de navios e que a colaboração com elas está nessa vertente da assimilação de dados desenvolvida no CPTEC. Comenta que será feito um convite para que elas possam apresentar também os resultados das suas atividades e interação entre a MB e o CPTEC. Acrescenta que o [Luciano Pezzi](http://lattes.cnpq.br/9168878830863753) não poderá participar da mesa redonda com o [Clemente Tanajura](http://lattes.cnpq.br/0765423133125301) e que o [Ronald Buss](http://lattes.cnpq.br/0537824080913130) será convidado para o seu lugar. 

## Pauta 7 - Outros assuntos

Outro item, é sobre a criação de um repositório para o armazenamento das apresentações do workshop (vide a seção de anexos). Luiz Sapucci comenta que é necessário criar uma lista dos apresentadores para que eles possam adicionar as suas apresentações e os demais para apenas visualização. Cita sobre o template das apresentações do workshop que está disponível para uso. Convida a todos para disponibilizarem as suas apresentações. Conclui dizendo que isso facilita a preparação dos documentos entre os participantes, de forma a evitar informações redundantes.

## Ações para o próximo mês

* **Ação01 @Sapucci:** Enviar por email o endereço do repositório para todos do DAS-MONAN contendo o template, o objetivo do repositório é que todos os apresentadores antecipadamente conhecam o que os demais colegas vão apresentar.
* **Ação03 @Sapucci:** Organizar junto a secretaria da DIMNT o procedimento adequado para a inclusão de cobaboradores do grupo DAS-MONAN. Nessa oportunidade iremos proceder a inclusão do Kleber P. Naccarato e Aurelienne Aparecida Souza Jorge do pré.
* **Ação04 @Eduardo:** Enviar o template por email e colocar no repositorio das apresentações do workshop DAS-MONAN
* **Ação05 @João:** Avançar com o Alex e demais membros do comitê de pré operação da assimilação e nos reportar os avanços na próxima reunião.
* **Ação06 @Carlos:** Escrever a ata da reunião no GitHub do MONAN com a lista de ações para o próximo mês.
* **Ação07 @João;@Aravequia:** Avançar com a versão do GSI no BAM-HIB na EGEON usando INTEL e GNU e reportar os andamento dessa atividade; 
* **Ação08 @Haroldo:** Avançar com a Assimilação de dados usando redes neurais Global como o modelo do CPTEC e reportar o reportar os andamento dessa atividade; 
* **Ação09 @Eduardo:** Avançar com a ampliação da triagem de novos dados para a assimilação e reportar os andamento dessa atividade; 
* **Ação10 @Renato:** Avançar na recepção/tratamento/avaliação de dados de satélites para a assimilação no BAM-HIB-GSI e reportar os andamento dessa atividade;
* **Ação11 @Sapucci:** Tratar com o pessoal da marinha a possibilidade da Comandante Flavia e Tenente Brunna Romero participar da nossa próxima reunião e apresentarem seus trabalhos sobre o tema assimilação de dados;
* **Ação12 @Sapucci:** Compilar os arranjos mais importantes obtidos nos resultados do Workshop e apresentar para discussão no grupo DAS-MONAN;
* **Ação13 @Haroldo:** Avançar com a Assimilação de dados usando redes neurais Global como o modelo do CPTEC e reportar o reportar os andamento dessa atividade; 
* **Ação14 @Sapucci:** atualizar o RoadMAp da assimilação pré operacional com as novas versões e um novo cronograma de entrega para 2023;
* **Ação15 @Todos:** Iniciar uma versão draft da avaliação diagnostica da assimilação de dados do sistema SMNA (BAM-HIB-GSI) experimento 18 para servir de relatório técnico da versão inicial pré operacional.  

??? example "Anexos"

    * [Repositório das Apresentações do Workshop da Assimilação de Dados](https://drive.google.com/drive/folders/1KjBX5Ek2mtY49SOBy9L1yex3ur9MhC5m?usp=sharing)
    * [Template para as Apresentações do Workshop da Assimilação de Dados](https://docs.google.com/presentation/d/1vpyZuzJaEp4MiJe8EaoyzzGKpUfFtub4/edit?usp=sharing&ouid=110636406231513515149&rtpof=true&sd=true())

