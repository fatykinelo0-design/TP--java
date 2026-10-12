TP Java — JDK et Maven

1. Présentation du projet

Ce dépôt contient les travaux pratiques réalisés pour apprendre à utiliser Java, le JDK, Maven et Git.

Il contient trois projets :

* tp-env-java : découverte de l’environnement Java et de Maven.
* projet-java21 : projet utilisant le JDK 21.
* projet-java25 : projet utilisant le JDK 25.

2. Installation du JDK

Le JDK (Java Development Kit) permet de développer des applications Java. Il contient notamment le compilateur javac et la commande java.

Pour vérifier l’installation du JDK, ouvrir un terminal et exécuter :

java -version
javac -version

Ces commandes permettent de vérifier les versions de Java et du compilateur installés.

3. Installation de Maven

Maven est un outil qui permet de gérer les dépendances et de compiler un projet Java.

Pour vérifier son installation, exécuter :

mvn -version

Cette commande affiche notamment la version de Maven et le JDK utilisé.

4. Compiler un projet avec Maven

Dans le terminal, se placer dans le dossier contenant le fichier pom.xml, puis exécuter :

mvn compile

Cette commande compile les sources Java du projet.

5. Changer de JDK selon le projet

Plusieurs versions du JDK peuvent être installées sur un même ordinateur.

Dans VS Code, il est possible de sélectionner un JDK pour un projet avec la palette de commandes :

1. Appuyer sur Ctrl + Shift + P.
2. Rechercher Java: Configure Java Runtime.
3. Vérifier les JDK détectés.
4. Sélectionner le JDK adapté au projet.

Il faut également vérifier la configuration Maven du projet, notamment les propriétés maven.compiler.release du fichier pom.xml.

Pour utiliser le JDK 21, le projet doit être configuré pour compiler avec Java 21. Pour utiliser le JDK 25, il doit être configuré pour compiler avec Java 25.

6. Vérification des projets

Pour vérifier le projet Java 21 :

cd projet-java21
java -version
mvn compile

Pour vérifier le projet Java 25 :

cd ../projet-java25
java -version
mvn compile

Les commandes doivent être exécutées dans les dossiers correspondants.

7. Gestion du code avec Git

Git permet de suivre les modifications du projet et GitHub permet de stocker le dépôt en ligne.

Les commandes principales utilisées sont :

git status
git add .
git commit -m "Message explicite"
git push

Plusieurs commits explicites permettent de conserver l’historique des modifications.