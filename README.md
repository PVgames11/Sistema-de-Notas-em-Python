

---

# Sistema de Notas

## Descrição

Este é um sistema de gerenciamento de notas de alunos desenvolvido em Python utilizando SQLite como banco de dados. O sistema permite criar tabelas de alunos e notas, inserir dados, atualizar, remover e consultar informações. Este projeto foi desenvolvido como parte de um trabalho para a faculdade.

## Funcionalidades

1. **Criar tabela de alunos**: Cria a tabela para armazenar informações dos alunos.
2. **Criar tabela de notas**: Cria a tabela para armazenar as notas dos alunos.
3. **Inserir alunos**: Adiciona novos alunos ao banco de dados.
4. **Inserir notas**: Adiciona novas notas para os alunos.
5. **Remover aluno**: Remove um aluno do banco de dados.
6. **Remover nota**: Remove uma nota específica de um aluno.
7. **Atualizar dados do aluno**: Atualiza as informações de um aluno.
8. **Atualizar notas**: Atualiza uma nota específica de um aluno.
9. **Consultar dados**: Consulta informações de alunos ou notas.
10. **Finalizar programa**: Encerra o programa.

## Requisitos

- Python 3.x
- SQLite

## Como usar

1. Clone o repositório para o seu ambiente local:
    ```bash
    git clone https:https://github.com/PVgames11/Sistema-de-Notas-em-Python
    ```
2. Navegue até o diretório do projeto:
    ```bash
    cd sistema-de-notas
    ```
3. Execute o script principal:
    ```bash
    python sistema_notas.py
    ```

## Estrutura do Banco de Dados

### Tabela `alunos`

| Campo     | Tipo    | Descrição                       |
|-----------|---------|---------------------------------|
| matricula | INTEGER | Chave primária, matrícula única |
| nome      | TEXT    | Nome do aluno                   |
| idade     | INTEGER | Idade do aluno                  |
| sexo      | TEXT    | Sexo do aluno                   |
| serie     | TEXT    | Série em que o aluno estuda     |

### Tabela `notas`

| Campo     | Tipo    | Descrição                       |
|-----------|---------|---------------------------------|
| id        | INTEGER | Chave primária, auto incremento |
| matricula | INTEGER | Matrícula do aluno              |
| trimestre | TEXT    | Trimestre da nota               |
| materia   | TEXT    | Matéria da nota                 |
| nota      | REAL    | Nota obtida                     |

## Funcionalidades Detalhadas

### Criar Tabelas

- **alunos**: Cria a tabela `alunos` se não existir.
- **notas**: Cria a tabela `notas` se não existir.

### Inserir Dados

- **Inserir alunos**: Adiciona um novo aluno ao banco de dados. Solicita matrícula, nome, idade, sexo e série do aluno.
- **Inserir notas**: Adiciona uma nova nota para um aluno existente. Solicita matrícula, trimestre, matéria e nota.

### Atualizar Dados

- **Atualizar dados do aluno**: Permite atualizar o nome, idade e série de um aluno existente.
- **Atualizar notas**: Permite atualizar a nota de uma matéria específica de um aluno.

### Remover Dados

- **Remover aluno**: Remove um aluno do banco de dados usando a matrícula.
- **Remover nota**: Remove uma nota específica de um aluno usando a matrícula e a matéria.

### Consultar Dados

- **Consultar dados**: Permite consultar todas as informações dos alunos ou notas, ou consultar dados específicos usando a matrícula.

## Observações

- Certifique-se de que o banco de dados `alunos.db` esteja no mesmo diretório do script Python.
- As operações de inserir, atualizar e remover dados são confirmadas apenas após a confirmação do usuário.

## Contribuição

Se desejar contribuir com o projeto, sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

### Contato

Paulo Vitor Silva Quintanilha - paulovitorstark@gmail.com

---

