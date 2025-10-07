# Arbetsöverenskommelse (Working Agreement)

**Team:** <Grupp X>  
**Repo:** <länk till GitHub-repo>  
**Trello-bräda:** <länk till Trello> (⟶ läraren har läsrätt)

## 1) Tillgänglighet & kommunikation
- **Kärntider:** <ex. vardagar 09–15> (synka dagligen 15 min).
- **Kanaler:** <Slack/Discord/e-post>. Notifiera frånvaro i <kanal>.
- **Svarstid:** vardagar 09–17 – svar inom **2h**.
- **Möten:** planering mån, dagliga standups tis–tors, retro fre.

## 2) Roller
- **PO:** <namn> (kundperspektiv, prioriterar).
- **SM:** roterande (ceremonier, hindrar slöseri).  
  **Rotationstabell:**  
  | Datum | Scrum Master |
  |-------|--------------|
  | …     | …            |
- **Developers:** <namn, namn, namn>

## 3) Bräda & WIP
Kolumner: **Backlog → Selected → Doing (WIP=2) → Review → Done**  
- WIP-limit i **Doing = 2**. Flytta **stegvis**.  
- Koppla kort ↔ PR/Issues (URL + GitHub Power-Up om möjligt).

## 4) Git & PR-policy (sammanfattning)
- Branch: `feature/<kort-namn>` (en story per branch).
- Små PR (≈ ≤ 250 rader diff). **Minst 1 review** före merge.
- Titel: `type(scope): syfte` (ex: `feat(list): add age column`)
- Beskrivning: **varför** + **hur** + hur testat + **länk** till kort/issue.
- **Squash & merge** rekommenderas.

## 5) Definition of Ready (DoR)
En story är “Ready” när:
- [ ] Beskrivning enligt “Som… vill jag… så att…”
- [ ] AC (checkboxar) är tydliga och testbara
- [ ] Estimat satt (SP) och inga blockerande beroenden
- [ ] Accepterad av teamet i planering

## 6) Definition of Done (DoD)
En story är “Done” när:
- [ ] Kod kör lokalt utan fel
- [ ] PR granskad & godkänd
- [ ] README/ev. docs uppdaterad
- [ ] Kort/issue länkat och **stängt vid merge**

## 7) Beslut & konflikter
- Tekniska beslut: kort synk i standup → beslut i PR/issue-kommentar.
- Oenighet: diskutera i teamkanal → SM faciliterar → PO bryter dödläge vid behov.

_Senast uppdaterad: YYYY-MM-DD_
