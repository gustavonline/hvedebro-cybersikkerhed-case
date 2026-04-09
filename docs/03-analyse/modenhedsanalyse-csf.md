# Modenhedsanalyse – CSF-inspireret baseline (Hvedebro)

## 1) Metode
Skala (1-5):
1. Begyndende
2. Delvis
3. Gentagende
4. Styret
5. Optimeret

For at gøre den let at kommunikere i slides, vises også en statusfarve:
- 🔴 = Kritisk modenhedsgab (niveau 1)
- 🟡 = Delvis modenhed (niveau 2)
- 🟢 = Styret/tilstrækkelig modenhed (niveau 3+)

---

## 2) Modenhed pr. område (baseline → mål)

| Område | Nu | Status | Mål 12 mdr. | Mål 24 mdr. | Kort begrundelse |
|---|---:|---|---:|---:|---|
| Governance og sikkerhedspolitik | 1 | 🔴 | 3 | 4 | Ingen samlet styringsmodel i udgangspunktet |
| Risikostyring og risikoregister | 2 | 🟡 | 3 | 4 | Risici håndteres, men ikke ensartet/formaliseret |
| IAM/MFA og adgangsstyring | 1 | 🔴 | 3 | 4 | Uens adgangspraksis og uklar remote-adgang |
| IT/OT segmentering | 1 | 🔴 | 3 | 4 | Fladt netværk og høj lateral bevægelsesrisiko |
| OT-sikkerhed og leverandøradgang | 1 | 🔴 | 3 | 4 | Uklare ansvars- og kontraktforhold |
| Backup, beredskab, restore-test | 2 | 🟡 | 3 | 4 | Restore er ikke systematisk testet |
| Leverandørstyring og kontraktkrav | 1 | 🔴 | 3 | 4 | Krav/SLA/revisionsret er utilstrækkeligt formaliseret |
| Logning, monitorering, detektion | 1 | 🔴 | 3 | 4 | Anomalier opdages ikke robust nok |
| Awareness og adfærdsforankring | 2 | 🟡 | 3 | 4 | Træning er ikke løbende og rollebaseret |
| Cloud-/platformstyring (lokal vs cloud) | 1 | 🔴 | 3 | 4 | Beslutninger tages ad hoc (fx skyggeplatforme) |

**Samlet baseline:** 1,3-1,7 (begyndende/delvis) afhængigt af vægtning  
**Mål:** mindst 2,8 efter 12 måneder og 3,5+ efter 24 måneder

---

## 3) CSF-funktionsview (supplerende)

| CSF-funktion | Vurdering | Kommentar |
|---|---:|---|
| Govern | 1 | Mangler formaliseret styring og ejeransvar |
| Identify | 2 | Delvist overblik over aktiver og risici |
| Protect | 2 | Basiskontroller findes, men ikke konsistente |
| Detect | 1 | Svag logning/monitorering |
| Respond | 2 | Reaktiv håndtering, begrænset playbook-praksis |
| Recover | 2 | Gendannelse muligt, men testes ikke systematisk |

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
