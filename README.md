# Flask-prosjekt -- Dokumentasjon

## 1. Forside

**Barberens tidssporing:**\
**Felix**\
**2IMI**\
**11.11.25**

Applikasjonen min bygger på barberyrket mitt Barberens tidssporing er et digitalt system som hjelper barberen å holde oversikt over kunder, hårtype, behandlingstyper og hvor lang tid hver behandling tar. 

Systemet gjør det enkelt å loggføre hver kunde, lagre informasjon om hårtype, pris og tidsbruk, og vise statistikk over arbeidet.
Prosjektet er utviklet med Flask, MariaDB og Raspberry Pi og kombinerer programmering, databasestruktur og drift i ett fungerende system.

 
------------------------------------------------------------------------

## 2. Systembeskrivelse

**Formål med applikasjonen:**\
Formålet med applikasjonen Barberens tidssporing er å lage et enkelt system som hjelper en barber med å holde oversikt over kundene sine.

Jeg ville lage et sted der jeg kan registrere informasjon om hver kunde, som hårtype, behandling, pris og hvor lang tid jeg brukte.
På den måten kan jeg lettere se hva slags behandlinger som tar mest tid, og få bedre kontroll over arbeidet mitt.
Jeg ønsket også å vise at jeg kan bruke Flask og MariaDB sammen, og sette opp alt på en Raspberry Pi slik at systemet kjører som en ekte webapplikasjon.

**Brukerflyt:**\
*Nettsiden er ganske simpel på hjemmsiden ser du en knapp, hvor det står legg inn kunde. Du kommer dermed inn på en helt ny side der du fyller på ønskendene informasjon om kunden.*

**Teknologier brukt:**

-   Python / Flask\
-   MariaDB\
-   HTML / CSS / JS\
-   (valgfritt) Docker / Nginx / Gunicorn / Waitress osv.

------------------------------------------------------------------------

## 3. Server-, infrastruktur- og nettverksoppsett

### Servermiljø

*F.eks.: Ubuntu VM, Docker, fysisk server.*

### Nettverksoppsett

-   Nettverksdiagram
-   IP-adresser\
-   Porter\
-   Brannmurregler

Eksempel:

    Klient → Waitress → MariaDB

### Tjenestekonfigurasjon

-   systemctl / Supervisor\
-   Filrettigheter\
-   Miljøvariabler

------------------------------------------------------------------------

## 4. Prosjektstyring -- GitHub Projects (Kanban)

-   To Do / In Progress / Done\
-   Issues\
-   Skjermbilde (valgfritt)

Refleksjon: Hvordan hjalp Kanban arbeidet?

------------------------------------------------------------------------

## 5. Databasebeskrivelse

**Databasenavn:**

**Tabeller:**\
\| Tabell \| Felt \| Datatype \| Beskrivelse \|
\|--------\|-------\|-----------\|--------------\| \| customers \| id \|
INT \| Primærnøkkel \| \| customers \| name \| VARCHAR(255) \| Navn \|
\| customers \| address \| VARCHAR(255) \| Adresse \|

**SQL-eksempel:**

``` sql
CREATE TABLE customers (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(255),
  address VARCHAR(255)
);
```

------------------------------------------------------------------------

## 6. Programstruktur

    projectnavn/
     ├── app.py
     ├── templates/
     ├── static/
     └── .env

Databasestrøm:

    HTML → Flask → MariaDB → Flask → HTML-tabell

------------------------------------------------------------------------

## 7. Kodeforklaring

Forklar ruter og funksjoner (kort).

------------------------------------------------------------------------

## 8. Sikkerhet og pålitelighet

-   .env\
-   Miljøvariabler\
-   Parameteriserte spørringer\
-   Validering\
-   Feilhåndtering

------------------------------------------------------------------------

## 9. Feilsøking og testing

-   Typiske feil\
-   Hvordan du løste dem\
-   Testmetoder

------------------------------------------------------------------------

## 10. Konklusjon og refleksjon

-   Hva lærte du?\
-   Hva fungerte bra?\
-   Hva ville du gjort annerledes?\
-   Hva var utfordrende?

------------------------------------------------------------------------

## 11. Kildeliste

-   w3schools\
-   flask.palletsprojects.com
# Prosjekt_oppgave
