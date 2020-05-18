# test

Test d'utilisation Git/Maven

### Prerequis

Os Linux: Ubuntu/Debian

#### Install Java

- https://java.com/fr/download/help/linux_x64_install.xml
or
- https://openjdk.java.net/install/

#### Install Maven

- https://maven.apache.org/install.html

#### Install Git

- https://gist.github.com/derhuerst/1b15ff4652a867391f03

### Procédure

 - Cloner le projet de test
 
 ```
cd /somewhere/

git clone https://github.com/test35-max/test.git

cd ./test

```

 - Ce test à pour objectif l'utilisation de Maven, outil de build/compilation de projets Java/scala et autres.
L'objectif est double:

 - compiler le code du projet en utilisant Maven

 - lire le contenu d'un fichier avro présent dans le répertoire /src/main/resources/users.avro
 
 
 - Avro est un projet open-source de la fondation Apache fournissant un framework de serialisation/déserialisation d'objets, trés utile dans le contexte des applications Big data.
 
 - https://avro.apache.org/
 
 -1) rajouter au fichier pom.xml, la dépendance correspondant à la librairie avro-1.8.2
 
 -2) vérifier que le code compile
 
 -3) Dans la classe fr.dga.App.java, implémenter la méthode readAvro(), de telle sorte à ce qu'elle lise le fichier users.avro et affiche les noms et prénoms de chaque utilisateur présent.
 
 
 
 ### Questions
 
  - Combien d'utilisateurs sont contenus dans le fichier?
  - Fournir la liste de leurs noms et prénoms
  - Quelle est la commande maven permettant de générer le jar test-1.0-SNAPSHOT.jar