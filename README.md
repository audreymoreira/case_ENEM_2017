Análise dos dados do MICRODADOS_ENEM_2017
Audrey Moreira – novembro de 2022
TRABALHO EM PROGRESSO

       1. Descrição da análise
O ENEM (Exame Nacional do Ensino Médio ou gratuitamente, Exame Nacional do Ensino Médio) foi criado em 1998, com o objetivo de avaliar o desempenho dos alunos que concluem o ensino médio. A partir de 2004, a prova passou a ser utilizada como instrumento de ingresso em instituições de ensino superior e, em 2010, com sua inclusão no Sistema de Seleção Unificada (Sisu), foi reconhecida como o maior e mais completo exame educacional do Brasil.
Neste projeto, os resultados deste exame foram examinados. Mais de 6 milhões de alunos foram inscritos para o exame em 2017.
Os microdados do ENEM são o nível mais baixo de desagregação dos dados coletados por meio do exame. Eles atendem à demanda de informações específicas por meio da disponibilização das provas, dos gabaritos, das informações sobre os itens, das notas e do questionário respondido pelos inscritos no Enem.
Fontes:
https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem
Neste link está o arquivo de microdados do ENEM 2017, objeto deste case técnico:
https://download.inep.gov.br/microdados/microdados_enem_2017.zip

2. Objetivo deste projeto
O objetivo principal é obter insights sobre este processo tão importante de medição de desempenho educacional que, em última análise, é o ENEM, este grande exame nacional de estudantes no Brasil.

3. Status do Projeto
Este é um trabalho em andamento, que será refinado e ampliado adicionando evolução no tempo, por exemplo.

4. Sequência de trabalho

    • O tamanho do arquivo
O primeiro problema que enfrentei foi como abrir/visualizar o arquivo MICRODADOS_ENEM_2017.csv, devido ao seu “tamanho grande”, quase 3GB. Nunca tratei um arquivo desse tamanho, então foi um aprendizado, aprender fazendo.
    • Colunas escolhidas
      Optei por reduzir a carga de memória e o tempo de processamento, definindo colunas (recursos) para carregar e analisar.

    01. 'TP_ESCOLA'			Tipo de escola do Ensino Médio (Pública, Privada, Exterior)
    02. 'NO_MUNICIPIO_PROVA'	Nome do município da escola
    03. 'SG_UF_PROVA'		Sigla da Unidade da Federação da escola
    04. 'TP_PRESENCA_CN'	 	Presença na prova de Ciências Naturais
    05. 'TP_PRESENCA_MT'		Presença na prova de Matemática
    06. 'TP_PRESENCA_CH'		Presença na prova de Ciências Humanas
    07. 'TP_PRESENCA_LC'	 	Presença na prova de Linguagens e Códigos
    08. 'NU_NOTA_CH'		Nota da prova de Ciências Humanas
    09. 'NU_NOTA_CN'		Nota da prova de Ciências Naturais
    10. 'NU_NOTA_LC'		Nota da prova de Ciências 
    11. 'NU_NOTA_MT'	Nota da prova de Matemática 
    12. 'NU_NOTA_REDACAO'	Nota da prova de Redação 
    13. 'Q001'	Até que série seu pai, ou o homem responsável por você, estudou?
    14. 'Q002'	Até que série sua mãe, ou a mulher responsável por você, estudou?
    15. 'Q006'	Qual é a renda mensal de sua família? (Some a sua renda com a dos seus familiares.)
    16. 'Q025'	Na sua residência tem acesso à Internet?

      • A nota final do aluno (‘NOTA_FINAL’) neste exame é obtida através do cálculo da média aritmética das suas cinco notas: ‘NU_NOTA_CH’, ‘NU_NOTA_CN’, ‘NU_NOTA_LC’, ‘NU_NOTA_MT’ e ‘NU_NOTA_REDACAO’.
    • Análises Efetuadas:
    a) Distribuição total de notas com todo o dataframe enem_2017, desconsiderando os alunos ausentes.
    b) Madiana da Nota Final
    c) Alunos ausentes: número em relação ao total
    d) Maior nota final, quanto e de onde
    e) Análise por tipo de Escola
    f) Distribuição de Estudantes por Faixa de Renda
    g) Relação entre Renda Familiar e Nota Final
    h) Nota Final por Estados e Regiões
    i) O Estado com a maior nota, menor nota (Nota Final e de Redação)
    j) Aquisição de arquivo externo com IDHM e IDHM Renda por Estado e por Região
    k) Correlação entre os Índices e a Nota Final
    l) Desempenho por Reistribuição de notas por Cidades
    m) Influência do grau de instrução de Pais e Mães
    n) Ter Internet em casa e a influência nas notas
    o) Heatmap para correlação entre a população das cidades e as notas.

Este é um trabalho em andamento.
Mais desenvolvimentos envolvem, por exemplo, a evolução histórica das análises executadas aqui.
Caso você queira enviar sugestões, elas serão muito apreciadas! Obrigada!
Audrey Moreira

