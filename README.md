# 🎵 BeatMarket Admin Panel

Panneau administrateur pour BeatMarket - Une plateforme de streaming musical avec gestion des utilisateurs, des tracks et des revenus.

## 🚀 Déploiement sur Vercel

### Prérequis
- Compte Vercel (gratuit)
- Accès au dépôt GitHub
- Compte Supabase (base de données)

### Étapes de déploiement

1. **Fork ou clone ce dépôt**
   ```bash
   git clone https://github.com/jonathankabre98-debug/beatmarket-admin.git
   ```

2. **Connecte-toi à Vercel**
   - Va sur [vercel.com](https://vercel.com)
   - Clique sur "New Project"
   - Sélectionne ton dépôt GitHub

3. **Configure les variables d'environnement (optionnel)**
   - Les clés Supabase sont codées en dur dans `public/index.html`
   - Tu peux les modifier directement dans le fichier ou utiliser les variables Vercel

4. **Déploie**
   - Clique sur "Deploy"
   - Attends la fin du déploiement
   - Accède à ton app via l'URL fournie par Vercel

## 📂 Structure du projet

```
beatmarket-admin/
├── public/
│   └── index.html          # App React statique
├── vercel.json            # Configuration Vercel
├── package.json           # Dépendances (minimal)
├── .gitignore            # Fichiers à ignorer
└── README.md             # Ce fichier
```

## 🔐 Sécurité

- Les clés Supabase sont publiques (c'est normal pour les clés anon)
- Les données sensibles restent protégées par les RLS de Supabase
- Modifie les emails admins dans `SUPER_ADMINS` en haut du script

## 📝 Variables d'environnement

Les variables suivantes peuvent être définies sur Vercel :

```
SUPABASE_URL=https://your-project.supabase.co
SUPABASE_ANON_KEY=your_supabase_anon_key
```

## 🛠️ Développement local

```bash
# Démarrer un serveur local
npm run dev

# Accède à http://localhost:3000
```

## 📊 Fonctionnalités

- 📈 Dashboard en temps réel
- 👥 Gestion des utilisateurs
- 🎵 Gestion des tracks (musiques)
- 📺 Analyse des publicités
- 🌍 Statistiques par pays
- 👑 Gestion des premium
- 🛡️ Gestion des administrateurs
- 🔔 Centre de notifications

## 🤝 Support

Pour toute question, crée une issue sur GitHub.

## 📄 Licence

MIT
