FlightBoard
A full-stack real-time Flight Board management system.  
Built with ASP.NET Core WebAPI, React, Redux Toolkit, SignalR, EF Core, and SQLite.

---

## Project Structure

FlightBoard/
├── client/ # React + TypeScript frontend
└── server/ # ASP.NET Core WebAPI backend
---
## Features

### Backend (ASP.NET Core)
- RESTful API for managing flights (GET/POST/DELETE/SEARCH)
- Real-time updates via **SignalR**
- EF Core with **SQLite** database
- Clean Architecture & TDD-ready
- Validation and business logic enforced server-side

### Frontend (React)
- TypeScript-based SPA
- State management with **Redux Toolkit**
- **TanStack Query** for async API handling (React Query)
- SignalR real-time flight updates
- Filtering, undo-delete popup, loading/error states
- Routing with **React Router**
---
## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- [Node.js (v18+)](https://nodejs.org/)
- SQLite (optional, DB auto-creates)

---

### Backend Setup

```bash
cd server
dotnet restore
dotnet ef database update  # Optional: to apply migrations
dotnet run
Runs on: https://localhost:7198

Frontend Setup
bash
Copy
Edit
cd client
npm install
npm start
Runs on: http://localhost:3000

 Real-Time
SignalR is used to broadcast real-time flight board updates.

Connected clients receive push updates immediately on changes (add/delete/search).

 Testing
 xUnit tests for backend and component tests for frontend.

 Technologies
Frontend: React, TypeScript, Redux Toolkit, React Query, Bootstrap

Backend: ASP.NET Core, Entity Framework Core, SignalR

Database: SQLite

Architecture: Clean Architecture

Tooling: Visual Studio, VS Code, GitHub

 Deployment
To deploy, build both apps and host them with IIS.


 Author
Olga Miller
GitHub: @OlgaMiller1808
