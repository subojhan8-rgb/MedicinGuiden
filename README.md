# MedicinGuiden

Gratis, statisk svensk medicinsk utbildningswebbplats med **31 diagnoser** inom kranskärlssjukdom, arytmier, retledningsrubbningar, elektrolytrubbningar, kärlsjukdom och lungsjukdom.

## Funktioner

- Sökbart och filtrerbart diagnosbibliotek på `index.html`.
- Separata, direktlänkbara diagnossidor via `diagnos.html?id=<diagnos-id>`.
- För varje diagnos: **orsak, symtom, kliniska fynd, provfynd, utredning, provtagning, EKG-fynd och behandling**.
- Syntetiska EKG-principbilder och egenritade anatomiska DT-/röntgen-/ultraljudsscheman. **Inga riktiga patientbilder.**
- **Endast fasta behandlingstabeller** (symtom, fynd, utredning, behandling). Inga interaktiva JA/NEJ-algoritmer.
- 15 diagnossidor har särskilda källanknutna behandlingsavsnitt; flertalet innehåller kontrollerade doseringsexempel. Övriga doser publiceras inte förrän de har verifierats.

## Medicinska källportaler

1. [Internetmedicin](https://www.internetmedicin.se/)
2. [Akut internmedicin – Kunskapsstöd för vårdgivare](https://kunskapsstodforvardgivare.se/omraden/akut-vard/regionala-kunskapsstod/akut-internmedicin-behandlingshandbok)
3. [Medicinakuten](https://medicinakuten.se/)

För dosuppgifter hänvisar varje relevant diagnossida även till **en specifik regional källa**. De övriga generella kliniska sammanfattningarna är inte fullständigt verifierade mot artikel för artikel. Källor kan uppdateras och doser behöver kontrolleras vid ordination.

## Start och gratis publicering

Ingen server eller databas behövs. Publicera gratis med **GitHub Pages**: repository → Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.

Efter en lyckad publicering förväntas webbplatsen finnas på:
https://subojhan8-rgb.github.io/MedicinGuiden/

Den adressen är inte verifierad som aktiv i detta dokument.

## Säkerhet och begränsningar

**Ej ett validerat kliniskt beslutsstöd.** Webbplatsen är en utbildningsprototyp och får inte ersätta patientanpassad läkarbedömning, lokala PM, specialiststöd eller läkemedelskontroll. Materialet gäller i första hand vuxna; doser kan vara olämpliga vid nedsatt njurfunktion, leversjukdom, graviditet, interaktioner eller annan kontraindikation.

EKG och bilddiagnostiska figurer är **schematiska illustrationer, inte verkliga registreringar eller diagnostiska patientundersökningar**.

Ingen patientinformation ska matas in. Allt fungerar statiskt i webbläsaren utan konto.

## Projektstruktur

- `index.html` – startsida, sökning, filter och global behandlingstabell
- `diagnoser.js` – 31 diagnosers faktakort
- `diagnos.html` – diagnossida, figurer, dosreferenser och behandlingstabell

Senaste kodrevidering: 2026-11-12.
