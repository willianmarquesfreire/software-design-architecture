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

<pre>
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
</pre>
    
SOFTWARE SYSTEM

<pre>
├── 1️⃣ ARCHITECTURAL STYLES (estrutura macro do sistema)
│   │
│   ├── Monolithic
│   │     ├── Modular Monolith
│   │     └── Layered Monolith
│   │
│   ├── Client–Server
│   │     ├── 2-Tier
│   │     ├── 3-Tier
│   │     └── N-Tier
│   │
│   ├── Microservices
│   │     ├── Service per Business Capability
│   │     ├── Database per Service
│   │     ├── API Gateway
│   │     ├── Service Discovery
│   │     └── Circuit Breaker
│   │
│   ├── Service-Oriented Architecture (SOA)
│   │     ├── ESB
│   │     ├── Service Contracts
│   │     ├── Orchestration
│   │     └── Choreography
│   │
│   ├── Event-Driven Architecture (EDA)
│   │     ├── Event Producers
│   │     ├── Event Consumers
│   │     ├── Message Broker
│   │     ├── Pub/Sub
│   │     └── Event Streaming
│   │
│   ├── Data-Centric
│   │     ├── Shared Database
│   │     └── Data Pipeline
│   │
│   ├── Component-Based
│   │     ├── Reusable Components
│   │     └── Plug-in Architecture
│   │
│   └── Domain-Oriented
│         ├── Bounded Context
│         └── Domain Segmentation
│
│
├── 2️⃣ ARCHITECTURAL PATTERNS (organização estrutural da aplicação)
│   │
│   ├── Layered Architecture
│   │     ├── Presentation Layer
│   │     ├── Application Layer
│   │     ├── Domain Layer
│   │     └── Infrastructure Layer
│   │
│   ├── MVC
│   │     ├── Model
│   │     ├── View
│   │     └── Controller
│   │
│   ├── Clean Architecture
│   │     ├── Entities
│   │     ├── Use Cases
│   │     ├── Interface Adapters
│   │     └── Frameworks & Drivers
│   │
│   ├── Hexagonal (Ports & Adapters)
│   │     ├── Ports (Inbound/Outbound)
│   │     └── Adapters
│   │
│   ├── Onion Architecture
│   │     ├── Domain Core
│   │     ├── Application Services
│   │     └── Infrastructure
│   │
│   ├── CQRS
│   │     ├── Commands
│   │     ├── Queries
│   │     ├── Write Model
│   │     └── Read Model
│   │
│   ├── Event Sourcing
│   │     ├── Event Store
│   │     ├── Aggregate Replay
│   │     └── Snapshots
│   │
│   ├── Pipe-and-Filter
│   │     ├── Filters
│   │     └── Pipes
│   │
│   ├── Microkernel
│   │     ├── Core System
│   │     └── Plug-ins
│   │
│   └── Serverless
│         ├── Functions
│         └── Managed Services
│
│
├── 3️⃣ ENTERPRISE PATTERNS (padrões corporativos estruturais)
│   │
│   ├── Domain-Driven Design (DDD)
│   │     ├── Ubiquitous Language
│   │     ├── Entity
│   │     ├── Value Object
│   │     ├── Aggregate
│   │     ├── Aggregate Root
│   │     ├── Repository
│   │     ├── Factory
│   │     ├── Domain Service
│   │     ├── Application Service
│   │     ├── Bounded Context
│   │     └── Context Mapping
│   │
│   ├── Service Layer
│   ├── Repository Pattern
│   ├── Unit of Work
│   ├── Identity Map
│   ├── Data Mapper
│   ├── Active Record
│   ├── Transaction Script
│   ├── Domain Model
│   ├── Table Data Gateway
│   └── Gateway Pattern
│
│
├── 4️⃣ ARCHITECTURAL PRINCIPLES (princípios estruturais)
│   │
│   ├── Separation of Concerns
│   ├── Single Responsibility (arquitetural)
│   ├── High Cohesion
│   ├── Low Coupling
│   ├── Dependency Rule
│   ├── Dependency Inversion
│   ├── Explicit Boundaries
│   ├── Interface Segregation (arquitetural)
│   ├── Modularity
│   ├── Encapsulation
│   └── Scalability by Design
│
│
├── 5️⃣ DESIGN PATTERNS (nível de código e componentes)
│   │
│   ├── Creational
│   │     ├── Factory Method
│   │     ├── Abstract Factory
│   │     ├── Builder
│   │     ├── Prototype
│   │     └── Singleton
│   │
│   ├── Structural
│   │     ├── Adapter
│   │     ├── Decorator
│   │     ├── Facade
│   │     ├── Composite
│   │     ├── Bridge
│   │     └── Proxy
│   │
│   ├── Behavioral
│   │     ├── Strategy
│   │     ├── Observer
│   │     ├── Command
│   │     ├── Mediator
│   │     ├── State
│   │     ├── Template Method
│   │     ├── Chain of Responsibility
│   │     ├── Iterator
│   │     └── Visitor
│   │
│   └── Concurrency Patterns
│         ├── Thread Pool
│         ├── Producer-Consumer
│         └── Future/Promise
│
│
└── 6️⃣ DESIGN PRINCIPLES (fundamentos do código)
    │
    ├── SOLID
    │     ├── SRP
    │     ├── OCP
    │     ├── LSP
    │     ├── ISP
    │     └── DIP
    │
    ├── DRY
    ├── KISS
    ├── YAGNI
    ├── Composition over Inheritance
    ├── Law of Demeter
    ├── Program to an Interface
    ├── Prefer Immutability
    └── Tell, Don’t Ask
</pre>
