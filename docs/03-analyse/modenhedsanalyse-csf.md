# Modenhedsanalyse – CSF-inspireret baseline (Hvedebro)

## 1) Metode
Skala (1-5):
1. Begyndende
2. Delvis
3. Gentagende
4. Styret
5. Optimeret

Trafiklys (anvendt i slides for **nu / 12 mdr / 24 mdr**):
- 🔴 = Niveau 1 (Begyndende)
- 🟡 = Niveau 2-3 (Delvis/Gentagende)
- 🟢 = Niveau 4-5 (Styret/Optimeret)

---

## 2) Modenhed pr. område (baseline → mål)

| Område | Nu | Status nu | 12 mdr | Status 12 mdr | 24 mdr | Status 24 mdr | Kort begrundelse |
|---|---:|---|---:|---|---:|---|---|
| Governance og sikkerhedspolitik | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Ingen samlet styringsmodel i udgangspunktet |
| Risikostyring og risikoregister | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Risici håndteres, men ikke ensartet/formaliseret |
| IAM/MFA og adgangsstyring | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Uens adgangspraksis og uklar remote-adgang |
| IT/OT segmentering | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Fladt netværk og høj lateral bevægelsesrisiko |
| OT-sikkerhed og leverandøradgang | 1 | 🔴 | 2 | 🟡 | 3 | 🟡 | OT løfter sig ofte langsommere pga. drift/leverandørafhængighed |
| Backup, beredskab, restore-test | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Restore er ikke systematisk testet i udgangspunktet |
| Leverandørstyring og kontraktkrav | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Krav/SLA/revisionsret er utilstrækkeligt formaliseret |
| Logning, monitorering, detektion | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Anomalier opdages ikke robust nok i baseline |
| Awareness og adfærdsforankring | 2 | 🟡 | 3 | 🟡 | 3 | 🟡 | Kræver kontinuerlig forankring over tid |
| Cloud-/platformstyring (lokal vs cloud) | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Beslutninger tages ad hoc (fx skyggeplatforme) |

**Samlet baseline:** 1,3-1,7 (begyndende/delvis) afhængigt af vægtning  
**Mål efter 12 mdr:** ca. 2,8-2,9 (primært gul, men markant løft)  
**Mål efter 24 mdr:** ca. 3,6-3,8 (tæt på grøn samlet set)

---

## 3) CSF-funktionsview (kerneprincipper, nu → 12 mdr → 24 mdr)

| CSF-funktion | Nu | Status nu | 12 mdr | Status 12 | 24 mdr | Status 24 | Kommentar |
|---|---:|---|---:|---|---:|---|---|
| Govern | 1 | 🔴 | 3 | 🟡 | 4 | 🟢 | Ledelsesforankring og rollemodel modnes i faser |
| Identify | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Asset- og risikobillede bliver systematisk |
| Protect | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Basiskontroller bliver standardiseret |
| Detect | 1 | 🔴 | 2 | 🟡 | 3 | 🟡 | Detektion modnes gradvist via logging/use-cases |
| Respond | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Incident-processer og øvelser løfter respons |
| Recover | 2 | 🟡 | 3 | 🟡 | 4 | 🟢 | Restore-test og recovery-planer professionaliseres |

---

## 4) Hvad bruges analysen til?
- Prioritere initiativer i fase 1-4
- Dokumentere fremdrift over for ledelse og kunde
- Understøtte NIS2-retning og ISO27001-alignment
- Kalibrere realistisk ambitionsniveau (ikke over-engineering)

---

## 5) Validering i gruppen (før aflevering)
- Er niveauer og farvestatus rimelige ift. casefakta?
- Er der områder, der bør op/nedjusteres efter jeres argumentation?
- Er målniveauet (3-4) realistisk inden for 24 måneder?

## 6) Undervisningsreference (sporbarhed)
- `undervisning-slides/Noter til grundkursus i cybersikkerhed version 0.97.md`:
  - CSF-niveauer 1-5 (Begyndende → Optimeret)
  - Anbefalede modenhedsområder (processer, politik, ressourcer, leverandører, risikostyring, audit, beredskab)
- `undervisning-slides/Modul7.md`:
  - Assessment kan formidles med **Grøn/Gul/Rød**
- `undervisning-slides/Modul2.md`:
  - Modenhed bruges som indgang til realistisk politik- og risikoniveau
