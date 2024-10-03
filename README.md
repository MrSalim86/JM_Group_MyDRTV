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
Vi vil inkludere følgende diagrammer for at visualisere arkitekturen:
- **Use Case Diagram**: Vis brugerinteraktioner som oprettelse af konti, vurdering af programmer og søgning efter indhold.
- **Domænemodel**: Illustrer nøgleenheder (Bruger, Program, Vurdering) og deres relationer.
- **Aktivitetsdiagram**: Skildre brugerflows for almindelige handlinger som at vurdere et program.
- **Sekvensdiagram**: Detaljer interaktioner mellem brugergrænsefladen, mikroservices og databasen under handlinger som at indsende en vurdering.

## 🎉 Konklusion
MyDRTV-projektet er ikke bare underholdning; det handler om at fejre og bevare den kulturelle arv i Danmark, samtidig med at vi overholder globale standarder for databeskyttelse. Vi ser frem til at realisere dette spændende projekt! 

## 📚 Referencer
- Mark Richards, *Software Architecture Patterns* (O'Reilly, 2022).
