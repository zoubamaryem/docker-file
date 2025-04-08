# Spécifie l'image de base
FROM node:18

# Crée et définit le répertoire de travail
WORKDIR /app

# Copie le package.json et package-lock.json (si existant)
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie tout le reste du code source dans l'image
COPY . .

# Expose le port sur lequel ton app écoute
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["npm", "start"]
