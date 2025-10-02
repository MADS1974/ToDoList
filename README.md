# 📝 ToDoList App

Um aplicativo Android para gerenciamento de listas de tarefas (**To-Do List**) desenvolvido em **Kotlin**.  
O objetivo principal é demonstrar a implementação de uma **arquitetura moderna** com Room, ViewModel e Navegação por Fragmentos, além de ilustrar operações **CRUD** (Criar, Ler, Atualizar, Excluir) em um banco de dados local.

Este projeto foi criado para fins acadêmicos no contexto da disciplina de **Desenvolvimento de Aplicações Móveis**, com foco em:

- Arquitetura **MVVM** (Model-View-ViewModel) para separação de responsabilidades  
- Uso de **Room** para persistência de dados local  
- Navegação entre **Fragmentos** com Navigation Component  
- Gerenciamento de estado com **ViewModel** e **LiveData**  
- Interação do usuário com listas de dados usando **RecyclerView** e **ListAdapter**  

---

## 🚀 Funcionalidades

✔️ **Listagem de Tarefas**: Exibe uma lista de tarefas em um RecyclerView  
➕ **Adicionar Nova Tarefa**: Abre um novo fragmento para preenchimento dos dados  
✏️ **Editar Tarefa**: Através de um menu de contexto (pressionar e segurar), abre a tela de edição com os dados já preenchidos  
🗑️ **Remover Tarefa**: Também pelo menu de contexto, permite excluir tarefas do banco de dados  
✅ **Marcar como Concluída**: Um CheckBox em cada item permite marcar/desmarcar como concluída  
💾 **Persistência de Dados**: As tarefas são salvas localmente e permanecem mesmo após fechar o app  
🎨 **Estilização Personalizada**: Fundo roxo arredondado nos itens via **Drawable Shape XML**  

---

## 🛠 Tecnologias Utilizadas

- **Kotlin** — Linguagem principal  
- **Android Studio** — IDE de desenvolvimento  
- **ViewBinding** — Acesso seguro e tipado aos elementos de UI  
- **Room Persistence Library** — Abstração sobre o SQLite para persistência robusta  
- **ViewModel** — Gerenciamento de estado e dados da UI  
- **LiveData** — Observação de dados reativa e consciente do ciclo de vida  
- **Navigation Component** — Navegação entre Fragmentos  
- **RecyclerView com ListAdapter** — Lista otimizada com DiffUtil  
- **Menus (Options e Context)** — Ações como adicionar, editar e remover  

---

📸 Demonstração do App
01 - Tela Principal

Exibição da lista de tarefas. O botão ➕ FloatingActionButton permite adicionar novas tarefas.
<img src="screens/1%20ToDoList.png" alt="Tela Principal" width="400"/>

02 - Adicionar/Editar Tarefa

Formulário para criar ou editar uma tarefa.
<img src="screens/2%20ToDoList.png" alt="Adicionar/Editar Tarefa" width="400"/>

03 - Lista de Tarefas Criadas

As tarefas aparecem na lista com fundo roxo arredondado.
<img src="screens/3%20ToDoList.png" alt="Lista de Tarefas" width="400"/>

▶️ Como Executar o Projeto

Clone este repositório:

git clone https://github.com/MADS1974/ToDoList


Abra o projeto no Android Studio
Aguarde a sincronização do Gradle
Execute em um emulador ou dispositivo físico

📚 Créditos

Projeto acadêmico desenvolvido para a disciplina Desenvolvimento para Android 1 – D1DA1, ministrada pelo professor Pedro Northon Nobile (IFSP).


## 📂 Estrutura do Projeto

```bash
ToDoList/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/br/edu/ifsp/scl/sdm/todolist/
│   │   │   │   ├── controller/
│   │   │   │   │   └── TaskViewModel.kt        # ViewModel para lógica de negócio
│   │   │   │   ├── model/
│   │   │   │   │   ├── database/
│   │   │   │   │   │   └── ToDoListDatabase.kt # Configuração do Room
│   │   │   │   │   ├── dao/
│   │   │   │   │   │   └── TaskDao.kt          # Queries SQL
│   │   │   │   │   └── entity/
│   │   │   │   │       └── Task.kt             # Entidade da tabela
│   │   │   │   └── view/
│   │   │   │       ├── adapter/
│   │   │   │       │   └── TaskAdapter.kt      # Adaptador do RecyclerView
│   │   │   │       ├── MainFragment.kt         # Lista de tarefas
│   │   │   │       └── TaskFragment.kt         # Adicionar/editar tarefa
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── fragment_main.xml
│   │   │   │   │   ├── fragment_task.xml
│   │   │   │   │   └── tile_task.xml           # Item da lista
│   │   │   │   ├── drawable/
│   │   │   │   │   └── purple_rounded_background.xml # Fundo roxo arredondado
│   │   │   │   ├── menu/
│   │   │   │   └── navigation/
│   │   │   │       └── nav_graph.xml           # Gráfico de navegação
│   │   │   └── AndroidManifest.xml
│   ├── build.gradle.kts (Module :app)
│
├── build.gradle.kts (Project: ToDoList)
└── settings.gradle.kts

---



