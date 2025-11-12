🧪 Projeto de Testes de API – Restful Booker
📘 Descrição do Projeto

Este projeto foi desenvolvido com o objetivo de praticar testes manuais de API REST, utilizando o serviço Restful Booker como base.
O foco é demonstrar o processo completo de planejamento, execução, registro de evidências e reporte de defeitos, simulando um fluxo real de QA Júnior em um ambiente profissional.

⚙️ Tecnologias e Ferramentas Utilizadas

Postman → Execução dos testes manuais e validação de requisições/respostas

Google Sheets → Documentação dos casos de teste e resultados

Trello → Gestão e acompanhamento das tarefas e bugs

GitHub → Publicação e versionamento do projeto

JSON → Formato de dados utilizado nas requisições
Projeto-RestfulBooker/
│
├── evidence/                         # Evidências (prints dos testes)
│   ├── CT01_token_gerado.png
│   ├── CT02_criar_reserva.png
│   ├── CT03_consultar_reserva.png
│   ├── CT04_atualizar_reserva.png
│   ├── CT05_excluir_reserva.png
│   ├── CT06_sem_token.png
│   ├── CT07_body_invalido.png
│   ├── CT08_id_inexistente.png
│   ├── CT09_token_invalido.png
│   └── CT01_bug200_token_invalido.png
│
├── collection_RodrigoGarcia.postman_collection.json   # Coleção Postman
├── README.md                                          # Documentação do projeto
└── planilha_casos_teste.xlsx                          # Planilha de testes

| ID   | Caso de Teste                          | Objetivo                               | Status                                 |
| ---- | -------------------------------------- | -------------------------------------- | -------------------------------------- |
| CT01 | Gerar token de autenticação            | Validar login válido                   | ✅ Passou                               |
| CT02 | Criar reserva                          | Criar reserva com dados válidos        | ✅ Passou                               |
| CT03 | Consultar reserva                      | Verificar consulta por ID válido       | ✅ Passou                               |
| CT04 | Atualizar reserva                      | Editar reserva existente               | ✅ Passou                               |
| CT05 | Excluir reserva                        | Remover reserva existente              | ✅ Passou                               |
| CT06 | Criar reserva sem token                | Validar acesso negado sem autenticação | ✅ Passou                               |
| CT07 | Criar reserva com body faltando        | Validar rejeição de payload incompleto | ✅ Passou                               |
| CT08 | Consultar reserva com ID inexistente   | Validar retorno 404 Not Found          | ✅ Corrigido (bug reportado e validado) |
| CT09 | Autenticação com credenciais inválidas | Validar erro 403 Forbidden             | ✅ Passou                               |

| ID do Bug | Descrição                                                             | Status      | Evidência                               |
| --------- | --------------------------------------------------------------------- | ----------- | --------------------------------------- |
| BUG-01    | API retornava **200 OK** ao enviar credenciais inválidas para `/auth` | ✅ Corrigido | evidence/CT01_bug200_token_invalido.png |

Passos para Reproduzir:

Enviar POST /auth com:

{"username": "invalid", "password": "wrong"}


Resultado Esperado: 403 Forbidden

Resultado Obtido (antes da correção): 200 OK – Token inválido

| Indicador               |            Valor            | Observação                   |
| :---------------------- | :-------------------------: | :--------------------------- |
| Total de Casos de Teste |            **09**           | Inclui positivos e negativos |
| Casos Passaram          |            **08**           | Resultados esperados         |
| Casos Falharam          |            **01**           | Corrigido após revalidação   |
| Bugs Reportados         |            **01**           | Resolvido com sucesso        |
| Taxa de Sucesso         |          **≈ 89%**          | Alto índice de conformidade  |
| Tipo de Teste           |      Manual – API REST      |                              |
| Período do Projeto      |   05/11/2025 → 12/11/2025   |                              |
| Responsável             | **Rodrigo Garcia da Silva** |                              |

🚀 Próximos Passos

 Adicionar testes automatizados da coleção Postman com Newman

 Criar relatório HTML automático (Newman Report)

 Incluir testes exploratórios adicionais

 Publicar vídeo curto de apresentação do projeto no LinkedIn 🎥

👨‍💻 Autor

Rodrigo Garcia da Silva
💼 Profissional de TI com experiência em manutenção e suporte técnico
🎯 Em transição de carreira para Qualidade de Software (QA)
📫 LinkedIn – Rodrigo Garcia

