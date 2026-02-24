# software-design-architecture

Este repo tem como objetivo ser um dicionário/guia de arquitetura

| Nível | Categoria                    | Granularidade            | O que define                                      | Conceitos envolvidos                           | Exemplos clássicos                      | Onde atua                      |
| ----- | ---------------------------- | ------------------------ | ------------------------------------------------- | ---------------------------------------------- | --------------------------------------- | ------------------------------ |
| 1️⃣   | **Architectural Styles**     | 🌍 Muito Macro           | Estrutura geral do sistema                        | Distribuição, comunicação, topologia           | Microservices, Layered, Event-Driven    | Sistema como um todo           |
| 2️⃣   | **Architectural Patterns**   | 🏗 Macro                 | Organização estrutural interna                    | Fluxo de dependência, separação de camadas     | MVC, CQRS, Hexagonal, Onion             | Arquitetura da aplicação       |
| 3️⃣   | **Enterprise Patterns**      | 🏢 Macro especializado   | Soluções arquiteturais para sistemas corporativos | Persistência, transação, integração            | Repository, Unit of Work, Service Layer | Dentro da arquitetura          |
| 4️⃣   | **Architectural Principles** | 📐 Conceitual estrutural | Regras que guiam arquitetura                      | Loose Coupling, High Cohesion, Dependency Rule | Separation of Concerns                  | Influenciam estilos e patterns |
| 5️⃣   | **Design Patterns**          | 🧱 Médio                 | Soluções para problemas recorrentes de design     | Criação, estrutura e comportamento             | Strategy, Factory, Adapter              | Nível de classes/módulos       |
| 6️⃣   | **Design Principles**        | 🧠 Micro conceitual      | Diretrizes de qualidade de código                 | SOLID, DRY, KISS                               | SRP, OCP                                | Dentro de classes e módulos    |


# Ordem

Macro estrutura do sistema
    ↓
Organização arquitetural interna
    ↓
Soluções arquiteturais corporativas
    ↓
Regras que guiam decisões estruturais
    ↓
Soluções reutilizáveis de código
    ↓
Princípios fundamentais de design

# Hierarquia Visual Completa

SOFTWARE SYSTEM
│
├── 1️⃣ Architectural Styles (macro estrutura)
│      ├── Microservices
│      ├── Layered
│      ├── Event-Driven
│      └── Client-Server
│
├── 2️⃣ Architectural Patterns (organização interna)
│      ├── MVC
│      ├── CQRS
│      ├── Hexagonal
│      ├── Onion
│      └── Clean Architecture
│
├── 3️⃣ Enterprise Patterns (dentro da arquitetura)
│      ├── Repository
│      ├── Unit of Work
│      ├── Service Layer
│      ├── Data Mapper
│      └── Identity Map
│
├── 4️⃣ Architectural Principles (regras estruturais)
│      ├── Separation of Concerns
│      ├── Loose Coupling
│      ├── High Cohesion
│      └── Dependency Inversion (arquitetural)
│
├── 5️⃣ Design Patterns (nível de código)
│      ├── Creational
│      │     ├── Factory
│      │     └── Builder
│      ├── Structural
│      │     ├── Adapter
│      │     └── Decorator
│      └── Behavioral
│            ├── Strategy
│            └── Observer
│
└── 6️⃣ Design Principles (fundamentos)
       ├── SOLID
       ├── DRY
       ├── KISS
       └── YAGNI
