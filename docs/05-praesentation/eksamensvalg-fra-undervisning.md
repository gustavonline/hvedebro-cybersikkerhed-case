# Eksamensvalg fra undervisningsmateriale (hvad giver mest mening at tage med)

Formål: koble jeres slides direkte til underviserens begreber/skabeloner, så det er tydeligt hvad I bygger på.

---

## 1) Hvad I bør prioritere i eksamensslides

## A. Modenhed (rød/gul/grøn + niveau 1-5)
**Tag med fordi:** det viser baseline, ambitionsniveau og begrunder risiko-sandsynlighed.

**Kilder i undervisning:**
- `undervisning-slides/Modul7.md` (assessment: grøn/gul/rød)
- `undervisning-slides/Noter til grundkursus i cybersikkerhed version 0.97.md` (CSF-niveau 1-5)

**Hvordan på slide:**
- Én tabel med områder + nuværende farve + mål 12/24 mdr.
- Kort tekst: “lav modenhed => højere sandsynlighed for hændelser”.

---

## B. Risikoanalyse med underviserens simple model
**Tag med fordi:** det matcher kursusmetodik direkte.

**Kilder i undervisning:**
- `undervisning-slides/Modul2.md`
  - Score = sandsynlighed × konsekvens
  - Farvezoner: 1-7, 8-10, 11-25
  - Behandling: Accept, Mitigering, Overføre, Undgå
  - Felter: risikoejer, accepteret ja/nej, restrisiko

**Hvordan på slide:**
- Vis kort “valgt skabelon” og 4 behandlingsvalg (4T)
- Vis risikoregister med flere risici, men marker Top 4 tydeligt

---

## C. NIS2 minimumskrav (praktisk oversættelse)
**Tag med fordi:** censor vil typisk spørge hvordan I omsætter lovtekst til handling.

**Kilder i undervisning:**
- `undervisning-slides/Modul3.md` (10 minimumsområder i NIS2)
- `undervisning-slides/Modul6.md` (supply chain/leverandørkrav + artikel 21)

**Hvordan på slide:**
- 5-6 bullets der viser at jeres initiativer dækker NIS2-kategorier
- Undgå juridisk overclaim: brug formuleringen “NIS2-ready retning via supply chain”

---

## D. OT + cloud/lokal + leverandørstyring
**Tag med fordi:** casen har konkrete hændelser netop her.

**Kilder i undervisning:**
- `undervisning-slides/Modul4.md` (OT: segmentering, asset mgmt, backup, IEC62443)
- `undervisning-slides/Modul6.md` (leverandøradgang, kontraktkrav, cloudovervejelser)

**Hvordan på slide:**
- Brug 1 konkret case-nær formulering: “Proshop-server/Shadow IT”, “uklar remote-OT adgang”, “cloud-vs-lokal regnskab”

---

## E. Processer og implementering
**Tag med fordi:** viser at planen kan realiseres.

**Kilder i undervisning:**
- `undervisning-slides/Modul7.md` (incident, change, patch, backup/restore, awareness, RACI)

**Hvordan på slide:**
- Knyt roadmap-initiativer til processer (ikke kun teknik)

---

## 2) Forslag til konkrete figurer/screenshots I kan indsætte

> Tip: Brug små “udklip-bokse” med tydelig kildetekst i nederste højre hjørne.

1. **Modenhedsskala 1-5** (Begyndende → Optimeret)  
   Kilde: `Noter ... version 0.97.md`

2. **Risikoskabelon-felter** (risikoejer, accepteret, restrisiko)  
   Kilde: `Modul2.md`

3. **4 risikobehandlinger (Accept/Mitigering/Overføre/Undgå)**  
   Kilde: `Modul2.md` + `Modul1.md`

4. **NIS2 minimumspunkter (politik, hændelser, backup, supply chain, MFA osv.)**  
   Kilde: `Modul3.md`

5. **Leverandørspørgsmål/checkliste**  
   Kilde: `Modul6.md`

6. **OT-principper (segmentering, asset mgmt, patch, backup)**  
   Kilde: `Modul4.md`

---

## 3) Hvad I med fordel kan skære væk i 10 min
- Lange historiske introduktioner (internet-historik, brede teori-passager)
- For mange standardnavne uden direkte casekobling
- For mange KPI’er på slides (behold få og stærke)

---

## 4) Foreslået “eksamenssprog” (kort)
- “Vi har valgt en simpel og sporbar metode fra undervisningen.”
- “Vi viser både risikoscore og risikobehandling.”
- “Vi kobler direkte fra casehændelse til initiativ og fase.”
- “Vi bruger NIS2/ISO/CER som styringsretning – ikke som overclaim om fuld certificering.”

## 5) Konkrete screenshot-idéer til jeres slides
1. **Modenhedstabel (rød/gul/grøn)** fra `docs/03-analyse/modenhedsanalyse-csf.md`
2. **Risikoregister med Top 4 markeret** fra `docs/03-analyse/risikoanalyse-score.md`
3. **4T-begreberne** (Mitigere/Undgå/Overføre/Acceptere) fra `Modul2.md` (udklip)
4. **NIS2 minimumsliste** (10 punkter) fra `Modul3.md` (udklip)
5. **Leverandørkrav-checkliste** fra `Modul6.md` (udklip)
6. **Roadmap/faseblokfigur** fra `docs/05-praesentation/hvedebro-eksamensslides.html` (slide 7)
