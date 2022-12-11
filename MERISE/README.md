# Merise

Merise est une méthode trés orienté données relationnels, elle est spécifiaue au théritoire français, Merise prévilégie la donnée contrairement à l'UML qui lui privilège la donnée.

## MCD

Le MCD (Modéle conceptuel de donnée) à pour but d'écrire de manière formelle les données d'un système d'information.

### Les composants

Le MCD est composé de :

- L'entité : C'est un objet ou un individu, deux objets ne peuvent pas avoir le même nom.
- L'association : Lien, relations entre les différentes entités.
- Les propriétés : Attributs.
- Les identifiants d'entité et d'association.
- Les cardinalités : Contraintes d'intéractions.
- Les occurences : Instances, l'instances représente la donnée stockée sur une ligne, elle n'est pas repésenté sur le MCD.

## Dictionnaire de données

### Table Clients

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description** |
| -------------- | ------------- | ---------------- | -------------- | --------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Client id       |

### Table Reservations

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description**           |
| -------------- | ------------- | ---------------- | -------------- | ------------------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Reservation id            |
| price          | DOUBLE        | 11               | NOT NULL       | Reservation price         |
| start          | VARCHAR       | 50               | NOT NULL       | Resarvation airport start |
| end            | VARCHAR       | 50               | NOT NULL       | Resarvation airport end   |

### Table vols

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description**   |
| -------------- | ------------- | ---------------- | -------------- | ----------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Client id         |
| id_reservation | INTEGER       | 11               | NOT NULL       | Id of reservation |
| airport        | VARCHAR       | 50               | NOT NULL       | Airport of escale |

### Table Passagers

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description**           |
| -------------- | ------------- | ---------------- | -------------- | ------------------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Client id                 |
| id_reservation | INTEGER       | 11               | NOT NULL       | Id of reservation         |
| name           | VARCHAR       | 50               | NOT NULL       | Name of passanger         |
| lastname       | VARCHAR       | 50               | NOT NULL       | Lastname of passanger     |
| mail           | VARCHAR       | 50               | NOT NULL       | Mail of passanger         |
| phone          | INTEGER       | 10               | NOT NULL       | Phone number of passanger |

### Table billet vol

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description** |
| -------------- | ------------- | ---------------- | -------------- | --------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Billet id       |
| id_vol         | INTEGER       | 11               | NOT_NULL       | Vol id          |

### Table billet reservation

| **Field Name** | **Data Type** | **Field Length** | **Constraint** | **Description** |
| -------------- | ------------- | ---------------- | -------------- | --------------- |
| id             | INTEGER       | 11               | PrimaryKey     | Billet id       |
| id_reservation | INTEGER       | 11               | NOT_NULL       | Reservation id  |
