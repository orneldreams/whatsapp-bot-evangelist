# WhatsApp Bot Evangelist

**Description**:
Ce projet vise à créer un chatbot intelligent et automatisé, spécialisé pour un usage évangélique. Le bot communique via WhatsApp avec plusieurs personnes dans le monde entier. Il est conçu pour :
- Envoyer des messages personnalisés en fonction des besoins de l'utilisateur.
- Centraliser et suivre toutes les conversations via une base de données.
- Être extensible et évolutif grâce à des technologies modernes comme Twilio, Redis, PostgreSQL, etc.

**Technologies prévues**:
- **Backend**: Node.js avec NestJS pour la gestion des API et la logique métier.
- **Base de données**: PostgreSQL pour la gestion des données relationnelles.
- **Queues**: Redis (avec BullMQ) pour gérer les tâches différées comme les rappels.
- **Interface WhatsApp**: Twilio API.
- **Frontend**: React.js pour le tableau de bord utilisateur (hébergé sur Vercel).

**Étapes pour démarrer**:
1. Clonez ce dépôt :
```
git clone https://github.com/orneldreams/whatsapp-bot-evangelist.git
cd whatsapp-bot-evangelist
```

2. Installez les dépendances :
```
npm install
```

3. Configurez les variables d'environnement :
Créez un fichier `.env` à la racine, par exemple :
```
TWILIO_ACCOUNT_SID=YourTwilioAccountSID
TWILIO_AUTH_TOKEN=YourTwilioAuthToken
POSTGRES_URL=YourPostgresDatabaseURL
REDIS_URL=YourRedisURL
```

4. Lancez l'application en mode développement :
```
npm run start:dev
```

**Fonctionnalités principales**:
- Gestion des utilisateurs via WhatsApp.
- Questions personnalisées et suivi des réponses.
- Notifications automatisées basées sur des files d'attente.

**Plan d'évolution**:
- Intégrer un moteur NLP comme Dialogflow ou Rasa.
- Ajouter la prise en charge multicanal (SMS, E-mail).