# Risikoanalyse – scoring, skabelon og risikobehandling (Hvedebro)

## 1) Valgt skabelon og metode
Vi anvender en **5x5 risikomatrix + risikoregister** med faglig reference til:
- **ISO/IEC 27005:2022** (information security risk management)
- **ISO 31000** (generel risikostyring)
- **NIST SP 800-30** (risk assessment guidance)

Kerneformel:

**Risikoscore = Sandsynlighed (1-5) × Konsekvens (1-5)**

- Sandsynlighed: 1 (meget lav) → 5 (meget høj)
- Konsekvens: 1 (ubetydelig) → 5 (katastrofal)

## 2) Zoneintervaller (trafiklys)
- **GRØN (1-7):** lav risiko
- **GUL (8-10):** mellem risiko
- **RØD (11-25):** høj risiko

---

## 3) Risikobehandling (4T)
1. **Mitigere (Reducere)** – indføre kontroller der sænker sandsynlighed/konsekvens
2. **Undgå (Avoid)** – stoppe aktivitet/løsning med uacceptabel risiko
3. **Overføre (Transfer/Share)** – flytte dele af risiko via kontrakt/forsikring/managed service
4. **Acceptere (Accept)** – bevidst acceptere rest-risiko med ejer og revurderingsdato

Beslutningsregel (udgangspunkt):
- Score 15-25: Mitigere eller Undgå
- Score 10-14: Mitigere eller Overføre
- Score 6-9: Mitigere/Overføre/Acceptere efter kontekst
- Score 1-5: Typisk Acceptere (med monitorering)

---

## 4) Risikoregister (uddrag)

> **TOP 4 (mitigeres først)** er markeret med ⭐

| Prio | ID | Risiko | S | K | Score | Zone | CIA-fokus | Behandlingsvalg | Kort beskrivelse (punktform) | Korthandling |
|---:|---|---|---:|---:|---:|---|---|---|---|---|
| 1 | R01 ⭐ | Ukontrolleret OT-fjernadgang via leverandør/hjemmeadgang | 4 | 5 | 20 | RØD | I/A | Mitigere | Høj driftsrisiko; uklar godkendelse; potentielt misbrug af adgang | Luk åben remote-adgang, brug MFA og tidsstyret adgang |
| 2 | R02 ⭐ | Manglende backup/restore-test på robotter/økonomi | 4 | 5 | 20 | RØD | A/I | Mitigere | Gendannelse er usikker; historik viser reel nedetid ved hændelser | 3-2-1 backup + månedlig restore-test |
| 3 | R03 ⭐ | Fladt IT/OT-netværk (lateral bevægelse) | 4 | 4 | 16 | RØD | C/I/A | Mitigere | Angreb kan sprede sig mellem administration og produktion | Segmentér IT/OT og etabler OT-DMZ |
| 4 | R04 ⭐ | Shadow IT (Proshop-server + gratis antivirus) | 4 | 4 | 16 | RØD | C/I/A | Undgå + Mitigere | Uautoriseret drift uden governance; høj fejl- og kompromisrisiko | Udfas shadow IT og migrér til styret platform |
| 5 | R06 | Svag IAM/MFA og privilegerede adgange | 4 | 4 | 16 | RØD | C/I | Mitigere | For brede rettigheder; manglende recertificering | MFA + least privilege + recertificering |
| 6 | R07 | Leverandørstyring uden tydelige sikkerhedskrav i kontrakter | 4 | 4 | 16 | RØD | C/I/A | Overføre + Mitigere | Tredjepart kan påvirke drift/data; uklart ansvar ved hændelser | Sikkerhedsbilag, SLA, revisionsret og exitkrav |
| 7 | R08 | IP-tyveri/industrispionage (CAD/prototyper) | 3 | 5 | 15 | RØD | C/I | Mitigere | Risiko for tab af konkurrencefordel og produktviden | Dataklassifikation + adgangsstyring + fysisk sikring |
| 8 | R11 | Ransomware mod økonomi-/administrationssystemer | 4 | 4 | 16 | RØD | I/A | Mitigere | Kan stoppe fakturering og bogføring; hændelse er set i casen | EDR, mailkontroller, segmentering, restore-øvelser |
| 9 | R05 | Uklar cloud-vs-lokal strategi for regnskab/forretningssystemer | 3 | 4 | 12 | RØD | C/I/A | Mitigere + Overføre | Beslutninger tages ad hoc; uklar ansvarsdeling mellem driftspartnere | Fast driftsmodel (cloud/lokal/hybrid) + leverandørkrav |
| 10 | R10 | Svag detektion: unormal trafik opdages ikke rettidigt | 4 | 3 | 12 | RØD | I/A | Mitigere | Angreb opdages sent; begrænset alarm- og logkapacitet | Central logning, use-cases og incident playbooks |
| 11 | R13 | AI-datalæk via uautoriserede GenAI-værktøjer | 3 | 4 | 12 | RØD | C/I | Mitigere | Fortrolige data kan lækkes via uautoriserede AI-tjenester | AI-politik, AI-register, AI-audit |
| 12 | R12 | Hjemmearbejde uden fælles sikkerhedsbaseline | 3 | 3 | 9 | GUL | C/I/A | Mitigere | Varierende sikkerhed på enheder/adgange ved skalering | Home office-standard, managed devices, VPN/MFA |
| 13 | R15 | BEC/deepfake mod ledelse og økonomi | 3 | 3 | 9 | GUL | C/I | Mitigere | Målrettet social engineering kan give økonomisk tab | Callback-procedure + 2-personers godkendelse |
| 14 | R16 | Nedetid på ikke-kritisk brochurewebsite | 2 | 2 | 4 | GRØN | A | Acceptere | Lav forretningspåvirkning og begrænset kritikalitet | Basal monitorering og planlagt servicevindue |

---

## 5) Prioriteret fokus i denne case
- **Mitigere først:** R01, R02, R03, R04
- **Næste bølge:** R06, R07, R08, R10
- **Digital fremtid:** R12, R13, R15

## 6) Governance-krav til risikoregister
- Hver risiko skal have: risikoejer, zone, CIA-fokus, behandlingstype (4T), deadline, status og rest-risiko
- Rest-risiko med *Accept* skal godkendes eksplicit af direktionen
- Re-score minimum kvartalsvist og ved større ændringer

## 7) Undervisningsreference (sporbarhed)
Denne model følger undervisningsmaterialets simple risikoskabelon:
- `undervisning-slides/Modul2.md`:
  - score = sandsynlighed × konsekvens
  - 4 behandlingsvalg: Accept, Mitigering, Overføre, Undgå
  - farvezoner: 1-7 lav, 8-10 mellem, 11-25 høj
- `undervisning-slides/Modul1.md`:
  - samme behandlingslogik omtales i assurance-kontekst
