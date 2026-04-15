### Estação Meteorológica IoT — Inception
---
**Sobre o Projeto**

Este projeto foi desenvolvido como parte de uma iniciativa da Tecsus, empresa especializada na coleta e processamento de dados por meio de redes de sensores sem fio (IoT), com atuação consolidada no monitoramento de utilidades como água, energia e gás.
Com o objetivo de expandir seu portfólio para o monitoramento ambiental, o projeto propõe o desenvolvimento de estações meteorológicas de baixo custo, capazes de coletar, transmitir e processar dados climáticos em tempo real. Os parâmetros monitorados incluem:

- Direção e velocidade do vento
- Índice pluviométrico
- Umidade relativa do ar
- Temperatura
- Pressão atmosférica

Os dados são transmitidos pelas estações por meio de tecnologias de comunicação como Sigfox, LoRa e NB-IoT, e encaminhados a um servidor central responsável pela recepção, armazenamento e processamento das informações. Os resultados são disponibilizados em um portal web com dashboards interativos e relatórios analíticos.

*Contexto de Aplicação*

A solução foi projetada para atender ao segmento de iniciativa privada, mais especificamente uma multinacional de agricultura de precisão que comercializa previsões climáticas ultra-localizadas para grandes produtores de soja. Nesse cenário, o sistema é dimensionado para:

Suportar um crescimento planejado e escalável da infraestrutura de sensores;
Garantir alta disponibilidade e confiabilidade na coleta e transmissão dos dados;
Permitir manutenções frequentes e evoluções contínuas da plataforma;
Atender às demandas de precisão e granularidade exigidas pelo agronegócio de grande porte.

---

###  Requisitos Funcionais (RF)
* **01 - Modelo de Dados Dinâmico:** Capacidade de receber e registrar estações meteorológicas equipadas com diversos tipos de sensores.
* **02 - CRUD Completo:** Funcionalidades de criação, leitura, atualização e exclusão para Estações, Parâmetros, Alertas e Usuários.
* **03 - Recepção de Dados:** Processamento e armazenamento dos dados enviados pelas estações meteorológicas.
* **04 - Dashboards:** Visualização interativa dos parâmetros meteorológicos.
* **05 - Geração de Alertas:** Criação automática de notificações baseadas em condições meteorológicas específicas.
* **06 - Desenvolvimento de Datalogger:** Implementação de um datalogger para registrar dados em uma estação meteorológica.
* **07 - Montagem da Estação:** Construção física de uma estação meteorológica com os componentes necessários.
* **08 - Tutorial Educativo:** Desenvolvimento de um guia explicativo sobre o significado de cada parâmetro meteorológico medido.
* **09 - Autenticação:** O sistema deve fornecer uma interface que permita Operador ou Usuário realizar o login mediante credenciais válidas.

###  Requisitos Não Funcionais (RNF)
* **Experiência do Usuário (UX):** O design dos dashboards deve priorizar a usabilidade e a estética para o melhor engajamento dos usuários.
* **Documentação de APIs:** Elaboração detalhada da documentação para todas as rotas da API, incluindo exemplos práticos de uso.
* **Integração Contínua (CI):** Implementação de um pipeline de CI para automação de testes e validações de código.
* **Deploy Automatizado:** Configuração de deploy de acordo com as necessidades de cada produto/cliente, garantindo o ROI e respeitando a arquitetura definida.

---

##  Backlog do Produto & Planejamento de Sprints

Abaixo estão as User Stories priorizadas e estimadas pelo time, divididas por Sprints para facilitar o acompanhamento das entregas.

| RF | Rank | Prioridade | User Story | Estimativa | Sprint |
| :---: | :---: | :---: | --- | :---: | :---: |
| **09** | 1 |  Alta | Como operador, quero efetuar login no sistema de forma segura para acessar as funcionalidades administrativas restritas. | 8 | **1** |
| **02** | 2 |  Alta | Como administrador, quero cadastrar novos administradores e operadores para descentralizar e auxiliar na gestão do sistema. | 5 | **1** |
| **01, 07** | 3 |  Alta | Como administrador, quero cadastrar ou remover estações meteorológicas para viabilizar a identificação e o registro dos dispositivos que enviarão dados ambientais. | 8 | **1** |
| **03** | 4 |  Alta | Como usuário, quero visualizar as estações meteorológicas cadastradas para acompanhar o status e a localização dos dispositivos de coleta ativos. | 3 | **1** |
| **02** | 5 |  Alta | Como operador, quero editar informações de estações meteorológicas para manter os dados cadastrais sempre atualizados e precisos. | 3 | **1** |
| **05** | 6 |  Média | Como operador, quero cadastrar regras de alertas meteorológicos para que o sistema monitore continuamente condições climáticas críticas estabelecidas. | 5 | **1** |
| **01** | 7 |  Média | Como usuário, quero receber dados enviados automaticamente pelas estações para armazenar as medições ambientais de forma persistente e escalável no banco de dados. | 13 | **2** |
| **04** | 8 |  Média | Como operador e usuário, quero visualizar dashboards interativos com gráficos para analisar e interpretar de forma clara as variações climáticas registradas pelas estações. | 8 | **2** |
| **04** | 9 |  Média | Como usuário, quero filtrar os dados meteorológicos por estação e período de tempo para focar minha análise em medições, eventos ou regiões específicas. | 5 | **2** |
| **05** | 10 |  Média | Como usuário, quero receber alertas visuais no sistema para ser notificado imediatamente quando ocorrerem condições meteorológicas extremas ou anormais. | 5 | **3** |
| **06** | 11 |  Média | Como operador, quero gerar relatórios meteorológicos consolidados para obter insights profundos e embasar tomadas de decisão sobre os dados coletados. | 13 | **3** |
| **08** | 12 |  Baixa | Como usuário público ou estudante, quero acessar guias e tutoriais educativos para compreender com facilidade o significado e o contexto de cada parâmetro meteorológico exibido no sistema. | 3 | **3** |

# Entregas de Sprints

| Sprint | Previsão de entrega | Status | Histórico |
|:--:|:----------:|:-------------------|:-------------------------------------------------:|
| 01 | 16/03/2026 a 05/04/2026 | Finalizado | [Ver relatório](https://drive.google.com/file/d/1_HgLopyOHJdeE_aSdh8RHsnkOMto9e46/view?usp=sharing) |
| 02 | 13/04/2026 a 03/05/2026 | Em breve | [Ver relatório]() |
| 03 | 11/05/2026 a 31/05/2026 | Em breve |  [Ver relatório]()|

---

##  Definition of Ready (DoR)

Para que uma tarefa seja considerada pronta para entrar em uma Sprint, ela deve obrigatoriamente cumprir os seguintes critérios:

- [x] **User Story Clara:** A história de usuário descreve o "quem", "o quê" e o "porquê" (valor de negócio).
- [x] **Critérios de Aceite:** Estão listados os pontos exatos que definem se a funcionalidade opera como o esperado.
- [x] **ID da Task Gerado:** A tarefa possui um ID único para seguir o padrão de nomenclatura de branch e commit (`#ID-task`).
- [x] **Dependências Mapeadas:** O time identificou previamente se a task depende da conclusão de outra ou da adição de alguma biblioteca externa.
- [x] **Estimativa Definida:** A dupla responsável já discutiu e definiu o esforço/tempo necessário para o desenvolvimento da task.

## Links Úteis

- [Modelo do Banco de Dados](https://drive.google.com/file/d/18yUxya8_wpQCmzCOSq8FHJrW0V8Bu8-m/view?usp=sharing)
- [Elicitação de Requisitos](https://drive.google.com/file/d/1ShDRmZJhckWnaFhiGJOOwl0BRvxQV6le/view?usp=sharing)
- [Fluxo de Entregas](https://drive.google.com/file/d/1Tsl4ooda1WgTUd1ZgnHvqcp75jaXHcYA/view?usp=sharing)
- [Mockup do Projeto](https://drive.google.com/file/d/1p6P29K0tUN_DnKkGYm8xj4WN0oVwOUfG/view?usp=sharing)
- [Onboarding de Novos Membros](https://docs.google.com/document/d/1b4mSGMyWPyq6AOTlBTp0pLTUoy2Yk7Q7oU-cBg2QVH0/edit?usp=sharing)
- [Guia de Desenvolvimento](https://docs.google.com/document/d/1b4mSGMyWPyq6AOTlBTp0pLTUoy2Yk7Q7oU-cBg2QVH0/edit?usp=sharing)
- [DevOps Docs](https://drive.google.com/drive/folders/1NVWPxc3sS2haeArmtEPTIM5_LAHxXVeA?usp=sharing)

## Equipe


|    Função     | Nome                                  |                                                                                                                                                      LinkedIn & GitHub                                                                                                                                                      |
| :-----------: | :------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|  Scrum Master  | Pedro Martins               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/pedrohmartinsss/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/pedro-h-martins)   |
| Product Owner   | Matheus Ramos      |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/matheusfcrms/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/KwMajor)        |
| Team Member   | Gabriel Lima |      [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/gabriel-fernando-bb430b330/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Gabriel-Fernando-Lima)     |
|  Team Member  | Lavinia Piratello               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lavinia-piratello-6a82101b1/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/laviniappiratello)   |
|  Team Member  | Lucas Araujo                 |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-araujo-448115329/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/LucasAraujo1016)        |
|  Team Member  | Lucas Guerra     |           [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-guerra000/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/lucasguerra12)   |
|  Team Member  | Lucas Martins               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lucasmscarmo/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/LucasMSCarmo)   |
|  Team Member  | Matheus Karnas              |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/matheuskarnas/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/matheuskarnas)   |