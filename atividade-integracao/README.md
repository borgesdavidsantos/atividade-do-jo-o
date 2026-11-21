# Integração entre Frontend e Backend — CRUD de Usuários

Frontend: React (Vite) + Material UI + Axios
Backend: Spring Boot (Web + Data JPA) + PostgreSQL

## 1. Banco de dados
```sql
CREATE DATABASE aulaintegracao;
```
Usuário/senha configurados em `backend/src/main/resources/application.properties`
(padrão: `postgres` / `postgres`). Ajuste para o seu PostgreSQL local.

## 2. Backend (porta 8080)
Requer Java instalado (ajuste `java.version` no `backend/pom.xml` se necessário).
```bash
cd backend
mvn spring-boot:run
```
(ou abra a pasta `backend` no IntelliJ/VS Code e execute `BackendApplication`).

## 3. Frontend (porta 5173)
```bash
cd frontend
npm install
npm run dev
```
Abra http://localhost:5173

## Endpoints
- GET    /api/users
- GET    /api/users/{id}
- POST   /api/users
- PUT    /api/users/{id}
- DELETE /api/users/{id}
