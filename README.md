# 🧪 Projeto de Testes de API – Restful Booker

🚀 Projeto desenvolvido para validar a API **[Restful-Booker](https://restful-booker.herokuapp.com/apidoc/index.html)**, explorando **testes manuais com Postman** e aplicando boas práticas de **documentação, rastreabilidade e versionamento com GitHub e Trello**.

---

## 🎯 Objetivo

Executar e documentar testes manuais em uma API REST, cobrindo **operações CRUD completas** e **cenários negativos**, simulando situações reais de uso.

---

## 🧰 Tecnologias Utilizadas

| Ferramenta | Finalidade |
|-------------|-------------|
| 🧪 **Postman** | Criação e execução das requisições |
| 🧾 **JSON** | Corpo das requisições e validações das respostas |
| 💻 **GitHub** | Versionamento e portfólio do projeto |
| 📋 **Trello** | Organização do fluxo de testes |
| 📊 **Google Sheets** | Documentação e rastreabilidade dos testes |

---

## 📁 Estrutura do Projeto

```bash
QA-Restful-Booker/
│
├── evidence/                     # Evidências dos testes (prints)
│   ├── CT01_token_gerado.png
│   ├── CT02_criar_reserva.png
│   ├── CT03_consultar_reserva.png
│   ├── CT04_atualizar_reserva.png
│   ├── CT05_excluir_reserva.png
│   ├── CT06_sem_token.png
│   ├── CT07_body_invalido.png
│   ├── CT08_id_inexistente.png
│   ├── CT09_bug200_token_invalido.png
│
├── README.md
└── Test_Cases.xlsx               # Planilha com os casos de teste
