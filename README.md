# Projet Banque

Ce projet implémente une application bancaire avec la modélisation JPA. Les entités JPA ont été créées en suivant le modèle UML fourni.

## Configuration du projet

1. **Structure du projet :**
   - Assurez-vous que votre projet suit une structure similaire à celle-ci :

     ```
     banque-project/
     |-- src/
     |   |-- main/
     |   |   |-- java/
     |   |   |   |-- com/
     |   |   |       |-- example/
     |   |   |           |-- model/
     |   |   |               |-- Banque.java
     |   |   |               |-- Compte.java
     |   |   |               |-- Operation.java
     |   |   |               |-- Client.java
     |   |   |               |-- Adresse.java
     |   |   |
     |   |   |-- resources/
     |   |       |-- META-INF/
     |   |           |-- persistence.xml
     |   |
     |-- target/
     |-- pom.xml
     |-- .gitignore
     ```

2. **Configuration de la base de données :**
   - Créez une nouvelle base de données appelée "banque".

3. **Persistence Unit (unité de persistance) :**
   - Assurez-vous que le fichier `persistence.xml` est correctement configuré dans `src/main/resources/META-INF/`. Vérifiez que l'unité de persistance est nommée "banquePU" et que les propriétés de connexion à la base de données sont correctes.

4. **Dépendances Maven :**
   - Assurez-vous que les dépendances nécessaires, telles que Hibernate, sont correctement spécifiées dans le fichier `pom.xml`.

   Exemple :

   ```xml
   <dependencies>
       <!-- Autres dépendances... -->
       <dependency>
           <groupId>org.hibernate</groupId>
           <artifactId>hibernate-core</artifactId>
           <version>5.6.15.Final</version>
       </dependency>
       <!-- Autres dépendances... -->
   </dependencies>
