## 🌟 JM Group 🌟

Mød det dedikerede team bag **JM Group**, som arbejder hårdt for at bringe MyDRTV-projektet til live!

- **👤 Mohamed Salim**  
  [🔗 LinkedIn](https://www.linkedin.com/in/mohamed-salim-467a93235/)  

- **👤 Jamal Ahmed**  
  [🔗 LinkedIn](https://www.linkedin.com/in/jamal-ahmed-7b4531169/)  

---

# 🌟 Projektoversigt: MyDRTV 🌟

## 📺 Projektoversigt
Velkommen til **MyDRTV**! Dette innovative projekt er fokuseret på at skabe en banebrydende videoplayer og et socialt netværk for Danmarks statsmedie. Vores mission? At præsentere og promovere dansk tv og film globalt og gøre en skattekiste af klassiske tv-programmer tilgængelige for publikum over hele verden! 🌍

Vi udforsker outsourcing-muligheder for at optimere udviklingsomkostningerne, især i Østeuropa og Asien, og vil omhyggeligt definere løsningsarkitekturen og teknologistakken for at opfylde både økonomiske og funktionelle krav. 💻

## 📜 Krav
MyDRTV-platformen er designet med fokus på brugervenlighed og indeholder en række vigtige funktioner:

- **👤 Brugerkonti:** Brugere kan oprette personlige konti for en skræddersyet oplevelse.
- **⭐ Bedømmelsessystem:** Brugere kan bedømme programmer og dele deres meninger gennem fællesskabsdrevne evalueringer.
- **🔍 Søgefunktionalitet:** En alsidig søgemaskine gør det muligt for brugere at finde film og tv-shows ud fra forskellige kriterier som:
  - Produktionsår
  - Titel
  - Genre

### ⚡ Høj Tilgængelighed
At sikre høj tilgængelighed er afgørende på grund af de omdømmemæssige risici, der er forbundet med at levere en pålidelig og engagerende brugeroplevelse. Vores system vil integrere et populært bedømmelsessystem for at fremme brugerinteraktion og skabe livlige samtaler om klassiske tv-programmer og film. 🗣️

### 🚀 Digitale Transformationsmål
MyDRTV er en nøglekomponent i Danmarks Radio's

## 🔍 Arkitektoniske Valg

### 🏗️ Sammenligning af Arkitekturstilarter
I vores systematiske tilgang har vi sammenlignet to fremtrædende arkitekturstilarter: **lagdelt arkitektur** og **mikroservices-arkitektur**. Nedenfor præsenteres en grundig analyse af hver arkitekturtype baseret på nøglekriterier, som er inspireret af Mark Richards' *Software Architecture Patterns*.

#### 📦 Lagdelt Arkitektur
- **Beskrivelse**: Lagdelt arkitektur organiserer systemet i separate lag, hvor hvert lag har en specifik rolle. Typisk inkluderer disse lag:
  - **Præsentationslag**: Håndterer brugergrænsefladen og interaktioner.
  - **Forretningslag**: Implementerer forretningslogikken og reglerne.
  - **Datatilgangslag**: Kommunikerer med databasen og styrer dataopbevaringen.

- **Fordele**:
  - **Struktureret tilgang**: Giver en klar opdeling af ansvar, hvilket kan føre til lettere vedligeholdelse og forståelse af systemet.
  - **Modularitet**: Ændringer i et lag kan implementeres uden at påvirke de andre lag, hvilket giver en vis grad af fleksibilitet.

- **Udfordringer**:
  - **Skalérbarhed**: Lagdelt arkitektur har begrænset skalérbarhed, da det kan være svært at skalere individuelle lag uafhængigt.
  - **Ydelse**: Hver lagdelt struktur kan introducere latens, da data skal passere gennem flere lag.

#### ⚙️ Mikroservices Arkitektur
- **Beskrivelse**: Mikroservices-arkitektur opdeler applikationen i små, uafhængige tjenester, der kommunikerer via API'er. Hver mikroservice fokuserer på en specifik forretningsfunktion eller proces.

- **Fordele**:
  - **Skalérbarhed**: Tjenester kan skaleres uafhængigt baseret på belastning og efterspørgsel.
  - **Fleksibilitet**: Hurtig implementering og opdatering af funktioner, da hver mikroservice kan opdateres uafhængigt.
  - **Moderne teknologistak**: Hver mikroservice kan bruge forskellige teknologier og programmeringssprog.

- **Udfordringer**:
  - **Kompleksitet**: Orkestrering og administration af mange tjenester kan være komplekst.
  - **Kommunikation**: Kræver pålidelige mekanismer til kommunikation mellem tjenesterne.

### ⚖️ Sammenligning af Kriterier

| Kriterier               | Lagdelt Arkitektur                                          | Mikroservices Arkitektur                                    |
|-------------------------|-----------------------------------------------------------|------------------------------------------------------------|
| **Skalérbarhed**        | Begrænset skalérbarhed; sværere at skalere individuelle komponenter. | Meget skalerbar; tjenester kan skaleres uafhængigt.       |
| **Fleksibilitet**       | Mere rigid; ændringer i ét lag kan påvirke andre.        | Meget fleksibel; individuelle tjenester kan opdateres uden at påvirke andre. |
| **Vedligeholdelse**     | Moderat vedligeholdelse; kræver omhyggelig styring af lagene. | Høj vedligeholdelse; hver tjeneste kan udvikles og vedligeholdes uafhængigt. |
| **Ydelse**              | Kan forringes med flere lag; potentielle latensproblemer. | Forbedret ydelse; letvægts tjenester kan håndtere forespørgsler hurtigt. |
| **Udviklingstid**       | Længere på grund af integration af forskellige lag.       | Kortere for uafhængige tjenester; teams kan arbejde samtidigt. |
| **Udrulningskompleksitet** | Simpel; enkelt udrulning for hele applikationen.         | Mere kompleks; kræver orkestrering og styring af flere tjenester. |
| **GDPR-overholdelse**   | Potentielt lettere at håndtere data i et centraliseret lag. | Kræver omhyggelig design for at sikre overholdelse på tværs af distribuerede tjenester. |
| **Brugerengagement**    | Kan implementere engagementsfunktioner i UI-laget.       | Muliggør målrettede engagementsfunktioner via mikroservices. |

### 🏆 Valgt Arkitektur
Baseret på ovenstående analyse har vi valgt **mikroservices-arkitektur** som den mest passende løsning for MyDRTV. Denne beslutning er truffet efter nøje overvejelse af projektets krav og de fordele, som mikroservices tilbyder. De specifikke beslutninger inkluderer:

- **Serviceopdeling**: Identifikation af specifikke forretningsfunktioner, der skal implementeres som separate tjenester, såsom brugeroprettelse, ratingsystem, søgefunktionalitet og programmetadatahåndtering.
  
- **Kommunikationsprotokoller**: Valg af kommunikationsprotokoller, såsom RESTful API'er eller gRPC, for effektiv interaktion mellem mikroservices. Implementering af en API-gateway til at styre indkommende anmodninger.

- **Datahåndtering og -lagring**: Beslutning om datahåndtering, herunder valg af databaser og strategier for datareplikation og -synkronisering, herunder muligheden for hver mikroservice at have sin egen database for at sikre uafhængighed.

## 📊 Diagrams
Vi vil inkludere følgende diagram for at visualisere arkitekturen:
- **Sekvensdiagram**: Detaljer interaktioner mellem brugergrænsefladen, mikroservices og databasen under handlinger som at indsende en vurdering.

# MyDRTV Sequence Diagrams


## Table of Contents
1. [User Registration and Login](#1-user-registration-and-login)
2. [Viewing and Rating a Program](#2-viewing-and-rating-a-program)
3. [Search and Recommendation Generation](#3-search-and-recommendation-generation)

## 1. User Registration and Login

This sequence diagram focuses on how a user registers and logs in to the system.

### **Actors and Components**
- **User**: The person interacting with the system.
- **UI/Client**: The frontend interface.
- **User Service**: Handles user registration, login, and GDPR.
- **GDPR Compliance Service**: Handles GDPR consent.
- **Database**: Stores user information.

### **Sequence**
1. **User** ➔ **UI/Client**: Enters registration information.
2. **UI/Client** ➔ **User Service**: `RegisterUser` command with user info.
3. **User Service** ➔ **GDPR Compliance Service**: Verifies GDPR consent.
4. **GDPR Compliance Service** ➔ **User Service**: GDPR consent validation result.
5. **User Service** ➔ **Database**: Stores user information.
6. **Database** ➔ **User Service**: Confirmation of user storage.
7. **User Service** ➔ **UI/Client**: Registration confirmation.
8. **User** ➔ **UI/Client**: Logs in with credentials.
9. **UI/Client** ➔ **User Service**: `LoginUser` command.
10. **User Service** ➔ **Database**: Validates credentials.
11. **Database** ➔ **User Service**: Login success/failure.
12. **User Service** ➔ **UI/Client**: Login response.

## 2. Viewing and Rating a Program

This diagram captures the scenario of viewing a TV program and submitting a rating.

### **Actors and Components**
- **User**: The person interacting with the system.
- **UI/Client**: The frontend interface.
- **Content Service**: Handles content requests.
- **User Service**: Validates user session.
- **Rating Service**: Manages rating submissions.
- **Database**: Stores content and ratings data.

### **Sequence**
1. **User** ➔ **UI/Client**: Searches for a TV program.
2. **UI/Client** ➔ **Content Service**: `PerformSearch` with search terms.
3. **Content Service** ➔ **Database**: Retrieves matching programs.
4. **Database** ➔ **Content Service**: Returns search results.
5. **Content Service** ➔ **UI/Client**: Displays search results.
6. **User** ➔ **UI/Client**: Selects a program to view.
7. **UI/Client** ➔ **Content Service**: `ViewProgram` command.
8. **Content Service** ➔ **Database**: Retrieves program details.
9. **Database** ➔ **Content Service**: Returns program information.
10. **Content Service** ➔ **UI/Client**: Displays program details.
11. **User** ➔ **UI/Client**: Submits a rating.
12. **UI/Client** ➔ **User Service**: Validates user session.
13. **User Service** ➔ **UI/Client**: Session valid.
14. **UI/Client** ➔ **Rating Service**: `RateProgram` command with rating details.
15. **Rating Service** ➔ **Database**: Stores the rating.
16. **Database** ➔ **Rating Service**: Confirmation of storage.
17. **Rating Service** ➔ **UI/Client**: Rating submission confirmation.

## 3. Search and Recommendation Generation

This diagram covers how a user searches for a program and receives recommendations.

### **Actors and Components**
- **User**: The person interacting with the system.
- **UI/Client**: The frontend interface.
- **Search Service**: Handles search queries.
- **Recommendation Service**: Generates personalized recommendations.
- **Database**: Stores program and user interaction data.

### **Sequence**
1. **User** ➔ **UI/Client**: Enters search criteria.
2. **UI/Client** ➔ **Search Service**: `PerformSearch` command.
3. **Search Service** ➔ **Database**: Searches for programs based on criteria.
4. **Database** ➔ **Search Service**: Returns search results.
5. **Search Service** ➔ **UI/Client**: Displays search results.
6. **User** ➔ **UI/Client**: Views a program.
7. **UI/Client** ➔ **Recommendation Service**: Triggers `GenerateRecommendations` based on the program viewed.
8. **Recommendation Service** ➔ **Database**: Retrieves user preferences and interaction history.
9. **Database** ➔ **Recommendation Service**: Returns relevant data.
10. **Recommendation Service** ➔ **Database**: Fetches recommended content.
11. **Database** ➔ **Recommendation Service**: Returns recommended content.
12. **Recommendation Service** ➔ **UI/Client**: Displays recommendations to the user.



## 🎉 Konklusion
MyDRTV-projektet er ikke bare underholdning; det handler om at fejre og bevare den kulturelle arv i Danmark, samtidig med at vi overholder globale standarder for databeskyttelse. Vi ser frem til at realisere dette spændende projekt! 

## 📚 Referencer
- Mark Richards, *Software Architecture Patterns* (O'Reilly, 2022).
