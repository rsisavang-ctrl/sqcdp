# SQCDP API

Une API REST simple basée sur Express.js

## Installation

```bash
npm install
```

## Démarrage

### Mode développement
```bash
npm run dev
```

### Mode production
```bash
npm start
```

L'API sera disponible sur `http://localhost:3000`

## Routes disponibles

### Health Check
- `GET /api/health` - Vérifie le statut du serveur

### Users
- `GET /api/users` - Récupère tous les utilisateurs
- `GET /api/users/:id` - Récupère un utilisateur par ID
- `POST /api/users` - Crée un nouvel utilisateur

## Configuration

Copiez `.env.example` vers `.env` et ajustez les variables d'environnement :

```bash
cp .env.example .env
```

## Structure du projet

```
src/
  ├── index.js       - Point d'entrée principal
  └── routes/        - Endpoints API
      ├── health.js  - Health check
      └── users.js   - Gestion des utilisateurs
```
