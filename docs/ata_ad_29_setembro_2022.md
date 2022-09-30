# 29 de Setembro de 2022

## ATA 002/2022 - Revisão 000

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados para o MONAN"
    
        * Preparado por: Carlos Frederico Bastarz
        * 29 de Setembro de 2022
        
        **Coordenação:** João Gerd Zell de Mattos e Luiz Fernando Sapucci
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 29/09/2022      | <ul> <li> Versão inicial </li> </ul> |
    
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

Luiz Sapucci inicia a reunião citando os assuntos a serem tratados durante a reunião, citando a inclusão de novos membros, o status da assimilação no MONAN, as atividades do grupo de pré-processamento, atividades de assimilação com métodos não convencionais, as contribuições da DISSM e o workshop da assimilação.

Luiz Sapucci pergunta se alguém gostaria de incluir mais algum item. Aprovada a pauta, Luiz Sapucci prossegue para a pauta 1, com a apresentação do novo membro, o pesquisador Dr. Kleber Naccarato da Divisão de Satélites e Sistema Meteorológicos.

## Pauta 1 - Inclusão de novos membros

Kleber Naccarato inicia a sua fala e agradece a oportunidade. Faz um breve relato sobre a sua trajetória, cita que entrou no INPE em 2013 ainda na antiga CSST e que a sua expertise sempre foi a física de raios. Seu interesse está nas técnicas de observação  e monitoramento de raios. Comenta que os estudos estão, em boa parte, relacionados com a climatologia dos raios, mas que atualmente tem crescido o interesse no estudo e na detecção de raios a partir e nano-satélites. Em relação ao MONAN, comenta que há o interesse de se utilizar os dados de observação de raios para a assimilação, na transformação dos dados de raio em parâmetros que podem ser utilizados para a correção de parâmetros específicos do modelo. Acrescenta que este procedimento tem potencial para melhorar a representação da convecção, da chuva e outros parâmetros do modelo.

Luiz Sapucci agradece as contribuições do Kleber Naccarato. Comenta que a intenção é importante, mas que ainda está longe de se chegar ao ponto em que as observações de raios possam ser utilizadas na assimilação, mas que haverá um momento certo para o desenvolvimento das linhas de trabalho para essa área. Luiz Sapucci complementa dizendo que a atitude e o interesse do Kleber Naccaratosão bastante entusiasmantes. 

## Pauta 2 - Status da assimilação no MONAN

Luiz Sapucci cita que, em relação ao status da assimilação para o MONAN, a primeira tarefa é colocar o modelo _Brazilian Atmospheric Model_ (BAM) e o sistema _Gridpoint Statistical Interpolation_ (GSI) operacionais no CPTEC e, a segunda, é a organização das versões do MONAN com a assimilação, de qual será a sequência de desenvolvimentos entre a versão a ser operacionalizada da assimilação de dados do CPTEC (i.e., BAM+GSI) e a primeira versão de assimilação de dados do MONAN (possivelmente com o sistema _Joint Effort for Data Assimilation Integration_ - JEDI ). A terceira ação, é a validação do experimento 18 da assimilação de dados (i.e., um dos últimos experimentos realizados pelo grupo de assimilação de dados do CPTEC, envolvendo a suíte BAM+GSI), como avaliação diagnóstica. Estes são os 3 pontos a serem tratados pelo grupo de assimilação de dados para o próximo mês.

## Pauta 3 - Atividades de pré-processamento

Seguindo a pauta, Luiz Sapucci comenta que o Eduardo Barbosa deverá relatar as atividades e os avanços das atividades do pré-processamento (observações).

Eduardo Barbosa cita, dentre as atividades realizadas, a configuração dos novos receptores de dados, a migração da recepção de dados de radar para serem recebidos pela DIPTC e algumas manutenções de scripts de triagem para a separação de dados. Cita que foram detectadas algumas inconsistências e que estas estão sendo tratadas. 

Luiz Sapucci agrade as contribuições do Eduardo Barbosa e comenta que no workshop da assimilação de dados, a ser realizado na a próxima semana, será uma boa oportunidade de conversar sobre esse assunto. Comenta que é importante que os grupos possam dominar todos os processos envolvidos, frente a importância deles ao INPE e ao MONAN.

## Pauta 4 - Atividades de assimilação com métodos não-convencionais 

Prosseguindo, Luiz Sapucci avançá para a próxima pauta com a apresentação do Haroldo, que não pôde comparecer à reunião. Luiz Sapucci informa que o grupo do Haroldo tem reuniões semanais com o pessoal do modelo global BAM e que esse é o tema que ele apresentaria. Luiz Sapucci comenta que se houver alguma demanda que esse grupo deve ajudar, então eles deverão trazer para a discussão na reunião.

## Pauta 5 - Contribuições da DISSM

Luiz Sapucci convida Renato Galante para fazer o seu relato sobre as atividades da DISSM no âmbito da assimilação de dados para o MONAN.

Renato Galante comenta sobre algumas novidades, que envolvem uma força tarefa junto com o Saulo Freitas, onde foram indicados o Thiago Biscaro e o Rogério Batista. Na lista, comenta que ele a Izabelly Costa e outros colaboradores devem revisar os dados do banco de dados para identificar o que está faltando. Também, cita sobre as instabilidades da antena da _Direct Broadcast Network_ (DBNET), situada em Cuiabá/MT. Comenta que há várias pessoas envolvidas nas demandas e que as ações estão sendo tomadas para que seja possível termos a versão operacional do BAM com a assimilação de dados.

Luiz Sapucci comaneta, sobre a DBNET, que a assimilação ajudará nesse tema porque trata-se dos dados provenientes de uma antena que está com problemas e que isso deve ser devidamente tratado para a sua resolução. Comenta que participou da reunião da _World Meteorological Organisation_ (WMO), que contou também com a participação do Diego Souza da DISSM, e que ficou clara a importância da DISSM e que isso deve ser preservado. 

Renato Galante acrescenta que, com a demanda pelo dado, consequentemente haverá a intenção de se consertar a antena para a recepção e uso dessess dados. Luiz Sapucci acrescenta que é necessário fazer as ocorrências e reportar os problemas para que eles sejam evidenciados e devidamente tratados. 

## Pauta 6 - Workshop da assimilação de dados

Luiz Sapucci, em relação à pauta do workshop da assimilação de dados a ser realizado nos dias 6 e 7 de Outubro de 2022, comenta sobre ajustes na programação. Cita que uma das mudanças é a alteração do horário da apresentação do Kleber Naccarato. Kleber Naccarato comenta sobre a quantidade de atividades desenvolvidas dentro da assimilação e que é importante a gravação do workshop para que ele possa se inteirar sobre essas atividades. Luiz Sapucci cita a inclusão da Flávia Pinheiro da Marinha do Brasil (MB) na mesa redonda. Cita que a Bruna Romero da MB também participará, mas como ouvinte. Luiz Sapucci comenta sobre as especialidades delas, que são os sensores a bordo de navios e que a colaboração com elas está nessa vertente da assimilação de dados desenvolvida no CPTEC. Comenta que será feito um convite para que elas possam apresentar também os resultados das suas atividades e interação entre a MB e o CPTEC. Acrescenta que o Luciano Pezzi não poderá participar da mesa redonda com o Clemente Tanajura e que o Ronald Buss será convidado para o seu lugar. 

## Pauta 7 - Outros assuntos

Outro item, é sobre a criação de um repositório para o armazenamento das apresentações do workshop. Luiz Sapucci comenta que é necessário criar uma lista dos apresentadores para que eles possam adicionar as suas apresentações e os demais para apenas visualização. Cita sobre o template das apresentações do workshop que está disponível para uso. Convida a todos para disponibilizarem as suas apresentações. Cita que isso facilita a preparação dos documentos entre os participantes, de forma a evitar informações redundantes.
