# 💰 Sistema de Movimentação de Dinheiro

Este projeto gerencia movimentações financeiras em contas bancárias, garantindo segurança e consistência nas transações.

## 🚀 Funcionalidades

✅ Criar contas bancárias associadas a um banco específico  
✅ Registrar entradas e saídas de dinheiro  
✅ Validar saldo antes de saídas  
✅ Impedir movimentações em contas inativas  
✅ Transferir saldo entre contas  
✅ Desativar contas (desde que sem saldo)  
✅ Exibir histórico de transações filtrado por data  
✅ Gerar gráficos com os valores de cada conta  

## 🛠 Tecnologias Usadas

- **Python** 🐍  
- **SQLModel** (para manipulação do banco de dados)  
- **SQLite** / **PostgreSQL** (dependendo do ambiente)  
- **Matplotlib** (para gráficos)  

## 📂 Estrutura do Projeto

/seu-projeto │── models.py # Definição das classes e do banco de dados │── view.py # Funções para manipulação de contas e transações │── templates.py # Interface em linha de comando para interação com o usuário │── requirements.txt # Dependências do projeto │── README.md # Documentação

bash
Copiar
Editar

## ⚡ Como Rodar o Projeto

### 1️⃣ Clonar o repositório
```sh
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

