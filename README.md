
# Lista de Compras

Aplicativo Android desenvolvido em Kotlin para ajudar no gerenciamento de listas de compras de forma simples, eficiente e intuitiva.

## 📱 Funcionalidades

- ✅ Adicionar itens à lista de compras
- ✅ Remover itens da lista
- ✅ Marcar itens como comprados
- ✅ Visualizar a lista de compras de forma prática

---

## 🏗️ Estrutura do Projeto

O projeto segue uma estrutura simples, porém bem organizada:

```
app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── carreiras/com/github/listadecompras/
│   │   │       ├── MainActivity.kt
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   │   └── activity_main.xml
│   │   │   ├── values/
│   │   │   └── drawable/
│   │   └── AndroidManifest.xml
├── build.gradle.kts
└── settings.gradle.kts
```

---

## 🗄️ Integração com Banco de Dados (SQLite)

O aplicativo utiliza o banco de dados **SQLite** nativo do Android para persistência de dados. Através dele, os itens da lista são armazenados localmente no dispositivo, permitindo que os dados permaneçam mesmo após fechar o app.

- 📦 Implementação feita utilizando classes auxiliares (`SQLiteOpenHelper`) para criação, atualização e gerenciamento do banco.
- ✔️ Operações realizadas:
  - **INSERT:** Para adicionar itens.
  - **SELECT:** Para listar todos os itens.
  - **UPDATE:** Para marcar como comprado ou alterar informações.
  - **DELETE:** Para remover itens.

---

## 🔄 RecyclerView

O aplicativo faz uso do **RecyclerView**, que é uma das principais ferramentas da interface Android para listas dinâmicas e performáticas.

- 🔥 Vantagens do RecyclerView:
  - Alta performance, mesmo com grandes quantidades de dados.
  - Possibilidade de customização de cada item da lista.
  - Suporte a clique nos itens (como remover ou marcar como comprado).

- 🛠️ Componentes:
  - **Adapter:** Responsável por criar e vincular os dados aos itens da lista.
  - **ViewHolder:** Define a interface visual de cada item.
  - **LayoutManager:** Controla o layout (Linear, Grid, etc.) — neste projeto é usado o **LinearLayoutManager** (lista vertical).

---

## 🧠 Conceitos e Tecnologias Envolvidas

- **Kotlin:** Linguagem principal do desenvolvimento.
- **Android SDK:** Ferramentas nativas do Android.
- **RecyclerView:** Para exibição da lista dinâmica de itens.
- **SQLite:** Banco de dados local para persistência dos itens.
- **Material Design:** Uso de componentes visuais seguindo as diretrizes do Google.
- **Ciclo de Vida de Atividades:** Manipulação correta de dados e interface de acordo com o ciclo de vida da `MainActivity`.
- **Validação de dados:** Garante que não sejam adicionados itens vazios ou inválidos.

---

## 🚀 Como executar o projeto

1. Clone este repositório:

```bash
git clone https://github.com/joavlr03/ListaDeComprasKotlin.git
```

2. Abra o projeto no **Android Studio**.

3. Aguarde a sincronização do Gradle.

4. Conecte um dispositivo físico Android ou configure um emulador.

5. Clique em **Run (▶️)** no Android Studio para executar o aplicativo.

----

## 📄 Sobre

Este projeto foi desenvolvido com o objetivo de praticar o desenvolvimento Android utilizando Kotlin, aplicando conceitos de persistência de dados, criação de interfaces dinâmicas e uso das ferramentas nativas do Android.
