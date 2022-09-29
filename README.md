# Learn_BrModelo
Avaliação de diagramas de modelo logico e conceitual em Sql

### Integrantes
- Lucas de Arimateia
- João Pedro Araujo



### MODELO CONCEITUAL


![Conceitual_1](https://user-images.githubusercontent.com/93049848/193116716-0b5c2fd3-f397-4913-9e79-0f284dbaa024.png)

### MODELO LOGICO

![Lógico_2](https://user-images.githubusercontent.com/93049848/193116804-6e9c9e36-e233-4e18-a10f-946a9307eaeb.png)

### DESCRIÇÃO DAS TABELAS DO MODELO LÓGICO

## Tabela alunos

Tabela alunos se refere aos dados dos alunos cadastrados na escola. Nela possuímos os atributos/colunas

- MAT: matrícula do aluno/chave primaria da tabela 
- nome: nome do aluno cadastrado
- endereço: mostra a rua onde o aluno se encontra
- cidade: informações sobre a localidade do aluno

## Tabela historico 

Tabela referida ao historico de cada aluno 

- MAT: chave estrangeira
- COD_TURMA:chave estrangeira
- COD_DISC: chave estrangeira 
- COD_PROF: chave estrangeira
- ANO: ano da tabela histórico 
- Frequencia: chave estrangeira 
- Nota: chave estrangeira

## Tabela prof_turma

A função da tabela prof_turma é ligar professor e turma. Nela temos os seguintes atributos/colunas:

- fk_professores_COD_PROF: chave estrangeira referente a tabela professor ( COD_PROF ) 
- fk_turma_COD_TURMA: chave estrangeira referente a tabela ( COD_ TURMA )

## Tabela turma 

A função da tabela turma é referenciar as disciplinas e professores que foram atribuidas a mesma. Nela possuímos os seguintes atribuitos/coluna:

- COD_TURMA:chave primária da tabela 
- COD_PROF: chave estrangeira da tabela 
- COD_DISC: chave estrangeira da tabela 
- horario: horário em que cada turma irá ter
- fk_turma_COD_TURMA: chave estrangeira 

## Tabela professores

A função da tabela professores é armazenar os professores contidos na escola. Nela possuímos os seguintes atributos/colunas:

- COD_PROF: chave primária do professor 
- nome: nome do professor
- endereço: endereço do professor 
- cidade: informações sobre o município do professor

## Tabela disciplina

A função da tabela disciplina é armazenar as disciplinas que o aluno irá possuir. Nela possuímos os seguintes atribuitos/colunas:

- COD_DISC: chave primária da tabela 
- nome_DISC: nome das disciplinas exercidas 
- Carga_Hor: carga horária de cada diciplina 
- fk_Diciplina_COD_DISC: chave estrangeira 

## Tabela Aluno_Historico

A função da tabela aluno histórico é armazenar todos os dados já contidos antes do aluno em um só tabela. Nela possuímos os seguintes atributos/colunas:

- MAT: chave primária da tabela
- nome: nome do aluno 
- endereco: localidade do aluno
- cidade: município atual do aluno
- COD_DISC: chave estrangeira referente as disciplinas exercidas pelo aluno
- COD_TURMA: chave estrangeira referente ao código da turma
- ANO: chave estrangeira referente ao ano de curso letivo do aluno
- frequência: frequência do aluno
- nota: boletim do aluno



