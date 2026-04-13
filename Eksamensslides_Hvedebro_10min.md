# Eksamensoplæg: Hvedebro Maskinfabrik (Gurli-perspektiv)

Formål: Et færdigt oplæg du kan fremlægge på 10 minutter + bruge i udspørgningen.

## Modelkobling (direkte til jeres slideshow)
Brug denne faste sætning på hver slide: `Case-hændelse -> Model -> Beslutning/tiltag`.

| Slide | Primær model | Hvorfor den giver mening her | Billede fra modulmappe |
|---|---|---|---|
| 1 | Modulsammenhæng + case-organisering | Sætter scenen og viser hvorfor planen er nødvendig | `slide_assets/modulsammenhaeng_overblik_p3.png` eller `slide_assets/case_organisationsdiagram_p4.png` |
| 2 | Hændelsesdrevet risikobillede | Viser at risici allerede er realiseret i casen | `slide_assets/modul2_enisa_haendelser_p33.png` |
| 3 | Modenhedsmodel (1-5) | Underbygger baseline og realistisk mål | `slide_assets/modul2_modenhed_oevelse_p10.png` + `slide_assets/modul3_nist_modenhedsmodel_p35.png` |
| 4 | Risikoformel (S x K) + CIA | Gør metoden tydelig og fagligt korrekt | `slide_assets/modul2_risikoscore_model_p20.png` + `slide_assets/modul1_cia_grundbegreber_p16.png` |
| 5 | Risk register prioritering | Underbygger hvorfor netop top 10 risici er valgt | `slide_assets/modul2_cia_risikovurdering_p25.png` + `slide_assets/modul5_trusselsvurdering_p3.png` |
| 6 | Incident/BCM/DR processer | Passer til fase 1 quick wins og driftsstabilitet | `slide_assets/modul7_incident_management_p10.png` + `slide_assets/modul2_bcm_bia_bcp_dr_p32.png` |
| 7 | Leverandørstyring + OT + Awareness | Passer til 6-24 mdr. løft og supply-chain krav | `slide_assets/modul6_styring_af_aftaler_p14.png` + `slide_assets/modul4_ot_otrisiko_p31.png` + `slide_assets/modul5_awareness_human_firewall_p29.png` |
| 8 | NIS2 minimumskrav | Direkte kobling mellem krav og jeres tiltag | `slide_assets/modul3_nis2_10_minimumskrav_p14.png` + `slide_assets/modul6_leverandoer_nis2_p5.png` |
| 9 | RACI / assurance | Viser hvem der gør hvad, så planen kan eksekveres | `slide_assets/modul1_raci_oevelse_p36.png` + `slide_assets/modul7_raci_assurance_p18.png` |
| 10 | KPI/rapportering | Viser hvordan I følger op og dokumenterer effekt | `slide_assets/modul3_kpi_rapportering_p45.png` + `slide_assets/modul7_assessment_vurderingsskala_p5.png` |

Praktisk brug:
- Brug maks 1-2 modelbilleder pr. slide.
- Sig altid én konkret case-hændelse før modellen.
- Slut hver slide med beslutning: "Derfor gør vi X i fase 1/2".
- Fuld metode og fuldt register: `Risikoanalyse_Hvedebro_5x5_4T.md`.

## Slide 1 - Formål, scope og beslutning
- Formål: Løfte Hvedebro til et risikobaseret sikkerhedsniveau på 2-3 år.
- Forretningsmål: Sikre drift, beskytte udvikling/IP, bevare nøglekunder, understøtte vækst.
- Kravpres: Kunde- og supply-chain krav, NIS2/CER-relevans, stigende trusselsniveau.
- Ramme: ISO27001 bruges som styringsramme for politik, risikostyring, kontroller og løbende forbedring.
- Direktionens beslutning i dag: Godkende fase 1 (0-6 måneder) og styringsmodel.

**Talepunkt (ca. 45 sek.)**  
Vi laver ikke sikkerhed for sikkerhedens skyld. Vi beskytter omsætning, leverancer og kundetillid.

Modelnøgle:
- Model: Modulsammenhæng + case-kontekst.
- Visuelt: `slide_assets/modulsammenhaeng_overblik_p3.png` eller `slide_assets/case_organisationsdiagram_p4.png`.
![Slide 1 model](slide_assets/modulsammenhaeng_overblik_p3.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Forslag til en 2-3 års plan der minimerer risici og sikre eventuel compliance," <em>(Case, side 7)</em></li>
  <li>"Rasmus holder nu fast: Det er nu, hvor vi alligevel skal gøre en del på sikkerhedsområdet, at vi skal tage NIS2 med" <em>(Case, side 7)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vi gør ikke det her for at have pæne dokumenter, men for at beskytte drift, kunder og omsætning."</li>
  <li>"ISO27001 er vores styringsramme, og NIS2/CER er det kravpres der gør tempoet nødvendigt."</li>
  <li>"I dag beder vi om mandat til fase 1, så vi kan reducere de største risici med det samme."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser censor, at I forstår forretningsvinklen og ikke kun teknikken.</li>
  <li>Det kobler jeres plan til både standard (ISO27001) og eksterne krav (NIS2/CER).</li>
  <li>Det gør sliden beslutningsorienteret og giver en klar rød tråd til resten.</li>
</ul>
</div>

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

Modelnøgle:
- Model: Hændelsesdrevet risikobillede.
- Visuelt: `slide_assets/modul2_enisa_haendelser_p33.png`.
![Slide 2 model](slide_assets/modul2_enisa_haendelser_p33.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"de har bedt om at få en forbindelse ind til robotterne" <em>(Case, side 1)</em></li>
  <li>"3 måneder efter bliver de ramt af et ransomware angreb der krypterede bogholderisystemet." <em>(Case, side 3)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Risiciene er allerede realiseret i casen, de er ikke teoretiske."</li>
  <li>"De tre vigtigste symptomer er ukontrolleret robotadgang, ransomware i økonomi og shadow IT."</li>
  <li>"Derfor stabiliserer vi først driften og bygger derefter modenhed."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>I får etableret urgency tidligt, så senere initiativer virker nødvendige.</li>
  <li>Tre nøgleord er lette at huske under eksamenspres.</li>
  <li>Det forklarer logikken bag faseopdeling i planen.</li>
</ul>
</div>

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

Modelnøgle:
- Model: Modenhedsskala 1-5 (Begyndende -> Optimeret).
- Visuelt: `slide_assets/modul2_modenhed_oevelse_p10.png` + `slide_assets/modul3_nist_modenhedsmodel_p35.png`.
![Slide 3 model 1](slide_assets/modul2_modenhed_oevelse_p10.png)
![Slide 3 model 2](slide_assets/modul3_nist_modenhedsmodel_p35.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Holger har bedt fætter om at dokumentere hvad der er forbundet til lokalnettet, det er fætter ikke lige nået til." <em>(Case, side 2)</em></li>
  <li>"Kan det virkelig passe at der ikke skal bruges flere ressourcer på IT-sikkerhed?" <em>(Case, side 5)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vi vurderer Hvedebro til modenhed 1-2 i dag og sigter mod 3-4 over 24 måneder."</li>
  <li>"Det er et realistisk løft: fra ad hoc til styret praksis."</li>
  <li>"Målet er stabil og dokumenterbar sikkerhed, ikke en hurtig pseudo-certificering."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser proportionalitet og troværdighed i planen.</li>
  <li>Det demonstrerer, at I kan omsætte teori til en modenhedsrejse.</li>
  <li>Det beskytter jer mod kritik om at planen er for ambitiøs eller for vag.</li>
</ul>
</div>

---

## Slide 4 - Risikoanalyse: Metode og kriterier
- Metode: 5x5-matrix og risikoregister efter ISO/IEC 27005, ISO 31000 og NIST SP 800-30.
- Risikoscore: Sandsynlighed (1-5) x Konsekvens (1-5).
- Risikoskala: 1-7 lav, 8-10 mellem, 11-25 høj.
- Farvezoner: <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> (11-25), <span style="background:#fff8c5;color:#9a6700;padding:2px 8px;border-radius:999px;font-weight:600">GUL</span> (8-10), <span style="background:#dafbe1;color:#116329;padding:2px 8px;border-radius:999px;font-weight:600">GRØN</span> (1-7).
- Perspektiv: CIA (fortrolighed, integritet, tilgængelighed) + forretningspåvirkning.
- Vurdering lavet ud fra case-hændelser, organisation og kendte svagheder.

Risikobehandling (4T):
- Mitigere (Reducere)
- Undgå (Avoid)
- Overføre (Transfer/Share)
- Acceptere (Accept)

Beslutningsregel (udgangspunkt):
- Score 15-25: Mitigere eller Undgå
- Score 10-14: Mitigere eller Overføre
- Score 6-9: Mitigere/Overføre/Acceptere efter kontekst
- Score 1-5: Typisk Acceptere (med monitorering)

CIA-fokus:
- C = Fortrolighed, I = Integritet, A = Tilgængelighed.
- Hver risiko mærkes med ét eller flere af C/I/A.
- CIA bruges, så vi kan forklare præcist hvilken type skade risikoen giver, og vælge kontroller derefter.

Detaljeret scoringsgrundlag:

| Parameter | Niveau 1-2 | Niveau 3 | Niveau 4-5 |
|---|---|---|---|
| Sandsynlighed (S) | Sjælden / lav sandsynlighed | Mulig indenfor perioden | Sandsynlig / meget sandsynlig pga. tidligere hændelser eller åben sårbarhed |
| Konsekvens (K) | Begrænset drifts- og økonomipåvirkning | Mærkbar driftspåvirkning eller økonomisk tab | Kritisk driftspåvirkning, kundepåvirkning, stort tab eller compliance-effekt |

Scoringseksempler (før mitigering):

| Scenarie | S-begrundelse | K-begrundelse | Score |
|---|---|---|---:|
| OT-fjernadgang uden stram styring | Adgangen er etableret uden klar kontrol og ansvar i casen | Nedbrud i robotter har allerede givet produktionstab | 20 |
| Backup/restore-svaghed på OT | Backupansvar var uklart og ikke sikret i praksis | Produktionsstop og forsinkede leverancer rammer direkte drift/kunder | 20 |
| Ransomware i økonomi | Hændelsen er allerede indtruffet i casen | Konkrete økonomiske tab og driftsforstyrrelser i bogholderi | 16 |
| Shadow IT i kundeservice/udvikling | Egen server og CAD uden central styring øger eksponering | Risiko for datatab, kompromittering og fejl i driftskritiske data | 16 |

**Talepunkt (ca. 1:15 min.)**  
Vi bruger en simpel, men konsekvent model, så ledelsen kan prioritere transparent og dokumenterbart.

Modelnøgle:
- Model: `Sandsynlighed x Konsekvens` + CIA.
- Visuelt: `slide_assets/modul2_risikoscore_model_p20.png` + `slide_assets/modul1_cia_grundbegreber_p16.png`.
![Slide 4 model 1](slide_assets/modul2_risikoscore_model_p20.png)
![Slide 4 model 2](slide_assets/modul1_cia_grundbegreber_p16.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"det kostede lige 10.000 at få robotleverandøren på banen og nok omkring 100.000 i mistet produktion." <em>(Case, side 3)</em></li>
  <li>"Holger kommer tilbage og siger omkring 250.000 Kr." <em>(Case, side 3)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vores metode er S x K med en fast rød/gul/grøn tærskel, så prioritering ikke bliver mavefornemmelse."</li>
  <li>"Vi vurderer både teknisk effekt og forretningseffekt, og bruger CIA som check på hvad der rammes."</li>
  <li>"Vi vælger samtidig behandlingstype pr. risiko: mitigere, undgå, overføre eller acceptere."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser metodekompetence og gør analysen efterprøvbar for censor.</li>
  <li>Farverne giver hurtig prioritering (hvad haster), mens CIA forklarer skadetype (hvad rammes).</li>
  <li>Det binder teknik og forretning sammen, som lærere ofte efterspørger.</li>
  <li>Det gør overgangen til Slide 5 logisk: fra score til konkret behandlingsvalg.</li>
</ul>
</div>

---

## Slide 5 - Risikoregister (uddrag, med 4T-behandling)
| Prio | ID | Risiko | S | K | Score | Zone | CIA-fokus | Behandlingsvalg | Kort beskrivelse (punktform) | Kort handling |
|---:|---|---|---:|---:|---:|---|---|---|---|---|
| 1 | R01 ⭐ | Ukontrolleret OT-fjernadgang via leverandør/hjemmeadgang | 4 | 5 | 20 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | I/A | Mitigere | - CIA: I/A (drift + datakorrekthed) <br>- Valg: Mitigere pga. høj driftsrisiko | Luk åben remote-adgang, brug MFA og tidsstyret adgang |
| 2 | R02 ⭐ | Manglende backup/restore-test på robotter/økonomi | 4 | 5 | 20 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | A/I | Mitigere | - CIA: A/I (nedetid + datatab) <br>- Valg: Mitigere for sikker recovery | 3-2-1 backup + faste restore-tests |
| 3 | R03 ⭐ | Fladt IT/OT-netværk (lateral bevægelse) | 4 | 4 | 16 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | C/I/A | Mitigere | - CIA: C/I/A (spredning rammer bredt) <br>- Valg: Mitigere for at begrænse skadesradius | Segmenter IT/OT og etabler OT-DMZ |
| 4 | R04 ⭐ | Shadow IT (kundeservice-server/CAD) | 4 | 4 | 16 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | C/I/A | Undgå + Mitigere | - CIA: C/I/A (uautoriseret drift uden kontrol) <br>- Valg: Undgå + Mitigere for at fjerne rodårsag | Udfas shadow IT og migrer til styret platform |
| 5 | R06 | Svag IAM/MFA og privilegerede adgange | 4 | 4 | 16 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | C/I | Mitigere | - CIA: C/I (for brede rettigheder) <br>- Valg: Mitigere for at mindske misbrug | MFA + least privilege + recertificering |
| 6 | R07 | Leverandørstyring uden sikkerhedskrav i kontrakter | 4 | 4 | 16 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | C/I/A | Overføre + Mitigere | - CIA: C/I/A (tredjepart påvirker drift/data) <br>- Valg: Overføre + Mitigere via kontrakt | Sikkerhedsbilag, SLA og revisionsret |
| 8 | R08 | IP-tyveri/industrispionage (CAD/prototyper) | 3 | 5 | 15 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | C/I | Mitigere | - CIA: C/I (IP-læk + manipulerede tegninger) <br>- Valg: Mitigere for at beskytte kerne-IP | Dataklassifikation + adgangsstyring + fysisk sikring |
| 11 | R10 | Svag detektion af unormal trafik | 4 | 3 | 12 | <span style="background:#ffebe9;color:#b42318;padding:2px 8px;border-radius:999px;font-weight:600">RØD</span> | I/A | Mitigere | - CIA: I/A (angreb opdages for sent) <br>- Valg: Mitigere for hurtig respons | Central logning, alarmer og incident playbooks |
| 14 | R12 | Hjemmearbejde uden fælles sikkerhedsbaseline | 3 | 3 | 9 | <span style="background:#fff8c5;color:#9a6700;padding:2px 8px;border-radius:999px;font-weight:600">GUL</span> | C/I/A | Mitigere | - CIA: C/I/A (varierende sikkerhedsniveau) <br>- Valg: Mitigere for ensartet praksis | Home office-standard, managed devices, VPN/MFA |
| 16 | R16 | Nedetid på ikke-kritisk brochurewebsite | 2 | 2 | 4 | <span style="background:#dafbe1;color:#116329;padding:2px 8px;border-radius:999px;font-weight:600">GRØN</span> | A | Acceptere | - CIA: A (lav forretningspåvirkning) <br>- Valg: Acceptere pga. lav score | Basal monitorering og planlagt servicevindue |

Fokus:
- Mitigere først: R01, R02, R03, R04
- Næste bølge: R06, R07, R08, R10
- Fremadrettet digital risiko: R13

**Talepunkt (ca. 1 min.)**  
Hovedbudskab: Risikoeksponeringen er høj, men nu har vi både prioritering og behandlingsvalg (4T) pr. risiko.

Modelnøgle:
- Model: Prioriteret risk register.
- Visuelt: `slide_assets/modul2_cia_risikovurdering_p25.png` + `slide_assets/modul5_trusselsvurdering_p3.png`.
![Slide 5 model 1](slide_assets/modul2_cia_risikovurdering_p25.png)
![Slide 5 model 2](slide_assets/modul5_trusselsvurdering_p3.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"det viser sig så at backup ikke rigtig var noget produktionschefen havde tænkt på" <em>(Case, side 3)</em></li>
  <li>"De har selv etableret en server som de anvender" <em>(Case, side 3)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vi viser ikke kun score, men også zone (rød/gul/grøn), CIA-fokus, behandlingsvalg (4T), en kort beskrivelse og en konkret handling."</li>
  <li>"Top 4 bliver mitigeret først, fordi de har størst samlet drifts- og forretningspåvirkning."</li>
  <li>"CIA hjælper os med at forklare konsekvensen konkret: er det datafortrolighed, datakorrekthed eller drift der er truet."</li>
  <li>"Dermed bliver planen operationel: hvem gør hvad, og hvorfor starter vi dér."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det beviser, at risikoregisteret bruges til styring og ikke kun rapportering.</li>
  <li>Zone viser prioritet med det samme, og CIA gør valg af kontrol mere fagligt og mindre tilfældigt.</li>
  <li>Det kobler tallene til konkrete beslutninger, som censor kan udfordre jer på.</li>
  <li>Det gør planen klar til direktionens godkendelse.</li>
</ul>
</div>

---

## Slide 6 - Initiativer (fase 1: 0-6 måneder)
- Fase 1 prioriterer direkte de 4 højeste risici fra risikoregisteret (R01-R04).
- **R01 (OT-fjernadgang):** Luk åben remote-adgang og indfør MFA, tidsvinduer, godkendelse og sessionslog.
- **R02 (backup/restore):** Implementer 3-2-1 backup, offline kopi og dokumenteret månedlig restore-test.
- **R03 (fladt IT/OT-net):** Start segmentering med OT-DMZ og stramme firewall-regler mellem zoner.
- **R04 (shadow IT):** Stop uautoriserede løsninger og migrer kundeservice/CAD til styret platform.
- Styringsramme for at holde effekten: godkend politik v1.0, fastlæg RACI og kør incident/beredskab v1.
- Konkrete 0-6 mdr. leverancer: risikoejer pr. top-risiko, deadline, statusrapport og dokumenteret restrisiko.

**Talepunkt (ca. 1 min.)**  
Fase 1 er bygget direkte på R01-R04 og omsætter hver top-risiko til en konkret handling med målbar effekt.

Modelnøgle:
- Model: Incident + BCM/DR + procesimplementering.
- Visuelt: `slide_assets/modul7_incident_management_p10.png` + `slide_assets/modul2_bcm_bia_bcp_dr_p32.png`.
![Slide 6 model 1](slide_assets/modul7_incident_management_p10.png)
![Slide 6 model 2](slide_assets/modul2_bcm_bia_bcp_dr_p32.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Nu må du frem på banen og se at få styr på den aftale med konsulenthuset!" <em>(Case, side 3)</em></li>
  <li>"er der styr på adgangene og hvem har egentlig sagt ok til det." <em>(Case, side 6)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Slide 6 er ikke generel - den er direkte koblet til top-risici R01-R04 fra Slide 5."</li>
  <li>"R01 = fjernadgang, R02 = backup/restore, R03 = netværkssegmentering, R04 = shadow IT."</li>
  <li>"Vi viser for hver risiko: hvad vi gør, og hvilken driftsrisiko det reducerer inden for 6 måneder."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser tydelig prioriteringslogik: vi starter dér, hvor konsekvensen for drift og økonomi er størst.</li>
  <li>Det binder politik, risikomodel og handlingsplan sammen i én rød tråd, som censor efterspørger.</li>
  <li>Det gør jeres svar skarpe i udspørgningen, fordi I kan pege på en konkret risiko bag hvert tiltag.</li>
</ul>
</div>

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

Modelnøgle:
- Model: Leverandørproces + OT-sikkerhed + awareness.
- Visuelt: `slide_assets/modul6_styring_af_aftaler_p14.png` + `slide_assets/modul4_ot_otrisiko_p31.png` + `slide_assets/modul5_awareness_human_firewall_p29.png`.
![Slide 7 model 1](slide_assets/modul6_styring_af_aftaler_p14.png)
![Slide 7 model 2](slide_assets/modul4_ot_otrisiko_p31.png)
![Slide 7 model 3](slide_assets/modul5_awareness_human_firewall_p29.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Awareness skal med i planen!" <em>(Case, side 6)</em></li>
  <li>"vil lave en risikoanalyse sammen med Preben." <em>(Case, side 6)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Fase 2-3 bygger varig sikkerhed, så vi ikke kun brandslukker."</li>
  <li>"Kerneområderne er segmentering, leverandørstyring, OT-sikkerhed og awareness."</li>
  <li>"Her flytter vi os fra reaktiv drift til en styrbar sikkerhedsmodel."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser langsigtet modenhed frem for punktvise fixes.</li>
  <li>Det adresserer både tekniske, organisatoriske og menneskelige risici.</li>
  <li>Det underbygger jeres 24-måneders modenhedsmål.</li>
</ul>
</div>

---

## Slide 8 - NIS2/CER kobling (praktisk)
ISO27001-kobling:
- Vi følger ISO27001-principper i implementeringen (risikobaseret styring, kontroller, auditspor og ledelsesopfølgning).
- Målet i denne plan er ISO27001-alignment (ikke fuld certificering i fase 1).

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

Modelnøgle:
- Model: NIS2 minimumskrav mappet til konkrete kontroller.
- Visuelt: `slide_assets/modul3_nis2_10_minimumskrav_p14.png` + `slide_assets/modul6_leverandoer_nis2_p5.png`.
![Slide 8 model 1](slide_assets/modul3_nis2_10_minimumskrav_p14.png)
![Slide 8 model 2](slide_assets/modul6_leverandoer_nis2_p5.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"det skal vi så også være, ellers vil de ikke handle med os!" <em>(Case, side 5)</em></li>
  <li>"NIS2/CER, vi skal som minimum sikre at de initiativer vi tager på sikkerhedsområdet, ikke er i modstrid med NIS2/CER – men vi bør tilstræbe at blive compliant" <em>(Case, side 7)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vi designer planen, så den er NIS2/CER-kompatibel fra start."</li>
  <li>"Kundekrav og supply-chain gør compliance til et forretningskrav."</li>
  <li>"ISO27001 er vores interne styringsramme, NIS2 er den eksterne kravretning."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser regulatorisk forståelse uden at påstå fuld certificering nu.</li>
  <li>Det forklarer tydeligt hvorfor compliance er kommercielt vigtigt.</li>
  <li>Det kobler standard og lovkrav i én logisk fortælling.</li>
</ul>
</div>

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

Modelnøgle:
- Model: RACI/assurance.
- Visuelt: `slide_assets/modul1_raci_oevelse_p36.png` + `slide_assets/modul7_raci_assurance_p18.png`.
![Slide 9 model 1](slide_assets/modul1_raci_oevelse_p36.png)
![Slide 9 model 2](slide_assets/modul7_raci_assurance_p18.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Sikkerheds governance, hvad skal vi have der?" <em>(Case, side 6)</em></li>
  <li>"Hvordan skal produktion, udvikling, kundeservice og administration hænge sammen?" <em>(Case, side 7)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"RACI afklarer konkret, hvem der udfører, ejer, rådgiver og orienteres."</li>
  <li>"Vi prioriterer ansvar og beslutningsveje før nye værktøjer."</li>
  <li>"Uden tydelige ejere bliver selv gode planer ikke implementeret."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser organisatorisk modenhed, ikke kun teknisk fokus.</li>
  <li>Det reducerer implementeringsrisiko, som ofte er største årsag til fejl.</li>
  <li>Det gør jeres governance-del eksamensstærk og praktisk.</li>
</ul>
</div>

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

Modelnøgle:
- Model: KPI/KSI og løbende ledelsesrapportering.
- Visuelt: `slide_assets/modul3_kpi_rapportering_p45.png` + `slide_assets/modul7_assessment_vurderingsskala_p5.png`.
![Slide 10 model 1](slide_assets/modul3_kpi_rapportering_p45.png)
![Slide 10 model 2](slide_assets/modul7_assessment_vurderingsskala_p5.png)
<div class="case-box">
<strong>Case-understøttelse (direkte citater)</strong>
<ul>
  <li>"Nu er der snart direktionsmøde,  urli bliver bedt om at fremlægge hendes forslag." <em>(Case, side 7)</em></li>
  <li>"Der er enighed om at nu skal virksomheden op i gear på IT og sikkerhedsfronten." <em>(Case, side 7)</em></li>
</ul>
</div>
<div class="say-box">
<strong>Råd til fremlæggelse</strong>
<p><strong>Det vi siger:</strong></p>
<ul>
  <li>"Vi måler månedligt, så vi kan dokumentere om risikoen faktisk falder."</li>
  <li>"Vores vigtigste KPI'er er fx restore-test succes, lukketid på incidents og andel åbne højrisici."</li>
  <li>"Derfor anbefaler vi at fase 1 godkendes nu."</li>
</ul>
<p><strong>Hvorfor vi siger det:</strong></p>
<ul>
  <li>Det viser, at planen kan styres og evalueres objektivt.</li>
  <li>Det gør det tydeligt hvordan direktionen følger fremdrift.</li>
  <li>Det slutter præsentationen med en klar beslutningsanbefaling.</li>
</ul>
</div>

---

# Appendix A - Kort manus (10 min)
- Slide 1: 0:45
- Slide 2: 1:00
- Slide 3: 1:00
- Slide 4: 1:15
- Slide 5: 1:00
- Slide 6: 1:00
- Slide 7: 1:00
- Slide 8: 1:00
- Slide 9: 1:00
- Slide 10: 0:45

Total: 9:45 (buffer ca. 15 sek.)

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
