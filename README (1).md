# E-Shop Brasil NoSQL - CRUD com MongoDB e Streamlit

Este projeto é uma aplicação de exemplo para a empresa fictícia **E-Shop Brasil**, utilizando tecnologias modernas como **MongoDB**, **Streamlit**, **Docker** e **Python**.

A aplicação permite realizar operações **CRUD** (Criar, Ler, Atualizar e Deletar) em uma base de dados **NoSQL**.

##  Tecnologias Usadas

- **MongoDB** (banco de dados NoSQL)
- **Streamlit** (interface web simples)
- **Docker** (containerizar MongoDB)
- **Python** (linguagem principal)
- **Faker** (geração de dados falsos)

##  Como Rodar o Projeto

### 1. Clone o Repositório
Primeiro, clone este projeto em sua máquina:


git clone https://github.com/seu-usuario/e-shop-brasil-nosql.git
cd e-shop-brasil-nosql


### 2. Suba o MongoDB com Docker
Dentro da pasta principal (`e-shop-brasil-nosql/`), execute:

docker-compose up -d


### 3. Instale as Dependências Python
Entrando na pasta `app/`:


cd app


Instalando as bibliotecas necessárias:


pip install -r requirements.txt


### 4. Gerando os Dados de Exemplo
Executando o gerador de dados para criar **1 milhão** de produtos falsos:


python data_generator.py


### 5. Rode a Aplicação Streamlit
Agora, rode a aplicação com:


streamlit run app.py


O navegador abrirá automaticamente com a interface do sistema.

##  Funcionalidades Disponíveis

- **Adicionar Produto**: cadastrar novos produtos.
- **Listar Produtos**: ver todos os produtos cadastrados.
- **Atualizar Produto**: alterar informações de um produto existente.
- **Deletar Produto**: excluir um produto do banco de dados.

##  Estrutura de Pastas


e-shop-brasil-nosql/
│
├── docker-compose.yml
├── README.md
└── app/
    ├── app.py
    ├── crud.py
    ├── db_connection.py
    ├── data_generator.py
    └── requirements.txt
```

##  Configurações Importantes

- O MongoDB roda localmente em `localhost:27017`.
- O banco de dados se chama `eshop_db`.
- A coleção usada é `products`.



Desenvolvido como parte do projeto de modernização de infraestrutura da **E-Shop Brasil**.

## 📽️ Entrega Final

- ✅ Código fonte no GitHub
- ✅ Docker funcionando para MongoDB
- ✅ Geração automática de 1 milhão de registros
- ✅ Aplicação CRUD completa via Streamlit
- ✅ Vídeo explicativo (caso necessário)
