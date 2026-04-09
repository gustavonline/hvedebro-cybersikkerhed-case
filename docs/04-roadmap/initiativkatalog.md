# Initiativkatalog – fra risikoregister til handling

Initiativerne er afledt af:
1) Risikoscorer i `03-analyse/risikoanalyse-score.md`  
2) Områderne IT, OT, fysisk sikkerhed, personale og governance

---

## Prioriterede initiativer

| ID | Initiativ | Primære risici | Risikobehandling | Hovedleverancer | Fase |
|---|---|---|---|---|---|
| I01 | Governance, roller og risikoproces | R07, R14 | Mitigere | RACI, risikoregister med ejere, månedligt styringsforum | F1 |
| I02 | Politikpakke (IT, OT, leverandør, hjemmearbejde, AI) | R05, R07, R12, R13 | Mitigere | Godkendte politikker + håndbog | F1-F2 |
| I03 | Asset inventory + klassifikation (IT/OT/data) | R03, R04, R08 | Mitigere | Aktivregister, kritikalitet, ejerskab | F1 |
| I04 | IT/OT-segmentering og OT-DMZ | R01, R03 | Mitigere | Zonearkitektur, firewall-regler, adgangslister | F1-F2 |
| I05 | Kontrolleret fjernadgang (PAM-light) | R01, R06 | Mitigere | VPN/jump-host, MFA, sessionslog, tidsstyring | F1-F2 |
| I06 | Backup- og restoreprogram | R02 | Mitigere | 3-2-1 backup, restore-test, recovery-runbooks | F1-F2 |
| I07 | Shadow IT-udfasning + platformstrategi (cloud/lokal) | R04, R05 | Undgå + Mitigere | Migration fra uautoriserede servere, beslutningskriterier cloud/lokal | F1-F2 |
| I08 | IAM/MFA-løft og adgangsrecertificering | R06 | Mitigere | Rollemodel, privilegiekontrol, JML-proces | F1-F2 |
| I09 | Leverandørstyring og kontraktkrav | R07 | Overføre + Mitigere | Sikkerhedsbilag, revisionsret, hændelseskrav, exitkrav | F1-F3 |
| I10 | Logning, monitorering og incident playbooks | R10, R11, R15 | Mitigere | Central logning, use-cases, eskalationsflow | F2-F3 |
| I11 | Fysisk sikkerhedsløft (ID/nøgler/lager) | R08, R09 | Mitigere | Adgangspolitik, nøgleproces, besøgslog, zonering | F1-F2 |
| I12 | Awareness- og træningsprogram (rollebaseret) | R11, R12, R15 | Mitigere | Årshjul, phishing-træning, ledertræning | F2-F4 |
| I13 | Hjemmearbejdsstandard | R12 | Mitigere | Managed devices, VPN/MFA-krav, datalagringsregler | F3 |
| I14 | AI-governance og AI-audit | R13 | Mitigere | AI-register, godkendelsesflow, kvartalsvis AI-audit | F3-F4 |
| I15 | Rest-risiko styring (accept/overførsel) | R16 + udvalgte medium-risici | Acceptere / Overføre | Register for accepterede risici med revurderingsdato | F2-F4 |

---

## Hvad prioriteres først?

### A. Første prioritet (top 4 risici)
- I04 (segmentering)
- I05 (fjernadgang)
- I06 (backup/restore)
- I07 (shadow IT + platformstrategi)

### B. Anden prioritet (stabilisering)
- I08 (IAM/MFA)
- I09 (leverandørstyring)
- I10 (detektion/incident)
- I11 (fysisk sikkerhed)

### C. Tredje prioritet (fremtidssikring)
- I12-I14 (awareness, hjemmearbejde, AI)
- I15 (styring af accepterede/overførte risici)

---

## Afhængigheder
- I04 kræver I03 (asset inventory)
- I07 kræver I01-I03 (governance, roller, overblik)
- I14 kræver I02 + I12 (AI-regler + træning)
- I15 kræver løbende opdateringer fra hele initiativporteføljen
