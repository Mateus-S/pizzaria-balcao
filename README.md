# Pizzaria Balcão

Sistema web para gestão de pedidos, produção e entregas de uma pizzaria com atendimento ao balcão e integração via WhatsApp.

---

## ✅ Card 01 — Estrutura Inicial do Projeto

- Estruturado repositório monorepo com solução `PizzariaBalcao.sln`
- Adicionados os projetos:
  - `pizzaria.API` (Web API com Clean Architecture)
  - `pizzaria.Domain`, `pizzaria.Application`, `pizzaria.Infrastructure`
  - `pizzaria.WEB` (Blazor WebAssembly com Bootstrap)
- Bootstrap incluído via CDN
- Git configurado para usar VS Code como editor de commits

Branch: `feature/card-01-config-structure`

---

## ✅ Card 1.02 — Configuração do Banco de Dados (SQLite + EF Core)

- Instalado o **Entity Framework Core** com suporte ao SQLite na camada `Infrastructure`
- Criadas entidades base com chave primária (`Pedido`, `Produto`)
- Implementado `SeuProjetoDbContext` com `DbSet`s tipados
- Registrado o DbContext no `Program.cs` da API
- Adicionada fábrica de contexto (`IDesignTimeDbContextFactory`) para suporte ao CLI
- Gerada a primeira migration `InitialCreate`
- Banco `pizzaria.db` criado localmente com sucesso

Branch: `feature/card-1.02-sqlite`
