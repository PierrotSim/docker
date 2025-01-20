Voici les instruction pour le TP blog_minimalist :

```markdown
# Minimalist Blog - Installation et configuration

Suivez les étapes ci-dessous pour cloner et configurer le projet.

## 1. Cloner le repository

Clonez le repository avec la commande suivante :

```bash
git clone https://github.com/RMarcAntoine/Minimalist-_-Blog.git
```

## 2. Accéder au répertoire du projet

Changez de répertoire pour accéder au dossier du projet :

```bash
cd Minimalist-_-Blog
```

## 3. Ouvrir le projet dans VS Code

Ouvrez le projet avec VS Code :

```bash
code .
```

## 4. Configurer l'environnement

Copiez le fichier `.env.example` pour créer un fichier `.env` :

```bash
cp .env.example .env
```

## 5. Installer les dépendances avec Docker

Exécutez la commande suivante pour installer les dépendances via Composer dans un conteneur Docker :

```bash
docker run --rm --interactive --tty \
  --volume $PWD:/app \
  composer install
```

## 6. Démarrer Sail

Démarrez le conteneur Docker avec Sail :

```bash
./vendor/bin/sail up -d
```

## 7. Générer la clé d'application

Générez la clé d'application avec Artisan :

```bash
./vendor/bin/sail artisan key:generate
```

## 8. Effectuer les migrations de la base de données

Exécutez les migrations de la base de données :

```bash
./vendor/bin/sail artisan migrate
```

## 9. Installer les dépendances front-end

Installez les dépendances front-end avec NPM :

```bash
./vendor/bin/sail npm install
```

## 10. Lancer le développement

Démarrez le serveur de développement front-end :

```bash
./vendor/bin/sail npm run dev
```

## Conclusion

Votre projet devrait maintenant être configuré et prêt à l'emploi !



J'ai cependant eux plusieurs (beaucoup) de soucis pour le faire fonctionner correctement sur mon poste. 😒

