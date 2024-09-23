# Exercicio de Estrutura de Dados 2

Na escola oferece 5 cursos de tecnologia, cada um contendo 12 disciplinas.

Os alunos se inscrevem para as disciplinas, que podem ter, no máximo, 15 alunos inscritos.
Cada aluno só pode estar matriculado em um único curso e estar inscrito simultaneamente em, no máximo 6 disciplinas.

Utilize o diagrama de classes abaixo para implementar a solução:
## Aluno
| Campo               | Tipo   |
|---------------------|--------|
| id                  | int    |
| nome                | string |

**Métodos:**
- `podeMatricular(Cursos cursos): bool`

---

## Disciplina
| Campo               | Tipo       |
|---------------------|------------|
| id                  | int        |
| descricao           | string     |
| alunos              | Aluno[15]  |

**Métodos:**
- `matricularAluno(Aluno aluno): bool`
- `desmatricularAluno(Aluno aluno): bool`

---

## Curso
| Campo               | Tipo           |
|---------------------|----------------|
| id                  | int            |
| descricao           | string         |
| disciplinas         | Disciplina[12] |

**Métodos:**
- `adicionarDisciplina(Disciplina disciplina): bool`
- `pesquisarDisciplina(Disciplina disciplina): Disciplina`
- `removerDisciplina(Disciplina disciplina): bool`

---

## Escola
| Campo               | Tipo     |
|---------------------|----------|
| cursos              | Curso[5] |

**Métodos:**
- `adicionarCurso(Curso curso): bool`
- `pesquisarCurso(Curso curso): Curso`
- `removerCurso(Curso curso): bool`


### Opções no seletor:
0. Sair
1. Adicionar curso
2. Pesquisar curso (mostrar inclusive as disciplinas associadas)
3. Remover curso (não pode ter nenhuma disciplina associada)
4. Adicionar disciplina no curso
5. Pesquisar disciplina (mostrar inclusive os alunos matriculados)
6. Remover disciplina do curso (não pode ter nenhum aluno matriculado)
7. Matricular aluno na disciplina
8. Remover aluno da disciplina
9. Pesquisar aluno (informar seu nome e em quais disciplinas ele está matriculado) 
