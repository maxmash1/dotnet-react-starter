# dotnet-react-starter

A minimal full-stack application template for demonstrating GitHub Copilot capabilities.

> **📋 Note:** This is a **demo/starter template** designed to showcase how organizations can configure and leverage GitHub Copilot (instructions, prompts, skills, and agents) within a real-world project structure. The development standards, patterns, and configurations included here are **illustrative examples** — they do not represent any proprietary or organization-specific standards. Feel free to use this as a template and adapt the standards to your own team's needs.

## Overview

- **Backend:** .NET 8 Web API with Entity Framework Core
- **Frontend:** React 18 + TypeScript + Vite + Tailwind CSS
- **Testing:** xUnit + Moq (backend)

## Quick Start

### Backend

```bash
cd backend
dotnet restore
dotnet build
dotnet run --project src/Api
```

The API will be available at `http://localhost:5000` with Swagger UI at `/swagger`.

### Frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`.

## Project Structure

```
├── backend/
│   ├── src/Api/           # Web API project
│   └── tests/Api.Tests/   # Unit tests
├── frontend/              # React + TypeScript application
├── legacy/                # Classic ASP files (for migration demo)
└── .github/
    ├── copilot-instructions.md  # Organization standards
    ├── agents/                   # Copilot agents
    ├── prompts/                  # Reusable prompts
    └── skills/                   # Copilot skills
```

## API Endpoints

| Method | Endpoint     | Description              |
|--------|--------------|--------------------------|
| GET    | /v1/health   | Health check endpoint    |

## Development Standards

See `.github/copilot-instructions.md` for complete development standards including:
- API design patterns (envelope responses, naming conventions)
- C# coding standards (async/await, DTOs, repositories, services)
- Testing standards (naming, AAA pattern, organization)
- Frontend standards (TypeScript, Tailwind)

## License

MIT
