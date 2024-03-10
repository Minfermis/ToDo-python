# ToDo App

Este é um aplicativo To-Do simples desenvolvido usando a biblioteca Flet (ft) para interface gráfica e SQLite para armazenamento de dados. O aplicativo permite ao usuário adicionar, marcar como concluída ou não concluída, e visualizar suas tarefas.

## Funcionalidades

### 1. Adição de Tarefas

O usuário pode adicionar novas tarefas digitando o nome da tarefa na caixa de texto e clicando no botão de adição.

### 2. Marcação de Conclusão

Cada tarefa é exibida na forma de uma caixa de seleção que o usuário pode marcar como concluída ou não concluída. A atualização do status da tarefa é refletida automaticamente no banco de dados.

### 3. Visualização de Tarefas

O usuário pode alternar entre três abas para visualizar todas as tarefas, tarefas em andamento (não concluídas) e tarefas concluídas.

## Estrutura do Código

- **Classe Principal:** `ToDo` é a classe principal do aplicativo que gerencia a interface e interage com o banco de dados SQLite.

- **Funções Principais:**
  - `db_execute(query, params=[]):` Função para executar consultas no banco de dados SQLite.
  - `set_value(e):` Função para definir o valor da tarefa com base na entrada do usuário.
  - `add(e, input_task):` Função para adicionar uma nova tarefa ao banco de dados.
  - `checked(e):` Função chamada quando uma tarefa é marcada como concluída ou não concluída.
  - `tasks_container():` Função para criar o contêiner de tarefas.
  - `update_task_list():` Função para atualizar a lista de tarefas exibida.
  - `tabs_changed(e):` Função chamada quando as abas de visualização são alteradas.
  - `main_page():` Função para criar a página principal do aplicativo.

## Como Executar

Certifique-se de ter as bibliotecas Flet (`flet`) e SQLite (`sqlite3`) instaladas em seu ambiente Python. Você pode instalar essas bibliotecas usando o seguinte comando:

```bash
pip install flet
