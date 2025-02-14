# 💰 Sistema de Movimentação de Dinheiro

## 📝 Sobre  
Este projeto permite a gestão de contas bancárias, incluindo movimentações financeiras, transferências e geração de gráficos.  

## 🚀 Tecnologias  
As tecnologias utilizadas neste projeto são:  

- ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)  
- ![SQLModel](https://img.shields.io/badge/-SQLModel-4479A1?logo=sqlite&logoColor=white)  
- ![SQLite](https://img.shields.io/badge/-SQLite-003B57?logo=sqlite&logoColor=white)  
- ![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?logo=plotly&logoColor=white)

## 🚀 Funcionalidades

- ✅ Criar contas bancárias associadas a um banco específico  
- ✅ Registrar entradas e saídas de dinheiro  
- ✅ Validar saldo antes de saídas  
- ✅ Impedir movimentações em contas inativas  
- ✅ Transferir saldo entre contas  
- ✅ Desativar contas (desde que sem saldo)  
- ✅ Exibir histórico de transações filtrado por data  
- ✅ Gerar gráficos com os valores de cada conta  

---

## 📂 Estrutura do Projeto

```bash
/app_financeiro
│── models.py       # Definição das classes e do banco de dados
│── view.py         # Funções para manipulação de contas e transações
│── templates.py    # Interface em linha de comando para interação com o usuário
│── requirements.txt # Dependências do projeto
│── README.md       # Documentação

```
## ⚡ Como Rodar o Projeto

### 1️⃣ Clonar o repositório
```sh
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```
### 2️⃣ Criar um ambiente virtual e ativá-lo
```sh
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate  # Windows
```
### 3️⃣ Instalar dependências
```sh
pip install -r requirements.txt
```
### 4️⃣ Criar o banco de dados
```sh
python models.py
```
### 5️⃣ Executar a aplicação
```sh
python templates.py
```
## 🏦 Como Funciona?

🔹` models.py`

Define as classes Conta e Historico, além do banco de dados e enumerações para Bancos, Status e Tipos de movimentação.

🔹 `view.py`


Contém as funções principais do sistema:

- Criar contas
- Listar contas
- Desativar contas
- Transferir saldo
- Movimentar dinheiro
- Buscar históricos de transações
- Gerar gráficos

🔹 `templates.py`

Interface de linha de comando (CLI) para interação do usuário, permitindo criar contas, transferir dinheiro, visualizar o total disponível e gerar gráficos.

## 📊 Exemplo de Uso
Criando uma conta via código:
```sh
python

from models import Conta, Bancos
from view import criar_conta

nova_conta = Conta(banco=Bancos.NUBANK, valor=500.0)
criar_conta(nova_conta)
```
Movimentando dinheiro:
```
python

from models import Historico, Tipos
from view import movimentar_dinheiro
from datetime import date

historico = Historico(conta_id=1, tipo=Tipos.ENTRADA, valor=100.0, data=date.today())
movimentar_dinheiro(historico)
```
## 📜 Licença
Este projeto está sob a licença MIT. Sinta-se livre para usá-lo e contribuir! 🚀
