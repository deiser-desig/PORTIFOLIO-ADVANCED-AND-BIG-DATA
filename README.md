# E-Shop Brasil – Integração de Soluções NoSQL com Streamlit
E-Shop Brasil NoSQL - CRUD com MongoDB e Streamlit
Este projeto é uma aplicação de exemplo para a empresa fictícia E-Shop Brasil, utilizando tecnologias modernas como MongoDB, Streamlit, Docker e Python.

A aplicação permite realizar operações CRUD (Criar, Ler, Atualizar e Deletar) em uma base de dados NoSQL

 Tecnologias Usadas
MongoDB (banco de dados NoSQL)

Streamlit (interface web simples)

Docker (containerizar MongoDB)

Python (linguagem principal)

Faker (geração de dados falsos)

1. Clone o Repositório
Primeiro, foi clonado o projeto:
git clone https://github.com/deiser-design/e-shop-brasil-nosql.git
cd e-shop-brasil-nosql

2 Foi subido o MongoDB com Docker
Dentro da pasta principal (e-shop-brasil-nosql/), executado:
docker-compose up -d

Isso vai criar e iniciar um container chamado mongodb ouvindo na porta 27017.


3. Instalando as Dependências Python
Entrando na pasta app/:
cd app

Instalando as bibliotecas necessárias:
pip install -r requirements.txt

4. Gerando os Dados de Exemplo:
Executando o gerador de dados para criar 1 milhão de produtos falsos:
python data_generator.py

5. Rode a Aplicação Streamlit
Agora, rodandando a aplicação com:
streamlit run app.py

E o navegador abrirá automaticamente com a interface do sistema.

Funcionalidades Disponíveis
Adicionar Produto: cadastrar novos produtos.
Listar Produtos: ver todos os produtos cadastrados.
Atualizar Produto: alterar informações de um produto existente.
Deletar Produto: excluir um produto do banco de dados.
Tudo funcionando de forma simples e rápida pela interface!

estrutura de pastas:
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

Configurações Importantes
O MongoDB roda localmente em localhost:27017.

O banco de dados se chama eshop_db.

A coleção usada é products.

Desenvolvido como parte do projeto de modernização de infraestrutura da E-Shop Brasil.







