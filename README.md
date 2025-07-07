# DCS – Debit and Credit System

**DCS** (Debit and Credit System) is a secure and scalable financial transaction platform built using **Angular** (`dcs.client`) and **.NET Core 8** (`DCS.Server`). The system ensures reliable debit and credit operations with proper authentication, encryption, and data integrity validation.

## 🔐 Key Features

- JWT-based Authentication with Refresh Token support
- Debit & Credit transaction module with validation and logging
- AES-256 data encryption using 32-byte hex key
- Enforced data integrity with transaction hash checking
- MSSQL normalized database schema
- Angular frontend with secured local storage
- Ready for enterprise-level scaling

## 🧱 Tech Stack

| Layer    | Technology                    |
| -------- | ----------------------------- |
| Frontend | Angular (`dcs.client`)        |
| Backend  | ASP.NET Core 8 (`DCS.Server`) |
| Database | Microsoft SQL Server          |
| Security | JWT, AES-256 Encryption       |

## 🔝 AES Encryption Key (Dev Only)

```
Generate your own key: https://emn178.github.io/online-tools/sha256.html
```

> ⚠️ **Note:** This key is for local development. Store securely in production using environment variables or a secret manager.

## 🚀 Getting Started

### 🔹 Backend – .NET Core 8 (`DCS.Server`)

```bash
cd DCS.Server
dotnet restore
dotnet ef database update
dotnet run
```

> Make sure your `appsettings.json` contains the correct connection string and JWT configuration.

### 🔹 Frontend – Angular (`dcs.client`)

```bash
cd dcs.client
npm install
ng serve
```

> You may configure base API URL in `environment.ts`.

## 📁 Project Structure

```
DCS/
├── dcs.client/       → Angular frontend project
│   └── README.md      → Frontend-specific notes (optional)
├── DCS.Server/       → .NET Core backend project
│   └── appsettings.json
├── README.md         → ✅ Main documentation file (this one)
├── DCS.sln           → Solution file
```

## 📌 Developer Info

**👨‍💻 Developer**: Norell Mantilla
📧 Email: [NRLDCM@gmail.com](mailto:NRLDCM@gmail.com)
📍 Location: Philippines
🗓️ Year: 2025
