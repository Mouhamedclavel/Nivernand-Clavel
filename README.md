[README_ExamenSOAP.md](https://github.com/user-attachments/files/21607865/README_ExamenSOAP.md)

📦 Projet ExamenSOAP - Service Web SOAP avec Spring Boot

🧾 Description

Ce projet est une application Java basée sur Spring Boot qui expose un Web Service SOAP pour gérer deux entités : Sector et Classe.  
Il permet de consommer, exposer et manipuler des données à travers des endpoints SOAP structurés à l’aide d’un schéma XSD.

 📁 Structure du projet

ExamenSOAP/
│
├── src/
│   ├── main/java/com/isi/examen/
│   │   ├── model/              Contient les entités Sector et Classe
│   │   ├── repository/         Accès aux données via JPA
│   │   ├── service/            Logique métier
│   │   ├── endpoint/           Endpoints SOAP
│   │   └── config/             Configuration Spring SOAP
│   └── resources/
│       ├── parametrage.xsd      Schéma XSD pour définir le contrat SOAP
│       └── application.properties
│
├── pom.xml                     Dépendances Maven
└── mvnw / mvnw.cmd             Wrapper Maven

 Lancement du projet

 Pré-requis :
- Java 17 ou plus
- Maven 3.6+
- IDE (Eclipse, IntelliJ...)

 Étapes :

1. Cloner ou importer le projet dans votre IDE :
git clone [votre_repo]

2. Lancer le projet :
./mvnw spring-boot:run


🔗 WSDL & Tests

- Le fichier parametrage.xsd est utilisé pour générer le WSDL.
- Le service est exposé à l'adresse :

  http://localhost:8080/ws


- Exemple d'endpoint disponible :
  - /ws/getSectorsRequest
  - /ws/getClassesRequest

- Testé avec **SoapUI** (soapuitest.png fourni comme exemple).


 🛠️ Fonctionnalités

- 🔍 Récupération des secteurs et des classes
- 💾 Stockage via Spring Data JPA
- 🔐 Séparation claire entre modèle, service et endpoint
- ⚙️ Configuration SOAP personnalisée

 Auteur

Nivernand Clavel KALLA DIELE  
© 2025 - Tous droits réservés

📸 Captures d’écran

- creation du projet sur springboot.png` – Création du projet
- soapuitest.png` – Test SOAP dans SoapUI

 Licence

Ce projet est à but éducatif dans le cadre d’un examen  de développement Java SOAP avec Spring Boot.
