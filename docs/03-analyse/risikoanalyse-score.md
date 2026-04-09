# Risikoanalyse – scoring, skabelon og risikobehandling (Hvedebro)

## 1) Valgt skabelon og metode
Vi anvender en **5x5 risikomatrix + risikoregister** med denne faglige reference:
- **ISO/IEC 27005:2022** (Information security risk management)
- **ISO 31000** (generel risikostyring)
- **NIST SP 800-30** (risk assessment guidance)

I praksis bruges en enkel ledelsesmodel:

**Risikoscore = Sandsynlighed (1-5) × Konsekvens (1-5)**

- Sandsynlighed: 1 (meget lav) → 5 (meget høj)
- Konsekvens: 1 (ubetydelig) → 5 (katastrofal)

---

## 2) Risikobehandling (4 strategier)
I stedet for kun grøn/gul/rød arbejder vi med klassiske behandlingsvalg:

1. **Mitigere (Reducere)** – indføre kontroller der sænker sandsynlighed/konsekvens
2. **Undgå (Avoid)** – stoppe aktivitet/løsning der skaber uacceptabel risiko
3. **Overføre (Transfer/Share)** – flytte dele af risiko via kontrakt, forsikring eller managed service
4. **Acceptere (Accept)** – bevidst acceptere risiko (med ejer, begrundelse og revurderingsdato)

**Praktisk beslutningsregel (udgangspunkt):**
- Score 15-25: Mitigere eller Undgå
- Score 10-14: Mitigere eller Overføre
- Score 6-9: Mitigere/Overføre/Acceptere efter kontekst
- Score 1-5: Typisk Acceptere (med monitorering)

---

## 3) Risikoregister (udvidet)

> **TOP 4 (mitigeres først)** er markeret med ⭐

| ID | Risiko | S | K | Score | Behandlingsvalg | Primær handling |
|---|---|---:|---:|---:|---|---|
| R01 ⭐ | Ukontrolleret OT-fjernadgang via leverandør/hjemmeadgang | 4 | 5 | 20 | **Mitigere** | Godkendt remote-adgang, MFA, sessionslog, tidsbegrænsning |
| R02 ⭐ | Manglende backup/restore-test på robotter, økonomi og filområder | 4 | 5 | 20 | **Mitigere** | 3-2-1 backup + faste restore-tests |
| R03 ⭐ | Fladt IT/OT-netværk (lateral bevægelse ved angreb) | 4 | 4 | 16 | **Mitigere** | Segmentering, OT-DMZ, firewall-regler |
| R04 ⭐ | Shadow IT (Proshop-server + gratis antivirus til kundeservice/CAD) | 4 | 4 | 16 | **Undgå + Mitigere** | Udfas uautoriseret drift, migrér til styret platform |
| R05 | Uklar cloud-vs-lokal strategi for regnskab/forretningssystemer | 3 | 4 | 12 | **Mitigere + Overføre** | Platformstrategi, evt. managed SaaS med sikkerhedskrav |
| R06 | Svag IAM/MFA og privilegerede adgange | 4 | 4 | 16 | **Mitigere** | MFA, least privilege, recertificering |
| R07 | Leverandørstyring uden tydelige sikkerhedskrav i kontrakter | 4 | 4 | 16 | **Overføre + Mitigere** | Sikkerhedsbilag, revisionsret, SLA, hændelseskrav |
| R08 | IP-tyveri/industrispionage (CAD/prototyper) | 3 | 5 | 15 | **Mitigere** | Dataklassifikation, adgangskontrol, DLP-light, fysisk sikring |
| R09 | Fysisk sikkerhed: nøglekontrol, lageradgang, besøgsstyring | 3 | 4 | 12 | **Mitigere** | ID/nøgleproces, zonering, logning |
| R10 | Svag detektion: unormal trafik opdages ikke rettidigt | 4 | 3 | 12 | **Mitigere** | Central logning, alarmer, incident playbooks |
| R11 | Ransomware mod økonomi-/administrationssystemer | 4 | 4 | 16 | **Mitigere** | EDR, mailkontroller, segmentering, restore-øvelser |
| R12 | Hjemmearbejde uden fælles sikkerhedsbaseline | 3 | 3 | 9 | **Mitigere** | Home office-standard, managed devices, VPN/MFA |
| R13 | AI-datalæk via uautoriserede GenAI-værktøjer | 3 | 4 | 12 | **Mitigere** | AI-politik, AI-register, AI-audit |
| R14 | Personafhængighed (få personer kan drift/sikkerhed) | 4 | 3 | 12 | **Mitigere** | Dokumentation, SOP’er, krydstræning, rollebackup |
| R15 | BEC/deepfake mod ledelse og økonomi | 3 | 3 | 9 | **Mitigere** | Awareness, callback-procedure, 2-personers godkendelse |
| R16 | Nedetid på ikke-kritisk brochurewebsite | 2 | 2 | 4 | **Acceptere** | Monitorér, lav servicevindue og basale kontroller |

---

## 4) Prioriteret fokus i denne case
- **Mitigere først:** R01, R02, R03, R04
- **Næste bølge:** R06, R07, R08, R10
- **Digital fremtid:** R12, R13, R15

---

## 5) Governance-krav til risikoregister
- Hver risiko skal have: ejer, behandlingstype (4T), deadline, status og rest-risiko
- Rest-risiko med *Accept* skal godkendes eksplicit af direktionen
- Re-score minimum kvartalsvist og ved større ændringer (ny hal, nye systemer, nye leverandører)

## 6) Undervisningsreference (sporbarhed)
Denne model følger undervisningsmaterialets simple risikoskabelon:
- `undervisning-slides/Modul2.md`:
  - **Score = sandsynlighed × konsekvens**
  - **4 behandlingsvalg:** Accept, Mitigering, Overføre, Undgå
  - **Farvezoner:** 1-7 lav, 8-10 mellem, 11-25 høj
  - **Risikoregister-felter:** risikoejer, accepteret ja/nej, nye foranstaltninger, restrisiko
- `undervisning-slides/Modul1.md`:
  - Samme 4 behandlingsvalg nævnes i assurance-kontekst (eliminere/reducere/overfør/accepter)
