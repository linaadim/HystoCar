🚗 HystoCar
HystoCar est une application multiplateforme (Android, iOS, Windows) développée avec **Xamarin** et basée sur une architecture **microservices**.  
Elle vise à simplifier et optimiser la gestion des véhicules pour les particuliers, gestionnaires de flotte et professionnels de l’automobile.  

🎯 Objectifs du projet
 Centralisation des données 
   Regrouper toutes les informations importantes des véhicules (contrôle technique, historiques de maintenance, prestations de service) dans une plateforme unique et accessible.

 Facilitation du suivi  
   Envoi de rappels automatiques pour les échéances (contrôles, entretiens, services), afin d’assurer une gestion proactive et efficace.

 Optimisation des processus 
   Automatisation de tâches comme la planification des interventions et la gestion documentaire, réduisant le temps perdu et les risques d’oubli.

 Amélioration de l’expérience utilisateur
   Interface fluide et intuitive, adaptée aussi bien aux particuliers qu’aux professionnels.


🏗️ Architecture du projet

Le projet est organisé en plusieurs microservices/modules principaux :

 HystoCar.API
- Responsable de l’interface côté serveur, exposant des endpoints REST pour les clients.
- Dossiers clés :
  - `Controllers/` : Gestion des requêtes HTTP entrantes.
  - `Data/` : Gestion des données et contextes spécifiques.
  - `appsettings.json` : Configuration (ex. chaînes de connexion).
  - `Program.cs` : Point d’entrée principal.
  - `Startup.cs` : Configuration des services et pipeline.
  - `WeatherForecast.cs` : Exemple de ressource.


  HystoCar.Core
- Contient la logique métier et les interfaces principales.
- Dossiers clés :
  - `Models/` : Entités du domaine.
  - `Repositories/` : Interfaces et implémentations de dépôts.
  - `Services/` : Logique métier (opérations complexes).
  - `IUnitOfWork.cs` : Interface du pattern **Unit of Work**.


 HystoCar.Data
- Gestion de l’accès aux données et des migrations.
- Dossiers clés :
  - `Configuration/` : Configurations spécifiques de la DB.
  - `Mappings/` : Mapping entités ↔ tables.
  - `Migrations/` : Historique et gestion des schémas DB.
  - `Repositories/` : Accès aux données.
  - `HystoCarDbContext.cs` : Contexte de la base de données.
  - `UnitOfWork.cs` : Implémentation de l’unité de travail.



HystoCar.Services
- Services supplémentaires (infrastructure, auxiliaires, isolés).
- Utilisé pour séparer des fonctionnalités ne relevant pas directement du **Core**.

<img width="230" height="484" alt="image" src="https://github.com/user-attachments/assets/33f840c1-8fda-4fb8-ad51-a772f1f2eae8" />

 📱 Plateformes cibles

- Android (Xamarin.Android)  
- iOS (Xamarin.iOS)  
- Windows (UWP ou Xamarin.Forms)  



 ⚙️ Technologies utilisées

- Backend: ASP.NET Core, C#  
- Frontend Mobile/Desktop : Xamarin  
- Base de données : SQL Server
- Architecture : Microservices



 Cloner le repository :  
   ```bash
   git clone https://github.com/votre-repo/HystoCar.git
