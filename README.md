# 🎓 REST API de Professores (Projeto de Bimestre)

Um projeto simples, desenvolvido como trabalho de bimestre do curso técnico, para construir uma API RESTful em **Python** utilizando **Flask**.

Esta aplicação permite gerenciar um cadastro de Professores (CRUD completo: criar, ler, atualizar e deletar) e foi desenvolvida para consolidar conceitos de desenvolvimento back-end, roteamento e organização no padrão MVC (Model-View-Controller).

---

## 🚀 Tecnologias Utilizadas

- **Python** 🐍
- **Flask** 🌶️ (Microframework web)
- Padrão arquitetural **MVC**

## 📂 Estrutura do Projeto

O projeto está organizado da seguinte forma:

- `app.py`: Arquivo principal que inicializa a aplicação Flask e define as rotas da API.
- `controle/`: Diretório contendo os controladores (ex: `ProfessorController`), responsáveis pelas regras de negócio e interações.
- `model/`: Diretório que contém os modelos de dados (ex: `Professor`).
- `router/`: (Possíveis rotas ou configurações adicionais).

## ⚙️ Funcionalidades (Endpoints)

A API roda localmente na porta `8080` (`http://localhost:8080`) e expõe os seguintes endpoints:

### Professores

| Método | Endpoint | Descrição |
|---|---|---|
| `GET` | `/professor/flask` | Retorna a lista de todos os professores cadastrados. |
| `GET` | `/professor/flask/<id>` | Busca um professor específico pelo seu ID. |
| `POST` | `/professor/flask` | Cria um novo professor. |
| `PUT` | `/professor/flask/<id>` | Atualiza os dados de um professor existente. |
| `DELETE` | `/professor/flask/<id>` | Remove um professor do sistema. |

### Exemplo de Payload para Criação (`POST` e `PUT`):

Para criar ou atualizar um professor, envie um JSON no corpo da requisição com a seguinte estrutura:

```json
{
  "professor": {
    "nome": "Nome do Professor",
    "email": "email@exemplo.com",
    "data_nascimento": "1980-01-01",
    "senha": "senha_segura"
  }
}
```

## 🛠️ Como Executar o Projeto

1. Certifique-se de ter o **Python** instalado em sua máquina.
2. Instale as dependências necessárias, como o Flask (recomendado usar um ambiente virtual):
   ```bash
   pip install flask
   ```
3. Execute o arquivo principal da aplicação:
   ```bash
   python app.py
   ```
4. A API estará disponível e aguardando requisições em: `http://0.0.0.0:8080`

---
*Projeto desenvolvido para fins educacionais.* 📚
