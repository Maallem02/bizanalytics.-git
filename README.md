cat > README.md << 'EOF'
# 📊 BizAnalytics — Business Analytics pour petits commerces

Application web MEAN Stack complète pour la gestion et l'analyse des ventes et dépenses.

## 🚀 Technologies utilisées

| Couche | Technologie |
|--------|-------------|
| Base de données | MongoDB Atlas + Mongoose |
| Backend | Node.js + Express |
| Frontend | Angular 17 |
| Graphiques | Chart.js |
| Auth | JWT (JSON Web Token) |

## ✨ Fonctionnalités

- 🔐 Authentification JWT (login / register)
- 📊 Dashboard avec KPIs (ventes, dépenses, bénéfice, marge)
- 💰 CRUD complet des ventes
- 💸 CRUD complet des dépenses
- 📥 Import Excel des ventes
- 📈 Graphiques automatiques (barres, camembert, courbe)

## 📁 Structure du projet

\`\`\`
bizanalytics/
├── backend/
│   ├── config/        → connexion MongoDB
│   ├── models/        → modèles Mongoose
│   ├── services/      → logique métier
│   ├── controllers/   → gestion requêtes HTTP
│   ├── routes/        → définition des routes API
│   ├── middleware/    → JWT + gestion erreurs
│   └── server.js      → point d'entrée
└── frontend/
    └── src/app/
        ├── core/      → services, guards, interceptors
        ├── modules/   → dashboard, ventes, dépenses, auth
        └── shared/    → sidebar, navbar, layout
\`\`\`

## ⚙️ Installation

### Backend
\`\`\`bash
cd backend
npm install
# Créer .env avec MONGO_URI et JWT_SECRET
node server.js
\`\`\`

### Frontend
\`\`\`bash
cd frontend
npm install
ng serve
\`\`\`

## 🌐 API Endpoints

| Méthode | Route | Description |
|---------|-------|-------------|
| POST | /api/auth/register | Inscription |
| POST | /api/auth/login | Connexion |
| GET | /api/ventes | Toutes les ventes |
| POST | /api/ventes | Créer une vente |
| PUT | /api/ventes/:id | Modifier une vente |
| DELETE | /api/ventes/:id | Supprimer une vente |
| GET | /api/depenses | Toutes les dépenses |
| POST | /api/depenses | Créer une dépense |
| GET | /api/dashboard | KPIs + graphiques |

## 👤 Compte de test

- Email : demo@bizanalytics.tn
- Mot de passe : demo123

## 🎓 Projet académique — Polytech Monastir
EOF
