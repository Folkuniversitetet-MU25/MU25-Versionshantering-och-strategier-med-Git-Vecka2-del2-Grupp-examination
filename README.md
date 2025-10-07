# Grupp-examination – “Studentkatalogen” (Scrum + Git)

Denna examination tränar ert agila arbetsflöde och Git-samarbete: planera med user stories, jobba i feature branches, skapa Pull Requests (PR), göra code reviews, hantera konflikter och leverera en demo.

## Mål
- Förstå och **tillämpa** ett lättviktigt agilt flöde (stories → planering → genomförande → demo/retro).
- Samarbeta effektivt i Git/GitHub (branches, PR, review, konfliktlösning).
- Kommunicera tydligt i **issues/tickets/lappar, commits, PR:er** och README.

## Projekt 
** Studentkatalog (HTML/CSS + JS)**  
Lista studenter (namn, ålder, aktiv-status). Knapp för att lägga till en ny fördefinierad/“hårdkodad” student.

> Tips: håll tekniken enkel. Det viktiga är Git/PR/Agilt.

## Start (en person i gruppen)
1. Skapa **privat** GitHub-repo: `mu25-grupp-<X>-studentkatalog`.  
2. Lägg grundstruktur:
README.md
.gitignore
index.html
style.css
app.js   (eller src/main.ts + tsconfig.json om ni vill)
students.json (valfritt)

3. Första commit → push till `main`.  
4. Bjud in gruppmedlemmar som collaborators i Github repot.

---

## Arbetsöverenskommelse (Working Agreement) 
Skapa docs/working-agreement.md med:
- **När** ses vi? Dagar/tider.
- **Var** träffas vi? (campus/online/plats).
- **Kanaler:** Slack/Discord/e-post.
- **Svarstid:** t.ex. “vardagar 09–17, svar inom 2h”.
- **Tillgänglighet:** hur signalera frånvaro/hinder.
- **Beslutsprocess:** hur vi fattar beslut om scope/merge.
- **Konfliktpolicy:** vi tar det i team-kanalen först, eskalerar vid behov.
- **Rotation Scrum Master:** vem håller ceremonierna vilken dag.
- **Länk till Trello-brädan** (bjud in läraren med läsrätt).

---

## Roller
Dokumentera i README.md:
- **Product Owner (PO)**, **Scrum Master (SM)** (rotera gärna), **Developers**.

---

## Ceremonier & protokoll
Skapa docs/ceremonies/ med följande mallar (en fil per möte):
1. **Sprint Planning** (`planning.md`)
- Sprintmål (1–2 meningar)
- Stories valda (ID + titel + kort motivering)
- Definition of Ready (DoR) bekräftad? (Ja/Nej)
- Estimat (story points) och risker
2. **Daily standups** (`daily-YYYY-MM-DD.md`)
- Vad gjorde jag senast?
- Vad gör jag härnäst?
- Hinder?
3. **Sprint Retrospective** (`retro.md`)
- Start / Stop / Continue (1–2 punkter per rad)
- 1 konkret förbättring att prova nästa gång

> **Sprint Review** = er presentation.

---

## Bräda (Trello)
Minst dessa Kolumner: **Backlog → Selected → Doing (WIP=2) → Review → Done**
- Flytta kort **stegvis**.
- Koppla PR/issue till kort:
- **Minst:** klistra in PR/issue-URL i kortet.
- **Bättre:** aktivera **GitHub Power-Up** och “Attach” PR/issue/branch (visar status-badges).

---

## User Stories (lägg in tickets/lappar/User stories i Trello + + Acceptance Criteria (AC)
- **US1**: "Som användare vill jag se en lista med studenters **namn**, så jag får överblick."  
**AC:** Minst 3 namn visas i en lista.
- **US2**: "Som användare vill jag se **ålder** per student, så att jag vet hur gamla de är."  
**AC:** Ålder visas bredvid namn för alla poster.
- **US3**: "Som användare vill jag se om studenten är **aktiv**, så att jag snabbt ser status (grön/röd indikator)."  
**AC:** Aktiv = grön, inaktiv = röd. Färg syns på alla rader.
- **US4**: "Som användare vill jag kunna klicka på **Lägg till student** och se en ny rad i listan."  
**AC:** Knappen finns; klick lägger till en fördefinierad student och renderar den i listan.

> Skriv Acceptance Criteria som checkboxar i Trello-kortet. Exempel:
> - [ ] Minst 3 poster renderas  
> - [ ] Ålder visas för varje student  
> - [ ] Aktiv/inaktiv markeras med färg  
> - [ ] Knapp lägger till en ny post

---

## Arbetsflöde (per story)
1. `git checkout main && git pull`
2. Skapa branch: `git checkout -b feature/<kort-namn>`
3. Implementera; gör **små commits**.
4. Push → Öppna **PR** mot `main` (länka issue/ticket med `Closes #<nr>`).
5. **Minst 1 review** från gruppkompis; åtgärda och besvara feedback.
6. Merge (gärna **Squash & merge**). Stäng kort/issue → flytta till Done.

---

## PR-policy (sammanfattning)
- Små, fokuserade PR (≈ ≤ 250 rader diff).
- **Rubrik**: `type(scope): kort syfte` (ex: `feat(list): add age column`)
- **Beskrivning**: _varför_ + _hur_ + ev. bild/GIF.
- **Länk** till issue/kort.
- **Minst 1 review** krävs innan merge.

---

## Konflikter & ånger
- **Före push**: små städningar via `git commit --amend` eller `git rebase -i` OK.  
- **Efter push**: **använd `git revert`** (ändra aldrig publicerad historik).
- Skapa **minst 4** medvetena små konflikter och **dokumentera** lösningarna i PR:ens kommentar.

---

## Leverabler (IG/G – mätbara krav)
**Planering & samarbete**
- `docs/working-agreement.md` (arbetsöverenskommelse) – **obligatorisk**.
- **Trello-länk** (läraren har åtkomst).
- Ceremoniloggar i `docs/ceremonies/`:
- 1 × **planning**
- **minst 2** × **daily** (under perioden)
- 1 × **retro**

**Stories & Git**
- **Minst 4 user stories** med tydliga **AC**.
- **Minst 4 feature-branches → 4 PR → review → merge** till `main`.
- **Minst 1** dokumenterad **konfliktlösning** (i PR-kommentar).
- **PR-policy följd** (rubrik/varför/hur/länk + review).

**README**
- Syfte, hur man kör, team & roller (PO/SM/Devs), SM-rotation, “Reflektion/retro: Vad vi lärde oss”.

> **Betyg:** IG/G. Samtliga punkter ovan krävs för **G**.

---

## Presentation (10–15 min)
- Visa **brädan → issues/lappar → PR → merge → Done** (kedjan).
- Demo av appen.
- Lärdomar från **reviews/konflikter/retro**.

---

## DoD (Definition of Done)
- Kod kör lokalt utan fel.
- PR granskad & godkänd.
- README uppdaterad.
- Issue/kort länkat och **stängt vid merge**.

---

##Små tips
- Håll WIP=2 i “Doing”.
-Skriv imperativ i commits: add, fix, update.
- Hellre 4 små PR än 1 stor.
- Använd “Assignees” och “Reviewers” på PR:er.
