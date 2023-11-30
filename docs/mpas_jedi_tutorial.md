# Curso do MPAS-JEDI-tutorial

## Descrição do material

O material disponivel aqui é uma descrição das atividades realizadas pelos participantes e o material disponibilizados pelo NCAR durante o curso, (disponivel no [link](https://www.mmm.ucar.edu/events/tutorials/mpas)) com uma tradução livre de alguns trechos do texto disponibilizado, originalmente em ingles. Como o material está disponível por acesso público o material aqui é linkado para os locais do material disponível no site do NCAR, sendo mantido os direitos autoriais dos autores e instituições responsáveis. 

Informações sobre a realização do curso e sobre os participantes está disponível aqui.

## Sobre o curso

A dinâmica do curso foi uma sequência de apresentações seguida de uma breve seção de perguntas e respostas dos participantes. Duas seções de atividades práticas foram também planejadas para serem trabalhadas. A relação das apresentações seguiu a seguinte programação, cujo links para o material apresentado estão também listados junto ao título das palestras.

## Programa das apresentaçãoes e link das apresentações.

### Thursday, 21 September

| Início | - | Fim | Título | Autor |
|--------|---|-----|--------|-------| 
| 8:30	| –| 	9:00 (30 mins)| 	Registration| 
| 9:00	| –| 	9:20 (20 mins)| 	Welcome and Participants' Introduction	| Jake Liu| 
| 9:20	| –| 	10:10 (50 mins)	| Fundamentals of Data Assimilation ([slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/1-IntroDA.pdf) | Chris Snyder| 
| 10:10	| –| 	10:30 (20 mins)	| Photo Taken and Break	
| 10:30	| –| 	11:00 (30 mins)	| MPAS-JEDI Overview & Introduction to the practical exercises [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/2-Overview.pdf) | Jake Liu| 
| 11:00	| –| 	11:30 (30 mins)	| Observations (1): Converting bufr obs to IODA format & HofX Application [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/3-obs2ioda_hofx.pdf) | Junmei Ban| 
| 12:30	| –| 	13:30 (60 mins)	| Lunch	
| 13:30	| –| 	14:00 (30 mins)	| Algorithms (1): 3D/4DEnVar [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/4-3D4DEnVar.pdf) | Robert Nystrom |  
| 15:15	| – | 15:45 (30 mins)| 	Observations (2): Assimilate "conventional" obs [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/5-CONV_DA.pdf) |  Junmei Ban | 

### Friday, 22 September

| Início | - | Fim | Título | Autor |
|--------|---|-----|--------|-------| 
|9:00 | – | 9:45 (45 mins) | Algorithms (2): 3DVar, Static B, and hybrid-EnVar ([slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/6-3DVar_StaticB_Hybrid.pdf) | Byoung-Joo Jung |
|9:45 | – | 10:30 (45 mins) | Observations (3): Satellite radiance DA [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/7-RadianceDA.pdf) | Jake Liu |
|10:30 | – | 10:45 (15 mins) | Break |  
|10:45 | – | 11:15 (30 mins) | Algorithms (3): EDA and LETKF [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/8-EDA-LETKF.pdf) | Tao Sun |
|12:30 | – | 13:30 (60 mins) | Lunch |  
|13:30 | – | 14:20 (50 mins) | Workflow & Graphics packages [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/9-Workflow-Graphics.pdf) | Ivette Hernández Baños |
|14:20 | – | 14:35 (15 mins) | Regional MPAS-JEDI [slides](https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/lectures/10-Regional.pdf) | Jake Liu |
|14:35 | – | 14:50 (15 mins) | Break |  
 
## Atividades práticas do curso MPAS tutorial

Para desenvolver as atividades praticas do curso foi disponibilizado aos participantes um acesso ao supercomputador do NCAR chamado Cheyenne.ncar.edu para isso algumas ações de segurança foram requeridas como criar uma senha e utilizar uma autenticação de acesso através de um aplicativo do celular. Foi requerido que os participantes tivessem seu próprio leptop disponível durante o curso e que ele estivesse apto a acessar um ambiente Linux via acesso SSH. Foi criado um usuário no sistema Cheyenne e um ambiente de submissão de Jobs no supercomputador. Foi recomendado a leitura do manual da máquina para todos os participantes. O manual está disponível no seguinte link de internet:

https://www2.mmm.ucar.edu/projects/mpas/mpas_atmosphere_users_guide_8.0.1.pdf

As atividades práticas foram desenvolvidas em seções específicas para esse fim, cujo a lista abaixo detalha as seções no curso.

### Thursday, 21 September

| Início | - | Fim (duração) | Título | 
|--------|---|-----|--------|
|11:30	|–|	12:30 (60 mins) |	Practical session (1): code build/ctest, obs conversion, hofx |	
|15:45	|–|	17:00 (75 mins)	| Practical session (2): 3D/4DEnVar with conventional obs	|

### Friday 22 September

| Início | - | Fim (duração) | Título | 
|--------|---|-----|--------|
|11:15   |–|	12:30 (75 mins)|	Practical session (3): 3DVar/Hybrid with satellite radiance|	
|14:50	|–|	16:30 (100 mins)|	Practical session (4): EDA/LETKF, Plot OMB/OMA, Regional|	

Nas atividades práticas houve uma lista de tarefas a serem desenvolvidas pelos participantes. As instruções para as aulas práticas estão disponives no link https://www2.mmm.ucar.edu/projects/mpas-jedi/tutorial/202309NCAR/.

A lista de atividades são as que se segue:

0. Pré-requisitos e configuração do ambiente
1. Compilando/Testando MPAS-JEDI
2. Convertendo NCEP BUFR obs para o formato IODA-HDF5
3. Executando o aplicativo HofX do MPAS-JEDI
4. Gerando arquivos de localização e executando 3D/4DEnVar com obs "convencionais"
5. Executando 3DVar e hybrid-3DEnVar
6. Executando EDA e LETKF
7. Traçando OMB/OMA a partir de dois experimentos
8. Executando MPAS-JEDI regional


## Repositório dos dados usados nos exercicios na máquina cheyenne.ucar.edu
Uma cópia fiel de todo a estrutura de diretórios criadas durante o curso usando o ambiente da maquina cheyenne.ucar.edu foi copiado para um repositório ftp do CPTEC e nele tdos podem acessar os dados usados e os resultados dos exercícios realizados. Esses dados não são colocados no reposiório do GitHub por conter uma grande quantidades de dados binários ou dados netcdf finais nada compactos e que ficaria inviavel o uso e desconfiguraria o ambiente para que ele foi criado, por isso se optou por um ambiente ftp, uma vez que é apenas para ser acessado visualizado, mas não baixado ou compilado.

Todo o conjunto de dados disponivel está disponivel no endereço:

http://ftp1.cptec.inpe.br/pesquisa/das/MPAS-Tutorial-NCAR-2023/mpas_jedi_tutorial/

A estrutura de diretório é ilustrada pela figura abaixo:


<img width="428" alt="Captura de tela 2023-10-19 152252" src="https://github.com/GAD-DIMNT-CPTEC/tutoriais/assets/105943057/84681a8a-3890-49ec-afec-93237552cd91">



