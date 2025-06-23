# IAgro

## Descrição do Projeto

Este projeto tem como objetivo a criação de uma plataforma para uma cooperativa agrícola, onde os associados podem reportar problemas em suas plantações ou criações de animais. A plataforma permitirá que os associados tirem fotos e escrevam detalhes sobre os problemas que estão encontrando. Esses pedidos serão enviados para a API do ChatGPT, que irá analisar e fornecer um diagnóstico preliminar, categorizando o tipo de problema e fornecendo sugestões de medidas preventivas e de execução.

A plataforma será composta por um aplicativo móvel para os associados e uma página web para os administradores. Os administradores terão acesso a todos os registros de consultas e poderão gerar relatórios estatísticos sobre os problemas encontrados, com a possibilidade de filtrá-los por período (mensal, semestral, anual).

## Desenvolvedores

- [Jean Charles Guichard Guichard](https://github.com/Lorrust)
- [Lucas da Rosa da Silva](https://github.com/guichardx2)
- [Matheus Augusto Daminelli](https://github.com/daminellis)

## Repositórios

- [App Mobile](https://github.com/Lorrust/iagro-app-mobile)
- [Painel Web (Admin)](https://github.com/Lorrust/iagro-web-admin)
- [Backend API](https://github.com/Lorrust/iagro-backend-api)
- [Integração IA](https://github.com/Lorrust/iagro-ai-integration)

## Funcionalidades

### Aplicativo Móvel (Associados)

- **Envio de Fotos e Descrições:** O associado pode tirar fotos de suas plantações ou criações de animais, adicionar descrições e enviar os detalhes para a API.

- **Recebimento de Diagnóstico:** A API responderá com o diagnóstico em formato JSON, incluindo:
  - Categoria do problema
  - Tipo de problema
  - Provável causa
  - Descrição de pré-diagnóstico com sugestões de ações preventivas e de execução.

- **Histórico de Consultas:** O associado poderá visualizar o histórico de suas consultas anteriores.

### Site Web (Administradores)

- **Acesso a Consultas de Todos os Associados:** O administrador poderá visualizar todas as consultas feitas pelos associados.
  
- **Geração de Relatórios Estatísticos:** O administrador poderá gerar relatórios detalhados, com filtros por:
  - **Mês:** Relatório mensal com o total de consultas e categorias mais recorrentes.
  - **Semestre:** Relatório semestral para análise de tendências.
  - **Ano:** Relatório anual para análise de longo prazo.

### Integração com API do ChatGPT

- **Diagnóstico de Problemas:** A API do ChatGPT será responsável por analisar os dados enviados (foto e descrição) e gerar um diagnóstico completo.

- **Resposta em Formato JSON:** A resposta da API será estruturada em JSON, com informações sobre a categoria do problema, tipo e causas possíveis, além de sugestões preventivas e de execução.

## Tecnologias Utilizadas

### Backend
[![My Skills](https://skillicons.dev/icons?i=py,ts,firebase,nestjs,fastapi,docker,nginx,redis)](https://skillicons.dev)

- **Python:** Para o desenvolvimento da API com FastAPI que gerenciará as solicitações dos usuários e a comunicação com a API do ChatGPT.

- **Firebase:** Para armazenamento de dados dos usuários, consultas e históricos.

- **NestJS:** Para desenvolvimento em TypesScript da API orquestradora ligada ao python e aos Frontends.

- **Docker:** Para a conteinerização do Backend junto dos serviços como Nginx e Redis.

- **Redis:** Para cacheamento de rotas e responstas da API NestJS.

- **Nginx:** Para o balancemaneto de carga (load balancer) da aplicação.

- **Docling:** Bliblioteca python para conversão de documentos e criação de chunks para o RAG (Técnica de alimentar um escopo de um modelo LLM com documentos únicos)

- **Chromadb:** Banco vetorial para guardar documentos de busca para a API do ChatGPT pela técnica de RAG.

### Frontend
[![My Skills](https://skillicons.dev/icons?i=react,vite,ts)](https://skillicons.dev)

- **React Native:** Para desenvolvimento do aplicativo móvel em TypesScript.

- **React:** Para desenvolvimento do painel de administração (site web) em TypesScript.

- **Vite:** Ferramenta para construção do site Web otimizado e organizado com react.

- **Expo:** Framework para a construção com uso do react native otimizado e organizado.

### Integração com API

- **API do ChatGPT:** Para análise dos problemas enviados pelos associados e fornecimento de respostas de diagnóstico.

### Hospedagem/Serviços

- **Firebase Hosting:** Para hospedagem do site web e do aplicativo (no caso de deploy no Firebase).
  
- **Firebase Firestore:** Para o armazenamento de dados em tempo real (consultas, usuários, histórico).
  
- **Firebase Storage:** Para o armazenamento de imagens enviadas pelos associados.

- **Docker:** Contêiner da aplicação Backend com os serviços do Redis e Nginx.

### Link da apresentação no Canva:
[IAgro](https://www.canva.com/design/DAGqve0tAGU/Kwx83QoHeDL3TQAOUxdsKg/view?utm_content=DAGqve0tAGU&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h3e3a0f6299)
