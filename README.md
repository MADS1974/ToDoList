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

<img src="screen/1%20Tela%20Principal.png" alt="Tela Principal" width="400"/>

02 - Adicionar Tarefa

<img src="screen/2%20Add%20Tarefa.png" alt="Adicionar/Editar Tarefa" width="400"/>


03 - Editar Tarefa

<img src="screen/3%20Editar%20Tarefa.png" alt="Adicionar/Editar Tarefa" width="400"/>

04 - Lista de Tarefas Criadas


<img src="screen/4%20Lista%20de%20Tarefas.png" alt="Lista de Tarefas" width="400"/>

Os itens da lista de tarefas são renderizados com um background roxo e bordas arredondadas, definido via Drawable XML (purple_rounded_background.xml) e aplicado ao layout do item (tile_task.xml).

▶️ Como Executar o Projeto

Clone este repositório:

git clone https://github.com/MADS1974/ToDoList


Abra o projeto no Android Studio
Aguarde a sincronização do Gradle
Execute em um emulador ou dispositivo físico

## 🎥 Vídeo Demonstrativo


👉 [xToDoList.Mp4](./xToDoList.mp4)


## 📚 Créditos

Projeto acadêmico desenvolvido para a disciplina **Desenvolvimento para Android 1 – D1DA1**, ministrada pelo professor **Pedro Northon Nobile (IFSP)**. 


## 🙋‍♂️

🔗 Conecte-se comigo

[LinkedIn - Márcio Adriano](https://www.linkedin.com/in/mads1974/)

