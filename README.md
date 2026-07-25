# Banco de Dados - NSA Simplificado

Este repositório reúne uma atividade desenvolvida com o objetivo de praticar a estrutura de um Banco de Dados e o desenvolvimento do mesmo utilizando o MySql Workbench.

## Conteúdo
Projeto desenvolvido em MySQL para simular o aplicativo NSA.

## Funcionalidades
- Cadastro de cursos
- Cadastro de turmas (por módulo/semestre e curso)
- Cadastro de alunos
- Cadastro de professores
- Cadastro de componentes curriculares
- Vínculo de docência (professor ↔ componente curricular)
- Cadastro de atividades (trabalhos) por componente curricular
- Lançamento de notas por aluno e atividade, incluindo nota 0 para atividades não realizadas

## Tecnologias
- MySQL

## Conceitos aplicados
- Modelagem relacional
- Chaves primárias e estrangeiras
- Integridade referencial
- Relacionamento N:N via tabela associativa (tb_docencia)
- DDL (CREATE, ALTER)
- DML (INSERT, DELETE)

## Estrutura do banco

tb_curso → tb_turma → tb_aluno
                    → tb_componente_curricular → tb_atividade → tb_nota
tb_professor → tb_docencia ← tb_componente_curricular

## Dados cadastrados
- 2 cursos (Informática e Administração)
- 6 turmas (1º, 2º e 3º semestre de cada curso)
- 60 alunos (10 por turma)
- 30 componentes curriculares (5 por semestre/curso, extraídos dos Planos de Curso oficiais)
- 16 professores (8 de Informática e 8 de Administração)
- 60 atividades (2 trabalhos por componente curricular)
- 600 notas (todos os alunos avaliados em todas as atividades da sua turma, com nota 0 para quem não realizou a atividade)

## Autor

Desenvolvido por **Celine** durante as aulas de Banco de Dados na ETEC Adolpho Berezin.
