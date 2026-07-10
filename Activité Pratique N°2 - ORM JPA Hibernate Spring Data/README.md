# Activite pratique 2 - ORM, JPA, Hibernate et Spring Data

## Objectif

Mettre en place la persistance Spring Boot, transformer des classes Java en
entites relationnelles et interroger les donnees avec Spring Data JPA.

## Fonctionnalites

- Entites `Patient`, `Medecin`, `RendezVous` et `Consultation`.
- Utilisateurs et roles applicatifs.
- Mapping des associations avec JPA.
- Repositories Spring Data et operations CRUD.
- Requetes derivees du nom des methodes.
- Base H2 en developpement et prise en charge de MySQL.

## Technologies

Java 17, Spring Boot 3.2.5, Spring Data JPA, Hibernate, H2, MySQL,
Lombok et Maven.

## Structure

```text
tp2-orm/src/main/java/ma/enset/
|-- entities/       Entites et enumerations JPA
|-- repositories/   Interfaces Spring Data
`-- Tp2OrmApplication.java
```

## Execution

```bash
cd tp2-orm
mvn clean spring-boot:run
```

La source de donnees se configure dans
`src/main/resources/application.properties`. Ne publiez pas de mot de passe
reel dans ce fichier.

## Resultat attendu

Spring initialise JPA et permet d'enregistrer, consulter, modifier et supprimer
les objets du domaine.

## Demonstration attendue

Cette activite est centree sur la persistance et ne fournit pas d'interface
graphique. Les donnees peuvent etre verifiees dans les journaux Spring Boot, la
console H2 ou avec un client SQL. Les captures pertinentes seraient donc celles
des tables generees et des requetes executees.

[Retour au README principal](../README.md)
