# Olá! Sou o Pedro Leanza 👋

<p align="center">
  <img src="./github_profile_banner.png" alt="Pedro Leanza - Pragmatic Backend Systems Engineer" width="100%" style="border-radius: 8px;" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=24&duration=3000&pause=1000&color=00F0FF&center=true&vCenter=true&width=600&lines=%3E+Computer+Science+Student;%3E+Focused+on+High-Performance+Backend;%3E+Building+Distributed+Systems;%3E+Mastering+Go%2C+Rust%2C+C%2B%2B+%26+Java;%3E+Pragmatic+AI-Augmented+Engineer" alt="Typing SVG" />
</p>

---

### ⚡ Sobre Mim

Sou estudante de **Ciência da Computação** com foco absoluto em construir uma fundação técnica robusta. Minha abordagem de aprendizado é pragmática: complemento minha base acadêmica aprofundando-me na prática para entender as engrenagens internas dos sistemas — concorrência, gerenciamento de memória, I/O e segurança de dados.

Minha rotina de engenharia divide-se em:
*   **🔬 Laboratórios de Sistemas & Fundamentos:** Onde desço ao nível do sistema operacional para entender e projetar sistemas distribuídos tolerantes a falhas.
*   **🚀 Desenvolvimento de Produtos & SaaS:** Onde implemento arquiteturas escaláveis, UX premium e integrações de alto valor comercial voltados ao mercado internacional.

---

### 🛠 Meu Arsenal Tecnológico

<table align="center" style="border: none; background: transparent;">
  <tr>
    <td align="left" valign="top" width="50%">
      <strong>Linguagens e Core</strong><br/>
      <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
      <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" />
      <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" /><br/>
      <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
    </td>
    <td align="left" valign="top" width="50%">
      <strong>Infraestrutura & Bancos</strong><br/>
      <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" /><br/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
    </td>
  </tr>
</table>

---

### 🗺️ Topologia de Sistemas Distribuídos

Em vez de acumular projetos soltos, eu desenho as minhas aplicações para operarem como peças conectadas de uma infraestrutura robusta de alta escala. O ecossistema abaixo ilustra como meus projetos se integram no fluxo de dados de um ambiente distribuído real:

```mermaid
flowchart TD
    classDef client fill:#0d1117,stroke:#58a6ff,stroke-width:2px,color:#fff;
    classDef proxy fill:#0d1117,stroke:#00F0FF,stroke-width:2px,color:#fff;
    classDef queue fill:#0d1117,stroke:#00ADD8,stroke-width:2px,color:#fff;
    classDef db fill:#0d1117,stroke:#ff7b72,stroke-width:2px,color:#fff;
    classDef svc fill:#0d1117,stroke:#d757b3,stroke-width:2px,color:#fff;

    Client["🌐 Client Layer <br/>(SkateTech / Storefront)"]:::client
    Client -->|HTTPS / 15k+ req/sec| Balancer["⚡ Aura Balancer <br/>(C++17 L7 Load Balancer)"]:::proxy
    
    Balancer -->|Zero-Copy TCP Sockets| Broker["📬 GigaMQ <br/>(Go Message Queue)"]:::queue
    
    Broker -->|Linearizable Log Consensus| Consensus["💾 RaftKV <br/>(Rust Key-Value Database)"]:::db
    Broker -->|Async Event Streaming| Saga["💼 SagaCommerce <br/>(Java/Spring Boot Microservices)"]:::svc
    
    Saga -->|Row-Level Isolated Sync| PG["🛢 PostgreSQL Cluster"]:::db

    style Client box-shadow:0 0 10px rgba(88,166,255,0.2)
    style Balancer box-shadow:0 0 10px rgba(0,240,255,0.2)
    style Broker box-shadow:0 0 10px rgba(0,173,216,0.2)
    style Consensus box-shadow:0 0 10px rgba(255,123,114,0.2)
    style Saga box-shadow:0 0 10px rgba(215,87,179,0.2)
```

---

### 💻 Simulador de Sistemas & Compilação

Para demonstrar a corretude e a performance real do meu código de baixo nível, o terminal interativo abaixo executa testes automatizados e benchmarks de desempenho dos meus serviços de backend:

<p align="center">
  <img src="./github_profile_terminal.svg" alt="Simulação de Compilação de Sistemas Distribuídos" width="100%" />
</p>

---

### 🔬 Laboratórios de Backend (Fundamentos e Arquitetura)

Projetos desenvolvidos para estudar como arquiteturas complexas se comportam sob estresse, priorizando eficiência de CPU/memória e corretude técnica.

*   **[GigaMQ (Go)](https://github.com/Leanza-dev/GigaMQ)**: Message Broker TCP em memória projetado para altíssimo throughput. Utiliza buffers otimizados e paralelismo seguro via goroutines/channels para evitar alocações desnecessárias no Garbage Collector.
*   **[RaftKV (Rust)](https://github.com/Leanza-dev/RaftKV)**: Banco de dados Key-Value distribuído e tolerante a falhas, implementando o protocolo de consenso Raft. Focado em consistência forte ($Linearizability$) e tratamento rigoroso de concorrência com Rust `tokio`.
*   **[SagaCommerce (Java)](https://github.com/Leanza-dev/SagaCommerce)**: Sistema de e-commerce baseado em microsserviços aplicando o padrão **Saga Coreografada** com Spring Boot e Apache Kafka para garantir consistência eventual resiliente.
*   **[Aura Balancer (C++)](https://github.com/Leanza-dev/AuraBalancer)**: Balanceador de carga L7 minimalista e de alta performance implementado em C++17 puro com POSIX sockets, demonstrando controle fino sobre ponteiros e sincronização de concorrência via `std::atomic`.

---

### 🚀 Produtos & SaaS (Entrega de Valor e UX)

Aplicações modernas focadas em resolver problemas reais de mercado, unindo engenharia scalável a uma experiência de usuário polida.

*   **[Showroom Velocidade (Next.js)](https://github.com/Leanza-dev/ShowroomVelocidade)**: Plataforma *Website-as-a-Service* (WaaS) multi-tenant altamente otimizada para concessionárias. Foco em performance extrema (100/100 Lighthouse no mobile), SSG dinâmico e integração com funil de conversão no WhatsApp. *(Código Proprietário - Estudo de Caso Arquitetural no Repositório)*
*   **[SkateTech (React Native)](https://github.com/Leanza-dev/SkateTech)**: Aplicativo mobile para skatistas mapearem picos e compartilharem linhas. Foco em UX nativa fluida, geolocalização e transições fluidas de interface.
*   **[GigaCloud Infra (TypeScript)](https://github.com/Leanza-dev/GigaCloud)**: Estrutura serverless de referência com suporte a alta disponibilidade na AWS, focada em estratégias de aquecimento para prevenção de Cold Starts e observabilidade avançada.

---

### 📫 Conecte-se Comigo

*   **LinkedIn:** [linkedin.com/in/pedro-leanza](https://www.linkedin.com/in/pedro-leanza/)
*   **Email:** [pedro.leanza.dev@gmail.com](mailto:pedro.leanza.dev@gmail.com)
*   **Portfólio:** [leanza-dev-site.vercel.app](https://leanza-dev-site.vercel.app/) *(Em breve atualizado com as novas animações e i18n)*

---
*“A complexidade é fácil. A simplicidade é que dá trabalho.”*
