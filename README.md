# PROVA_BD
Avaliação em dupla 

 Integrantes:
 
 - Pedro Cauã
 - Matheus Coelho

### CONCEITUAL


![conceitual](https://user-images.githubusercontent.com/107321701/193120430-f0dd5faf-ffcc-4825-bb0c-fb7184509c11.png)


### LOGICO


![logico](https://user-images.githubusercontent.com/107321701/193120308-f8e81faa-0ea0-458d-a7b1-a99ca6c10132.png)


# DESCRIÇÃO DAS TABELAS DO MODELO LOGICO

## TABELA <i>ALUNO_TURMA_HISTORICO</i>
Tabela <i>ALUNO</i> diz respeito em relação aos dados dos alunos cadastrados nesta escola. É possível encontrar os atributos e colunas:

- matricula: matricula do aluno/chave primária da tabela
- nome: nome do aluno cadastrado
- endereco: endereço do aluno cadastrado nesta escola
- cidade: informação importante referente ao aluno e onde se localiza sua residencia

A tabela <i>TURMA</i> se refere a turma na qual as disciplinas e os  professores foram atribuídos a ela. Nela possuímos os atributos e colunas:

- codigo_turma: chave primária
- codigo_disciplina: chave estrangeira
- codigo_professor: chave estrangeira
- ano: ano em que a turma está
- horario: horario em que cada turma terá, referente as aulas ministradas

A tabela <i>HISTORICO</i> se refere a todas as outras tabelas tornando suas chaves primárias para chaves estrangeiras. Nela encontramos os atributos/colunas:

- codigo_disciplina: chave estrangeira
- codigo_turma: chave estrangeira
- codigo_professor: chave estrangeira
- ano: ano da tabela historico
- matricula: chave estrangeira

## TABELA <i>DISCIPLINAS</i>

Tabela <i>DISCIPLINAS</i> se refere as disciplinas em que a turma que o aluno foi atribuído irá ter. Nela se encontra os atributos e colunas:

- codigo_disciplina: chave primária da tabela
- nome_disciplina: o nome das disciplinas
- carga_horaria: a carga horaria em que cada disciplina terá

## TABELA <i>PROFESSORES</i>

A tabela <i>PROFESSORES</i> se refere aos professores que os alunos terão em cada turma. Nela se encontra os atributos/colunas:

- codigo_professor: chave primária da tabela
- nome: nome do professor
- endereco: endereço do professor
- cidade: informação de onde se localiza sua residencia

## TABELA <i>RELACIONAMENTOS_/1/2</i>

Tabela <i>RELACIONAMENTOS_/1/2</i> tabelas de ligações entre alunos e histórico; turma e histórico; disciplinas e turma; professores e turma. Nela possuímos os atributos/colunas:

- fk_alunos_matricula: chave estrangeira que faz referência a tabela alunos
- fk_turma_codigo_turma: chave estrangeira que faz referência a tabela turma
- fk_disciplinas_codigo_disciplina: chave estrangeira que faz referência a tabela disciplinas
- fk_professores_codigo_professor: chave estrangeira que faz referência a tabela professores



