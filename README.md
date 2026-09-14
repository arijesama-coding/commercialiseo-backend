# Commercialiseo Backend

Backend REST API de la plateforme **Commercialiseo**, développée avec Node.js, Express et MongoDB.

Le backend assure la gestion de l'authentification, des utilisateurs, des produits, des catégories, des variants, des promotions, du panier et des commandes selon les rôles de la plateforme.

---

## Stack Technique

| Technologie | Version | Utilisation |
|------------|---------|-------------|
| Node.js | >= 18.0.0 | Runtime JavaScript |
| Express | 5.2.1 | Framework API REST |
| MongoDB | 6 | Base de données NoSQL |
| Mongoose | 9.2.1 | ODM MongoDB |
| JWT | 9.0.3 | Authentification |
| Bcrypt | 3.0.3 | Hachage des mots de passe |
| Nodemailer | 8.0.1 | Envoi d'emails |
| Winston | 3.11.0 | Logging |
| Multer | 2.1.0 | Upload de fichiers |

---

## Architecture

```text
Client Angular
      |
      | HTTP / HTTPS
      v
Express API
      |
      +--------------------+
      |                    |
      v                    v
  MongoDB              Services
                       |
                       +-- Authentification
                       +-- Utilisateurs
                       +-- Produits
                       +-- Catégories
                       +-- Variants
                       +-- Promotions
                       +-- Panier
                       +-- Commandes
                       +-- Emails
