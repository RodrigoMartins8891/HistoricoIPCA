# 📈 HistoricoIPCA - API de Consulta e Histórico do IPCA

## Visão Geral do Projeto

O **HistoricoIPCA** é uma API (Application Programming Interface) RESTful desenvolvida para fornecer dados históricos e informações sobre o **Índice Nacional de Preços ao Consumidor Amplo (IPCA)**.

Este projeto Full Stack (Back-End) foi essencial para consolidar meu conhecimento em:
1.  Criação de APIs robustas com Node.js e Express.
2.  **Orquestração de dados** (seja de uma fonte externa ou interna).
3.  Processo de **Deploy e Hospedagem** em um servidor real (Render).

### Acesso à API

A API está totalmente funcional e disponível publicamente:

**URL Base:** [**https://projetohistoricoipca-cmlg.onrender.com**](https://projetohistoricoipca-cmlg.onrender.com) 👈 **Destaque Importante!**

## ⚙️ Tecnologias Utilizadas (Stack Back-End)

| Categoria | Tecnologia | Descrição |
| :--- | :--- | :--- |
| **Linguagem** | **JavaScript** (ES6+) | Linguagem de programação principal. |
| **Runtime** | **Node.js** | Ambiente de execução do servidor. |
| **Framework** | **Express.js** | Framework web utilizado para roteamento e construção da API REST. |
| **Banco de Dados** | MongoDB / PostgreSQL / JSON File (Qual você usou?) | Sistema de gestão para armazenamento dos dados históricos. |
| **Hospedagem** | **Render** | Serviço utilizado para o *deploy* e manutenção do servidor em produção. |
| **Outros** | Axios / Fetch (para busca de dados) | Se a API consome dados de uma fonte externa. |

## 🚀 Funcionalidades e Endpoints da API

A API fornece os seguintes recursos principais (Endpoints):

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| **GET** | `/api/ipca/historico` | Retorna o histórico completo do IPCA. |
| **GET** | `/api/ipca/mes/:mes_ano` | Retorna o valor do IPCA para um mês e ano específicos (Ex: `/api/ipca/mes/10-2023`). |
| **GET** | `/api/ipca/periodo` | Aceita query parameters `data_inicial` e `data_final` para buscar um intervalo (Ex: `?data_inicial=2020-01&data_final=2023-12`). |
| **POST** | `/api/ipca/atualizar` | (Opcional) Endpoint protegido para alimentar ou atualizar o banco de dados. |

## 🧠 Aprendizados e Desafios

O desenvolvimento desta API me proporcionou experiência prática em:

* **Roteamento RESTful:** Definição e gestão correta de rotas (GET, POST, etc.) seguindo os princípios de uma API REST.
* **Conexão com Banco de Dados:** (Se aplicável) Manipulação e consulta de dados persistentes.
* **Gerenciamento de Servidor:** Configuração de *scripts* de inicialização e variáveis de ambiente (`.env`).
* **Deploy Contínuo (CI/CD Básico):** Compreensão do processo de *build* e *deploy* automatizado via Render.

## 🛠️ Como Rodar Localmente

Siga os passos para configurar e executar a API em seu ambiente de desenvolvimento.

### Pré-requisitos

* Node.js instalado (versão 14+).
* Um gerenciador de pacotes (npm ou Yarn).

### Instalação

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/RodrigoMartins8891/HistoricoIPCA.git](https://github.com/RodrigoMartins8891/HistoricoIPCA.git)
    cd HistoricoIPCA
    ```

2.  **Instale as dependências:**
    ```bash
    npm install
    ```

3.  **Configuração de Variáveis de Ambiente:**
    Crie um arquivo chamado `.env` na raiz do projeto e adicione as variáveis necessárias (Ex: `PORT=3000`, `DATABASE_URL=...`).

4.  **Inicie o Servidor:**
    ```bash
    npm start
    ```

O servidor estará rodando em `http://localhost:3000` (ou na porta configurada).

## 🤝 Contato

([https://www.linkedin.com/in/rodrigo-martins-de-oliveira1988/])

**Rodrigo Martins** - Desenvolvedor Back-End em Formação
