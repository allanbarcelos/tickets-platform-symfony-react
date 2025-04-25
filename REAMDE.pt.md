# Tickets Platform - Symphony PHP

Este repositório contém a versão atualizada de uma aplicação de tickets desenvolvida originalmente em 2016, usando **Symfony** no backend e **frontend sem frameworks**, utilizando apenas **jQuery** como biblioteca JavaScript. O código legado foi aprimorado e reestruturado para proporcionar uma plataforma mais robusta e escalável.

## Estrutura do Repositório

```bash
/tickets-platform
├── /api           ← Symfony (PHP Backend)
│   └── ...
├── /app           ← Next.js (React Frontend)
│   └── ...
├── docker-compose.yml
├── .env
└── README.md
```

## Sobre a Atualização

A versão atualizada da aplicação passou por várias melhorias e reestruturações, incluindo:

- **Backend:** O Symfony foi mantido no backend, mas com melhorias de performance e estruturação do código.
- **Frontend:** O frontend foi completamente refeito utilizando **Next.js** (React), oferecendo uma experiência de usuário mais moderna e responsiva.
- **Docker:** A aplicação agora utiliza **Docker** para dividir os serviços em containers, facilitando o gerenciamento e a escalabilidade.

## Aplicação Legada

O código original, desenvolvido em 2016, está em produção até hoje. No entanto, devido a questões de segurança e dados sensíveis, o repositório da versão original está privado. Caso tenha curiosidade em conhecer o código legado, por favor, entre em contato para que eu possa te apresentar com algumas limitações de acesso.

## Como Rodar o Projeto

### Pré-requisitos

Certifique-se de que você tenha as seguintes ferramentas instaladas:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Iniciar os Containers

Para rodar a aplicação localmente utilizando Docker, basta seguir os seguintes passos:

1. Clone o repositório:
   ```bash
   git clone <URL do repositório>
   cd tickets-platform
   ```

2. Suba os containers:
   ```bash
   docker-compose up --build
   ```

3. Acesse o backend e o frontend no seu navegador:

   - **Frontend (Next.js):** `http://localhost:3000`
   - **Backend (Symfony):** `http://localhost:8000`

## Contribuindo

Sinta-se à vontade para contribuir com melhorias ou correções! Caso você tenha sugestões ou problemas, abra uma **issue** ou envie um **pull request**.

---

**Nota:** Este projeto é uma atualização de um sistema legado e possui algumas limitações, principalmente em relação ao código original. Qualquer dúvida ou necessidade de esclarecimentos adicionais, estou à disposição!