# Methodologie

- **Werktitel onderzoeksvoorstel:** Automatiseren en optimaliseren van de kwaliteitscontrole (QC) test op een PET-CT-scanner.
- **Naam Student:** Ulenaers Andries
- **URL Github repo:** https://github.com/Andries-U/RM2023Juni

## Plan van aanpak

### **Fase 1: Formuleren takenpakket voor plugin**

- **Doelstelling:** Begrijpen wat de plugin precies moet kunnen
- **Aanpak:**
  - Overlopen van de huidige werkwijze
  - Documenteren stappen die de plugin moet overnemen
  - Documenteren van onduidelijkheden + gaten in kennis die nodig is om de werking te begrijpen
- **Resultaat, deliverable(s):**
  - Verkrijgen van document die alle **uitkomsten** die de opdrachtgever wilt opsomt

### **Fase 2: Stand van zaken**

- **Doelstelling:** Hoe zit alles nu in elkaar. Geeft dit beperkingen voor ons?
- **Aanpak:**
  - Welke technologieën worden al gebruikt?
  - Waarom worden bepaalde technologieën gebruikt?
  - Zijn er toekomstplannen voor switchen waarmee we rekening kunnen houden?
- **Resultaat, deliverable(s):**
  - Welke technologieën gaan we onderzoeken

### **Fase 3: Begrijpen van alle facetten van de opdracht**

- **Doelstelling:** Verdiepen
- **Aanpak:**
  - Verdiepen in de globale werking van het toestel
  - Begrijpen werking van de specifieke bestandsformaten
  - Welke basisstructuren hebben we om mee te werken (deze opsommen)
- **Resultaat, deliverable(s):**
  - Deel 1 literatuurstudie
  - Verdere "versimpeling van probleem

### **Fase 4: Identificeren basisprobleem**

- **Doelstelling:** Het identificeren van het probleem in de meest simpele vorm
- **Aanpak:**
  - Blijven zoeken naar een simpelere vorm om het probleem te beschrijven
  - Zoveel mogelijk verwijderen van te specifieke ideeën en verwijderen overbodige stappen
- **Resultaat, deliverable(s):**
  - Duidelijke en meest simplistische probleemomschrijving.

### **Fase 5: Onderzoeken mogelijke technieken om probleem op te lossen**

- **Doelstelling:**
  - In de literatuur zoeken naar mogelijke manieren om het probleem op te lossen
- **Aanpak:**
  - Verder zoeken in de literatuur en eventuele fundamentele kennis
  - ideeën putten uit andere vakgebieden
- **Resultaat, deliverable(s):**
  - Literatuurstudie deel 2
  - Minstens 2 technieken die we kunnen gebruiken (liefst 4)

### **Fase 6: Coderen technieken**

- **Doelstelling:**
  - Prototypes coderen voor elke techniek die in [fase 5](#fase-5-onderzoeken-mogelijke-technieken-om-probleem-op-te-lossen) is geïdentificeerd
  - Deze prototypes moeten minstens de gewenste data geven voor verdere vergelijking
- **Aanpak:**
  - a.d.h.v. vakkennis en literatuurstudie deel 2 voor elke techniek een script/prototype maken die data geeft waarmee we een vergelijkende studie kunnen uitvoeren
- **Resultaat, deliverable(s):**
  - prototype voor elke techniek
  - uitgekomen data van elke techniek voor de verdere vergelijkende studie

### **Fase 7: Vergelijkende studie**

- **Doelstelling:**
  - bekomen van resultaten vergelijkende studie tussen de gekozen technieken en manueel werk
- **Aanpak:**
  - We vergelijken de bekomen kwantitatieve en kwalitatieve data
  - blinde studie met erkende fysici voor visuele beoordeling van alle resultaten
- **Resultaat, deliverable(s):**
  - bekomen van "best" scorende techniek
  - studie toont aan dat er minstens 1 techniek even goed of beter scoort dan de manuele huidige methode

### **Fase 8: Finalizeren proof-of-concept**

- **Doelstelling:**
  - Het volledig afwerken van een bruikbaar proof-of-concept
- **Aanpak:**
  - Verder uitwerken van gekozen beste techniek
  - drastisch reduceren eventuele foutmarge
  - introduceren controleerbare resultaten bij eventueel "vreemde" uitkomsten
  - Integratie in huidige workflow zoals geïdentificeerd in [fase 2](#fase-2-stand-van-zaken)
- **Resultaat, deliverable(s):**
  - proof-of-concept waarmee de partner in het onderzoek kan werken.

### **Finaliseren bachelor proef**

- **Doelstellingen**
  - Finaliseren van de bachelor proef
  - Poster maken
- **Resultaten**
  - Afgewerkte bachelorproef

## Verloop

### FlowChart

::: mermaid
graph LR;
    id1[Fase 1]-->id2[Fase 2];
    id1-->id4[Fase 4];
    id2-->id3[Fase 3];
    id3-->id5[Fase 5];
    id4-->id5;
    id5-->id6[Fase 6];
    id6-->id7[Fase 7];
    id7-->id8[Fase 8];
    id1 --> Literatuurstudie;
    Literatuurstudie --> id9[Finaliseren BP];
    id8--> id9;
:::

### Gantt-planning

::: mermaid
gantt
dateFormat YYYY-MM-DD
axisFormat %m-%d
tickInterval 1week
todayMarker off
title GANTT

Fase 1 :   des1, 2023-02-10, 7d
Fase 2    :   des2, after des1, 14d
Fase 3    :   des3, after des2, 7d
Fase 4    :   des4, after des1, 4d
Fase 5    :   des5, after des3 after des4, 14d
Fase 6    :   des6, after des5, 14d
Fase 7    :   des7, after des6, 3d
Fase 8    :   des8, after des7, 16d
Literatuurstudie  : des9, after des1, 2023-04-26
Finaliseren BP : des 10, after des8, 2023-05-29
:::