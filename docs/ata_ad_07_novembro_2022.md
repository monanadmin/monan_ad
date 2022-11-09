# 07 de Novembro de 2022

## ATA 001/2022 - Revisão 000

??? info "Informações"

    === "Ata da Reunião do Grupo de Desenvolvimento em Assimilação de Dados da DIMNT"
    
        * Preparado por: Carlos Frederico Bastarz
        * 07 de Novembro de 2022
        
        **Coordenação:** Luiz Fernando Sapucci
    
    === "Histórico de Revisões"
    
        | REVISÃO | DATA DA REVISÃO | ALTERAÇÕES |
        |---------|-----------------|------------|
        | R000    | 07/11/2022      | <ul> <li> Versão inicial </li> </ul> |
    
    === "Participações"
    
        * **INPE:** 
        * Carlos Frederico Bastarz
        * João Gerd Zell de Mattos
        * Luiz Fernando Sapucci

        * **UFBA:**
        * Clemente Augusto Souza Tanajura
        * Felipe Costa
        
    === "Registro"
    
        **Local, Data e Hora**
        
        * Plataforma Google Meet
        * 07 de Novembro de 2022, das 09:00 horas às 10:00 horas
        
## Pauta

1. Informações iniciais sobre a abertura de contas e um plano de trabalho inicial;
2. Ideias e expectativa de vida do RODAS no CPTEC e trabalhos no MONAN;
3. Primeiras ações de ordem técnica para a instalação do RODAS no Egeon;
4. Perspectivas de trabalho e projetos futuros na continuidade dos trabalhos.

## Pauta 1 - Informações iniciais sobre a abertura de contas e uma plano de trabalho

Clemente iniciou a reunião dizendo que ele e o Filipe já tem acesso a máquina Egeon e que precisa das informações iniciais para iniciar o processo de instalação do RODAS no sistema. Ele destacou qual seria a estratégia de implementação do sistema e a versão e o domínio para atender a costa brasileira. Ele destacou que há dificuldades de se fazer modificações no aninhamento das versões para compatibilizar os níveis verticais do sistema entre diferentes domínios. Procurando evitar modificações na mesma versão que eles rodam hoje na máquina Santos Dumont, a qual seria trazida para o INPE. Sapucci destacou a importância de ser ter um documento oficializando essa estratégia para assegurar a continuidade desse trabalho dentro do INPE. João disse que a plano de trabalho já está escrito e que veria com o Saulo como podemos registrar e tornar pública essa atividade no INPE. O SEI poderia ser uma forma, mas precisa ser verificado com a chefia.

## Pauta 2 - Ideias e expectativa de vida do Rodas no CPTEC e trabalhos no MONAN

Clemente disse que a ideia é iniciar com essa versão da assimilação usando a Interpolação Ótima e depois migrar para uma versão usando o Kalman Filter. Nesse tempo teríamos que avaliar como seria a integração com o modelo MONAN e como seria a assimilação de dados usando o JEDI no contexto do MONAN. Clemente se colocou à disposição para avaliar esse trabalho e como isso seria feito. Sapucci destacou que a seu ver, o MONAN deverá demorar pelo menos 4 anos para ser operacionalizado e, assim como o atmosférico deverá ser o BAM-HIB-GSI por esse tempo, a versão do RODAS com HYCOM deverá também ser explorada nesse período e, por isso, teríamos tempo para implementar essa versão e aprimorá-la usando o Kalman Filter. Clemnete destacou que há uma aluna dele nesse tema é que seria interessante que ela tivesse uma conta na Egeon para ajudar nesse tema da assimilação usando o Kalman Filter.

## Pauta 3 - Primeira ações de ordem técnica para a instalação do RODAS no Egeon

De forma técnica algumas questões-chave foram levantadas e discutidas: (a) qual seria o repositório de código a ser usado nesse projeto: Carlos destacou que como é uma projeto novo, temos que já iniciá-lo no GitHub, embora ainda tenhamos o SMNA no SVN do CPTEC. Se tiver novas melhorias que necessitem a integração dos dois sistemas, o SMNA terá que ser migrado para o GitHub. O Carlos deverá criar um local para esse projeto no GitHub do MONAN. (b) Qual o espaço de disco necessário para o RODAS na Egeon. João apresentou o disco a ser usado para essa implementação, o qual já informou que tem 60% usado dos 120 Tb disponíveis. Felipe ficou de fazer um levantamento do espaço necessário para a instalação e execução do RODAS e nos passar. João se colocou a disposição para contribuir para a otimização do tempo do Felipe no processo de instalação do RODAS na Egeon. Eles ficaram de interagir nesse processo. (c) Quais são os tipos de dados que eles utilizam na assimilação para passar para o pessoal do pré preparar a base de dados pra eles. João destacou a importância dessa lista, mas entendemos que ela não é essencial no momento e poderá ser tratada posteriormente na continuação da atividade. 

## Pauta 4 - Perspectivas de trabalho e Projetos futuros na continuidade dos trabalhos

Clemente destacou que podemos pensar em submeter uma proposta de pesquisa na FAPESP para investir nessa pesquisa, com recursos para adquirir storage de dados, recursos para participação de eventos e organização de um wokshop. Sapucci concordou e precisamos conversar para identificar a dimensão do projeto, se ele pode ser pequeno envolvendo apenas a componente oceânica ou mais amplo envolvendo todas as componentes no MONAN. Isso teríamos que conversar para discutir essa dimensão.

## Lista de ações

* João: Verificar com o Saulo como documentar apropriadamente essa atividade usando o plano de trabalho já elaborado;
* Carlos: Criar um repositório no GitHub do MONAN para esse projeto e colocar lá essa memória dessa primeira reunião;
* Felipe: Fazer um levantamento do espaço em disco necessário para o RODAS na Egeon;
* João: verificar a possibilidade de mais uma conta para a aluna do Clemente ter acesso a Egeon;
* Felipe e João: Iniciar a instalação do RODAS na Egeon e interagir com o João para avançar nesse processo de forma eficiente.

## Comentários adicionais

Clemente destacou a importância do INPE, através de seus membros do macrogrupo de assimilação de dados (DAS-MONAN), estar sendo integrado no grupo de pesquisa da REMO no DGP do CPNq, e para isso fez um convite para nossa participação. Sapucci concorda com essa integração e agradece o convite, mas destaca que embora ainda não tenhamos a especialidade em assimilação oceânica, é um tema de grande importância e essa integração pode nos ajudar a adquirir esse conhecimento e assim no futuro contribuir de forma mais real ao REMO. Obviamente, na assimilação atmosférica e sua integração com a assimilação oceânica, a contribuição do INPE pode ser efetiva.
