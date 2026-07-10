# Projet bancaire - Spring, Angular, JWT et Spring Security

## Objectif

Plateforme bancaire pour gerer clients, comptes et operations avec une API
securisee, une interface Angular et une extension chatbot.

## Partie 1 - Backend Java

- Entites : clients, comptes courants/epargne et operations.
- Repositories Spring Data.
- DTO et mappers pour separer API et persistance.
- Services de debit, credit et transfert.
- Controleurs REST pour clients et comptes.
- Validation, audit JPA et documentation Swagger/OpenAPI.

Le fichier Maven se trouve dans `Partie 1 (JAVA)/pom.xml`.

## Partie 2 - Frontend Angular

Le frontend comprend le tableau de bord, la gestion des clients et les services
d'authentification et d'acces aux fonctions bancaires.

## Partie 3 - Securite JWT

Spring Security authentifie les utilisateurs et protege les routes. Le backend
produit et verifie les JWT ; Angular les transmet lors des requetes.

## Partie 4 - Chatbot et IA

Cette partie explore Spring AI, le RAG et un bot Telegram. Le fichier
`conditions-bancaires.txt` constitue la documentation locale du chatbot.

## Flux global

```text
Angular -> JWT -> API Spring Boot -> services -> comptes et operations
                    |
                    `-> Spring Security

Telegram -> Bot -> Spring AI / RAG -> documentation bancaire
```

## Demarrage

1. Configurer la base et les variables d'environnement.
2. Compiler le backend avec `mvn clean package` dans `Partie 1 (JAVA)`.
3. Demarrer l'application Spring Boot.
4. Demarrer Angular avec `npm install` puis `npm start`.
5. Utiliser Swagger pour tester les endpoints.

## Securite

Ne versionnez jamais mots de passe, tokens ou cles API. Utilisez des variables
d'environnement, encodez les mots de passe, limitez la duree des JWT, validez
les entrees et restreignez les endpoints selon les roles.

## Interfaces a documenter

Le dossier fournit actuellement des extraits de composants et de services,
mais pas encore une application Angular complete directement executable. Les
captures seront ajoutees lorsque les ecrans suivants seront integres :

- authentification ;
- tableau de bord bancaire ;
- liste et formulaire des clients ;
- details d'un compte et historique des operations ;
- formulaire de debit, credit et transfert ;
- interface du chatbot.

[Retour au README principal](../README.md)
