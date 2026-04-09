# Eksamensoplæg: Hvedebro Maskinfabrik (Gurli-perspektiv)

Formål: Et færdigt oplæg du kan fremlægge på 10 minutter + bruge i udspørgningen.

## Slide 1 - Formål, scope og beslutning
- Formål: Løfte Hvedebro til et risikobaseret sikkerhedsniveau på 2-3 år.
- Forretningsmål: Sikre drift, beskytte udvikling/IP, bevare nøglekunder, understøtte vækst.
- Kravpres: Kunde- og supply-chain krav, NIS2/CER-relevans, stigende trusselsniveau.
- Direktionens beslutning i dag: Godkende fase 1 (0-6 måneder) og styringsmodel.

**Talepunkt (ca. 45 sek.)**  
Vi laver ikke sikkerhed for sikkerhedens skyld. Vi beskytter omsætning, leverancer og kundetillid.

---

## Slide 2 - Case-status: Hvor står Hvedebro nu
- OT-robotter har haft ekstern adgang uden stærk styring.
- Der har været konkrete hændelser: OT-nedbrud og ransomware i økonomisystem.
- Backup/restore har været utilstrækkelig og uklart placeret ansvar.
- IT/OT/administration virker delvist sammenkoblet uden tydelig segmentering.
- Shadow IT: Kundeservice/udvikling har etableret egen "server"-løsning.
- Fysisk sikkerhed er svag (indbrud, nøglestyring, lagerkontrol).
- Leverandørstyring og kontraktkrav er umodne.

**Talepunkt (ca. 1 min.)**  
Hændelserne viser, at risiciene allerede er realiseret. Vi skal stabilisere først, derefter modne.

---

## Slide 3 - Modenhedsanalyse (baseline -> mål)
Vurderingsskala: 1=Begyndende, 2=Delvis, 3=Gentagende, 4=Styret, 5=Optimeret.

| Område | Nu | 12 mdr. mål | 24 mdr. mål |
|---|---:|---:|---:|
| Governance og sikkerhedspolitik | 1 | 3 | 4 |
| Risikostyring og risk register | 1 | 3 | 4 |
| IAM, MFA og adgangsstyring | 1 | 3 | 4 |
| Netværk og segmentering (IT/OT) | 1 | 3 | 4 |
| OT-sikkerhed og leverandøradgang | 1 | 3 | 4 |
| Beredskab, backup, restore-test | 1 | 3 | 4 |
| Leverandørstyring og kontraktkrav | 1 | 3 | 4 |
| Logning, monitorering, rapportering | 2 | 3 | 4 |
| Awareness og adfærd | 2 | 3 | 4 |

**Talepunkt (ca. 1 min.)**  
Målet er ikke "perfekt sikkerhed", men kontrolleret modenhed med dokumenterbar effekt.

---

## Slide 4 - Risikoanalyse: Metode og kriterier
- Metode: Sandsynlighed (1-5) x Konsekvens (1-5) = Risikoscore.
- Farver: Grøn 1-7, Gul 8-10, Rød 11-25.
- Perspektiv: CIA (fortrolighed, integritet, tilgængelighed) + forretningspåvirkning.
- Vurdering lavet ud fra case-hændelser, organisation og kendte svagheder.

**Talepunkt (ca. 45 sek.)**  
Vi bruger en simpel model, så direktionen kan prioritere hurtigt og realistisk.

---

## Slide 5 - Top-risici (før mitigering)
| ID | Risiko | CIA-fokus | S | K | Score | Niveau |
|---|---|---|---:|---:|---:|---|
| R1 | Ukontrolleret OT-fjernadgang via leverandør | I/A | 4 | 5 | 20 | Rød |
| R2 | Manglende backup/restore test på kritiske systemer | A/I | 4 | 5 | 20 | Rød |
| R3 | Utilstrækkelig IT/OT-segmentering | I/A | 4 | 4 | 16 | Rød |
| R4 | Shadow IT (kundeservice/server/CAD) | C/I/A | 4 | 4 | 16 | Rød |
| R5 | Svag IAM/MFA og privilegerede adgange | C/I | 4 | 4 | 16 | Rød |
| R6 | Leverandørstyring uden klare sikkerhedskrav | C/I/A | 4 | 4 | 16 | Rød |
| R7 | Industrispionage/IP-tyveri i udvikling | C/I | 3 | 5 | 15 | Rød |
| R8 | Fysisk sikkerhed: nøglestyring/lageradgang | C/I/A | 3 | 4 | 12 | Rød |
| R9 | Manglende incident-proces og eskalation | I/A | 4 | 3 | 12 | Rød |
| R10 | Lav awareness/social engineering | C/I | 4 | 3 | 12 | Rød |

**Talepunkt (ca. 1 min.)**  
Hovedbudskab: Risikoeksponeringen er for høj til vækstplanen og kundekravene.

---

## Slide 6 - Initiativer (fase 1: 0-6 måneder)
- Etabler sikkerheds-governance v1.0 med RACI, mødehjul og beslutningsforum.
- Luk/hærd OT-fjernadgang: VPN med MFA, on/off-adgang, logning, godkendt change-flow.
- Stop shadow IT: central godkendelse af servere/applikationer og midlertidig konsolidering.
- Backup baseline: 3-2-1 princip, offline kopi, restore-test hver måned.
- IAM quick wins: MFA på kritiske konti, deaktiver gamle brugere, least privilege.
- Incident- og beredskabsplan (v1): roller, kontaktliste, eskalation, øvelser.
- Fysisk quick win: nøglekontrol, lageradgang, hændelseslog.

**Talepunkt (ca. 1 min.)**  
Fase 1 reducerer de røde risici hurtigt og gør virksomheden driftsrobust.

---

## Slide 7 - Initiativer (fase 2-3: 6-24 måneder)
- Segmenteret netværksarkitektur (IT/OT/DMZ) og standard for nye integrationer.
- OT-sikkerhedsprogram med asset-overblik, patch-plan og leverandørkrav (IEC62443-inspireret).
- Sikker software/udviklingsmiljø for CAD og produktdata, inkl. klassifikation.
- Leverandørstyring end-to-end: krav, kontrakter, audit-ret, exit-plan, SLA/KPI.
- NIS2-alignment: politikker, risikoproces, hændelseshåndtering, træning, kryptografi, MFA.
- Løbende awareness-program med målinger (phishing-træning, rollerettede moduler).
- KPI-rapportering til direktion månedligt, bestyrelse kvartalsvist.

**Talepunkt (ca. 1 min.)**  
Fase 2-3 flytter Hvedebro fra reaktiv drift til styrbar, dokumenterbar sikkerhed.

---

## Slide 8 - NIS2/CER kobling (praktisk)
| NIS2 minimumsområde | Hvedebro-tiltag |
|---|---|
| Risikoanalyse/politik | Governance v1->v2, årlig risikoopdatering |
| Hændelseshåndtering | Incident-proces, træning, rapportering |
| Kontinuitet/backup | BIA/BCP/DR, restore-test |
| Forsyningskæde | Leverandørkrav, due diligence, kontraktstyring |
| Sikker udvikling/vedligehold | Change/patch/sårbarhedsproces |
| Effektivitetsvurdering | KPI, audit/assessment-plan |
| Cyberhygiejne/uddannelse | Awareness-program |
| Kryptografi | Krypteringspolitik og certifikatstyring |
| Personalesikkerhed/adgang | IAM, least privilege, joiner/mover/leaver |
| MFA/sikret kommunikation | MFA på kritiske adgange, sikre fjernforbindelser |

**Talepunkt (ca. 1 min.)**  
Målet er at være NIS2-kompatibel i praksis, også når krav kommer via kunder/supply chain.

---

## Slide 9 - Governance, ansvar og ressourcer
RACI (forenklet):

| Område | R | A | C | I |
|---|---|---|---|---|
| Sikkerhedsprogram | Gurli / sikkerhedsleder | CEO (Rasmus) | COO (Poul), Kasim | Direktion/bestyrelse |
| OT-sikkerhed | Ny teknologi + OT-ansvarlig | COO | Leverandører, Preben | CEO |
| IT/IAM/backup | IT-ansvarlig funktion | Kasim | Gurli | Direktion |
| Leverandørstyring | Indkøb/kontraktansvarlig | Kasim | Juridisk/IT/OT | CEO/COO |
| Awareness | HR/ledere + sikkerhed | CEO | Linjeledelse | Alle ansatte |

Ressourcer:
- Intern kerneteam: 3-5 nøglepersoner på tværs af IT, OT, drift og ledelse.
- Ekstern støtte: målrettet OT/netværk, incident readiness og NIS2-dokumentation.
- Styregruppe: månedligt, med tydelig prioritering og risikobeslutninger.

**Talepunkt (ca. 1 min.)**  
Uden tydeligt ansvar bliver planen papir. RACI gør implementeringen reel.

---

## Slide 10 - KPI, beslutning og næste skridt
Måleparametre (månedlig):
- Antal kritiske sårbarheder > 30 dage.
- Backup-success rate + restore-test succes.
- Antal åbne højrisici i risk register.
- MFA-dækning på kritiske konti.
- Incident-detektionstid og lukketid.
- Leverandører med opdateret sikkerhedsvurdering.
- Awareness-deltagelse og phishing-resultater.

Beslutning i direktionen:
- Godkend fase 1 finansiering og mandat.
- Godkend governance og RACI.
- Godkend at leverandørkrav bliver kontraktkrav.

**Talepunkt (ca. 45 sek.)**  
Hvis vi godkender fase 1 nu, kan de mest kritiske risici reduceres markant inden for 6 måneder.

---

# Appendix A - Kort manus (10 min)
- Slide 1: 0:45
- Slide 2: 1:00
- Slide 3: 1:00
- Slide 4: 0:45
- Slide 5: 1:00
- Slide 6: 1:00
- Slide 7: 1:00
- Slide 8: 1:00
- Slide 9: 1:00
- Slide 10: 0:45

Total: 9:15 (buffer ca. 45 sek.)

# Appendix B - Typiske eksamensspørgsmål (korte svar)
1. Hvorfor starter du ikke med fuld ISO27001-certificering?  
Svar: Modenheden er for lav nu. Vi tager risikobaseret trinvist løft og bygger dokumentation, så certificering bliver realistisk senere.

2. Hvorfor er OT højere prioriteret end fx sociale medier?  
Svar: OT rammer produktion direkte og har allerede forårsaget tab. Forretningspåvirkning er størst her.

3. Er Hvedebro sikkert omfattet af NIS2?  
Svar: Ikke nødvendigvis direkte, men kundekrav og supply-chain gør NIS2-tilpasning forretningskritisk.

4. Hvad er den vigtigste quick win?  
Svar: Kontrolleret fjernadgang + MFA + backup/restore-test på kritiske systemer.

5. Hvad gør du ved leverandørrisiko?  
Svar: Krav i kontrakt, adgangsstyring, revisionsret, statusmøder og exit-plan.

6. Hvordan beviser du fremdrift?  
Svar: KPI-dashboard, risk register trend og faste ledelsesrapporter.

7. Hvad er største implementeringsrisiko?  
Svar: Manglende ledelsesforankring og uklart ansvar. Derfor styringsmodel først.

8. Hvorfor skal awareness med?  
Svar: Menneskelig adfærd er en primær angrebsflade; træning reducerer hændelser markant.

9. Hvorfor kan vi ikke "bare købe et værktøj"?  
Svar: Værktøj uden processer/ansvar reducerer ikke risiko stabilt. Governance + drift skal med.

10. Hvad accepterer du som rest-risiko?  
Svar: Lavere risici (grøn/gul) kan accepteres midlertidigt med begrundelse, ejer og revurderingsdato.

# Appendix C - Antagelser (sig dem højt hvis du bliver spurgt)
- Der er ikke fuld asset-inventarliste i casen; derfor er planen faseopdelt.
- Økonomiske estimater er på styringsniveau og kræver leverandørtilbud i fase 1.
- NIS2-mål er kompatibilitet/compliance-by-design, ikke juridisk detailfortolkning i sig selv.
