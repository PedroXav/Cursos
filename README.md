# Sistema de Gerenciamento de Cursos

Este projeto é uma aplicação simples em C# que simula o gerenciamento de cursos, disciplinas e alunos em uma escola. Ele permite realizar operações como adicionar e remover cursos, gerenciar disciplinas e matricular ou desmatricular alunos.

## Funcionalidades

A aplicação oferece as seguintes funcionalidades:

### 1. **Adicionar Curso**
   - Permite ao usuário adicionar um novo curso à escola, informando o ID e a descrição do curso.
   - Limite de 5 cursos.

### 2. **Pesquisar Curso**
   - Busca um curso pelo seu ID.
   - Exibe a descrição do curso e uma lista de suas disciplinas associadas.

### 3. **Remover Curso**
   - Remove um curso da escola pelo seu ID, desde que não haja disciplinas associadas ao curso.

### 4. **Adicionar Disciplina ao Curso**
   - Permite adicionar uma disciplina a um curso existente.
   - Limite de 12 disciplinas por curso.
   
### 5. **Pesquisar Disciplina**
   - Busca uma disciplina pelo ID em todos os cursos e exibe os alunos matriculados.

### 6. **Remover Disciplina do Curso**
   - Remove uma disciplina de um curso, desde que não haja alunos matriculados.

### 7. **Matricular Aluno em Disciplina**
   - Matricula um aluno em uma disciplina, verificando se o aluno já está matriculado em 6 ou mais disciplinas e se a disciplina ainda tem vagas disponíveis (máximo de 15 alunos por disciplina).

### 8. **Desmatricular Aluno de Disciplina**
   - Remove um aluno de uma disciplina, baseado no ID do aluno.

### 9. **Pesquisar Aluno**
   - Permite buscar por um aluno pelo nome. A pesquisa verifica todas as disciplinas de todos os cursos e exibe em qual disciplina o aluno está matriculado.

## Estrutura do Projeto

O projeto contém as seguintes classes principais:

### 1. **Escola**
   - Gerencia os cursos da escola (até 5 cursos).
   - Contém métodos para adicionar, pesquisar e remover cursos, além de pesquisar por alunos.

### 2. **Curso**
   - Representa um curso com até 12 disciplinas.
   - Contém métodos para adicionar, pesquisar e remover disciplinas.

### 3. **Disciplina**
   - Representa uma disciplina com até 15 alunos.
   - Contém métodos para matricular e desmatricular alunos.

### 4. **Aluno**
   - Representa um aluno com um ID e nome.
   - Inclui um método para verificar se o aluno pode se matricular em mais disciplinas.

