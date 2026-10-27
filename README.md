# SalesWebMvc

**Português** | [English](README.en.md)

Projeto inicial em **ASP.NET Core MVC (.NET 8)**, criado como estudo. O conteúdo atual é o modelo padrão do Visual Studio: página inicial ("Welcome"), página de privacidade e página de erro.

> **Status: estudo inicial.** Ainda não há código de vendas, banco de dados ou Entity Framework Core.

## Funcionalidades

- `GET /`: página inicial do modelo.
- `GET /Home/Privacy`: página de privacidade do modelo.
- `/Home/Error`: página de erro.

## Tecnologias

- **C#** / **.NET 8**
- **ASP.NET Core MVC** com Razor Views
- **Bootstrap 5** e **jQuery** (bibliotecas do modelo em `wwwroot/lib`)

O GitHub classifica o repositório como HTML porque as bibliotecas de front-end incluídas pelo modelo ocupam a maior parte dos arquivos.

## Estrutura

```
SalesWebMvc/
├── SalesWebMvc.sln
└── SalesWebMvc/
    ├── Controllers/HomeController.cs
    ├── Models/ErrorViewModel.cs
    ├── Views/            # Home e Shared (Razor)
    ├── wwwroot/          # css, js e lib (Bootstrap, jQuery, jQuery Validation)
    ├── Program.cs
    └── appsettings.json
```

## Como executar

Requisito: [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0).

Na raiz do repositório:

```bash
dotnet run --project SalesWebMvc/SalesWebMvc.csproj
```

Acesse **http://localhost:5224**. Para usar HTTPS (**https://localhost:7012**), execute com o perfil `https`:

```bash
dotnet run --project SalesWebMvc/SalesWebMvc.csproj --launch-profile https
```

Os perfis estão em `SalesWebMvc/Properties/launchSettings.json`.
