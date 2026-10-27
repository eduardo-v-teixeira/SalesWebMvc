# SalesWebMvc

[Português](README.md) | **English**

A starter **ASP.NET Core MVC (.NET 8)** project, created as a study. Its current content is the default Visual Studio template: a home page ("Welcome"), a privacy page and an error page.

> **Status: early study.** There is no sales code, database or Entity Framework Core yet.

## Features

- `GET /`: template home page.
- `GET /Home/Privacy`: template privacy page.
- `/Home/Error`: error page.

## Tech stack

- **C#** / **.NET 8**
- **ASP.NET Core MVC** with Razor views
- **Bootstrap 5** and **jQuery** (template libraries in `wwwroot/lib`)

GitHub lists the repository as HTML because the front-end libraries bundled by the template make up most of the files.

## Structure

```
SalesWebMvc/
├── SalesWebMvc.sln
└── SalesWebMvc/
    ├── Controllers/HomeController.cs
    ├── Models/ErrorViewModel.cs
    ├── Views/            # Home and Shared (Razor)
    ├── wwwroot/          # css, js and lib (Bootstrap, jQuery, jQuery Validation)
    ├── Program.cs
    └── appsettings.json
```

## How to run

Requirement: [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0).

From the repository root:

```bash
dotnet run --project SalesWebMvc/SalesWebMvc.csproj
```

Open **http://localhost:5224**. To use HTTPS (**https://localhost:7012**), run with the `https` profile:

```bash
dotnet run --project SalesWebMvc/SalesWebMvc.csproj --launch-profile https
```

The profiles are defined in `SalesWebMvc/Properties/launchSettings.json`.
