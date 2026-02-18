# Hvedebro Maskinfabrik – cybersikkerhedscase (kondenseret og virkelighedsnær)

*Udarbejdet som undervisnings-/studienote med fokus på at skære støj fra uden at miste de praktiske forhold i casen.*

---

## 1) Executive summary (kort version)

Hvedebro er en voksende produktionsvirksomhed med stærk forretning, men med **modenhedsgab i IT/OT-sikkerhed**. De vigtigste problemer er:

1. **Manglende governance og ejerskab** (uklar rollefordeling, beslutninger tages ad hoc).
2. **Fladt netværk mellem administration og produktion** (høj risiko for lateral bevægelse).
3. **Ukontrolleret ekstern adgang** til robotter/OT og uklare leverandøraftaler.
4. **Utilstrækkelig backup/beredskab**, dokumentation og test.
5. **Shadow IT** (uautoriserede servere/løsninger i kundeservice/udvikling).
6. **Leverandør- og supply-chain-risiko** er allerede realiseret (angreb + potentielt IP-læk).
7. **Fysiske sikkerhedshuller** (nøgler/adgang/lagerhændelser).
8. **Compliancerisiko ift. NIS2/CER og kundekrav**, hvilket direkte kan koste omsætning.

**Konklusion:** Der er behov for et **program (2-3 år)**, hvor governance, OT/IT-arkitektur, incident response, leverandørstyring og awareness bygges systematisk op. Fokus skal være både på driftssikkerhed og forretningskontinuitet.

---

## 2) Kondenseret caseforløb (uden unødig støj)

### Forretningsudvikling
- Familieejet industrivirksomhed med kraftig vækst (fra klassisk maskinfabrik til robotunderstøttet produktion).
- Nye markeder: fødevareindustri (højere krav), mulig senere forsvarsindustri.
- Omsætning vokser markant (ca. 100 mio. kr. i 2020, fortsat vækstforventning).

### Organisatoriske forhold
- Ledelsen er i praksis persondrevet (Rasmus/Poul), men roller og mandat er ikke konsekvent formaliseret.
- IT-området er historisk opbygget via relationer/familiære kontakter (fætter, venner, konsulenthus).
- Beslutninger om kritisk infrastruktur træffes ofte uden dokumenteret risikovurdering.

### Sikkerhedshændelser (reelle signaler)
- Mistænkt **IP-udslip/industrispionage** (nyt gear dukker op hos kinesisk konkurrent før markedsintroduktion).
- **Fysiske indbrud** med tyveri af relevante komponenter.
- **OT-hændelse**: 2 robotter sat ud af drift; backupansvar uklart.
- **Ransomware** mod økonomisystem; backup kun 1 uge gammel.
- Uforklarlig netværkstrafik uden for arbejdstid.

### Compliancepres
- Storkunde (ISO9000-certificeret) stiller krav om sikkerhed, politikker, risikovurderinger og NIS2-niveau i supply chain.
- Virksomheden bevæger sig fra “kan vi undgå?” til “vi bør aktivt blive klar”.

---

## 3) Hovedfund: hvor er hullerne?

## 3.1 Governance og ledelse
- Ingen samlet informationssikkerhedspolitik med tydelig godkendelse i direktion/bestyrelse.
- Uklare ejerskaber mellem CEO/COO/adm.-chef/IT-ansvarlig.
- Manglende formaliseret risikoproces, prioriteringsmodel og opfølgning.

## 3.2 IT/OT-arkitektur
- Produktion og administration er koblet tæt uden tydelig segmentering.
- Ekstern adgang til OT er etableret af tredjepart uden stærk kontrolmodel.
- Usikker fjernadgang (“blinkende kasse”, hjemmeadgang uden tydelig godkendelse).

## 3.3 Drift og robusthed
- Backupstrategi er uens og ikke dokumenteret på tværs af systemer (særligt OT).
- Mangelfuld asset inventory/CMDB (“hvad er koblet på netværket?” er uklart).
- Svag change management og utilstrækkelig logning/monitorering.

## 3.4 Mennesker og kultur
- Stor tillid, lav dokumentation.
- Kompetencer findes hos enkelte personer, men er ikke institutionaliseret.
- Awareness er sporadisk og ikke programmatisk.

## 3.5 Leverandør- og tredjepartsstyring
- Ingen tydelige kontraktkrav til sikkerhed, backup, hændelsesrapportering, revisionsret m.m.
- Leverandørintegration sker teknisk før risiko- og complianceafklaring.

## 3.6 Fysisk sikkerhed
- Nøgle- og adgangsstyring er utilstrækkelig.
- Samspillet mellem fysisk og digital sikkerhed er ikke tænkt sammen.

---

## 4) Risikobillede (prioriteret)

| # | Risiko | Sandsynlighed | Konsekvens | Samlet |
|---|---|---|---|---|
| 1 | Ransomware via flat network (IT→OT) | Høj | Kritisk | Kritisk |
| 2 | Driftstop i OT pga. manglende backup/restore | Middel-høj | Kritisk | Kritisk |
| 3 | IP-tyveri (tegninger/prototyper) | Høj | Høj | Høj |
| 4 | Leverandørkompromittering (konsulenthus/fjernadgang) | Middel-høj | Høj | Høj |
| 5 | Tab af nøglekunde pga. manglende compliance | Middel-høj | Høj | Høj |
| 6 | Datatab/forretningsafbrydelse i økonomi/salg | Middel | Høj | Høj |
| 7 | Insider- eller fejlhandling (uklare rettigheder) | Middel | Middel-høj | Høj |
| 8 | Fysisk tyveri/sabotage af kritiske komponenter | Middel | Middel-høj | Høj |
| 9 | BEC/C-level fraud/social engineering | Middel | Middel | Middel |
|10| Omdømmeskade ved hændelse uden kommunikationsberedskab | Middel | Middel-høj | Middel-høj |

---

## 5) Root cause-analyse (hvorfor sker det?)

1. **Vækst hurtigere end styring:** Organisatorisk og teknisk modenhed følger ikke med forretningen.
2. **Personafhængig IT:** Kritisk viden er bundet til få personer, dokumentation mangler.
3. **Manglende arkitekturprincipper:** Ingen tydelige principper for segmentering, adgang, logging og standardplatform.
4. **Ingen samlet sikkerhedsprogramledelse:** Initiativer er reaktive efter hændelser, ikke proaktive.
5. **Kunde- og regulatorpres kom sent på agendaen:** Compliance ses først som kundekrav, ikke som strategisk evne.

---

## 6) Forslag til styringsmodel (governance)

## 6.1 Beslutningsstruktur
Etabler et **Security Steering Committee** (månedligt):
- Deltagere: CEO (Rasmus), COO (Poul), adm.-chef (Kasim), udvikling (Preben), IT/sikkerhedsansvarlig.
- Formål: Prioritering, risikoaccept, budget, opfølgning på hændelser og compliance.

## 6.2 Roller (minimum)
- **Information Security Manager (ISM)**: Programansvar for sikkerhed/NIS2.
- **OT Security Lead**: Ansvar for PLC/robot-zoner, backup/restore, leverandøradgang.
- **IT Operations Lead**: Identitet, endpoint, servere, netværk, monitorering.
- **Data owner pr. forretningsområde**: Økonomi, salg, kundeservice, udvikling, produktion.

## 6.3 Politikker (første pakke)
1. Access control + MFA + least privilege.
2. Backup & recovery (inkl. restore-testkrav).
3. Incident response + rapportering.
4. Supplier security requirements.
5. Change management for IT/OT.
6. Data classification & håndtering af CAD/IP.
7. Fysisk adgang og nøglestyring.

---

## 7) Målarkitektur (IT/OT) – pragmatisk

1. **Netværkssegmentering i zoner**
   - Corporate IT, OT DMZ, Produktionsceller/PLC, udviklingsmiljø, gæstenet.
   - Strenge firewallregler, ingen “fri trafik” mellem IT og OT.

2. **Kontrolleret fjernadgang**
   - Kun via godkendt jump-host/VPN med MFA, sessionslogning og tidsbegrænset adgang.
   - Ingen private/”uofficielle” remote-bokse.

3. **Identitet og endpoint-sikkerhed**
   - Central identitetsstyring (fx Entra ID/AD), rollebaserede rettigheder, periodisk recertificering.
   - EDR/XDR på servere og klienter.

4. **Backup/restore-design**
   - 3-2-1-princip, immutable/offline kopier for kritiske systemer.
   - OT-konfigurationer (robot/PLC) versioneres og restore-testes kvartalsvist.

5. **Platformsanering**
   - Shadow servere udfases/migreres til styret platform.
   - CAD/IP-systemer placeres i kontrolleret udviklingszone.

6. **Monitorering og logning**
   - Central logopsamling/SIEM-light i starten.
   - Alarmer for out-of-hours aktivitet, failed logins, ny admin-konto, dataeksfiltration.

---

## 8) NIS2/CER – praktisk tolkning for Hvedebro

> **Vigtigt:** Endelig juridisk kvalifikation skal bekræftes med advokat/revisor med NIS2-erfaring.

Selv hvis Hvedebro ikke bliver direkte klassificeret som “væsentlig/vigtig enhed”, er virksomheden **de facto omfattet via kundekrav i supply chain**. Derfor bør målet være “NIS2-ready” med dokumenterbar modenhed.

### 8.1 NIS2-kapabiliteter der bør etableres
- Risikostyring og ledelsesforankring.
- Incident handling og rapporteringsflow.
- Business continuity/disaster recovery.
- Supply-chain sikkerhed.
- Secure acquisition/development/maintenance.
- Baselinekontroller: MFA, adgangsstyring, kryptering hvor relevant.
- Træning og awareness.

### 8.2 CER-perspektiv
- Fysisk robusthed, adgangskontrol, leverancesikkerhed, beredskab.
- Reelt overlap med OT/produktion, hvorfor IT- og fysisk sikkerhed skal samordnes.

---

## 9) 2-3 års plan (realistisk og prioriteret)

## Fase 0: 0-90 dage (stabilisér)
- Stop ukontrolleret fjernadgang; indfør midlertidig godkendelsesprocedure.
- Lav akut asset inventory (IT + OT + integrationspunkter).
- Gennemfør backup-verifikation på økonomi, CAD og OT-konfigurationer.
- Etabler incident response “minimum viable” playbook.
- Fjern/isolér højrisiko shadow IT (eller sæt kompensatoriske kontroller).

**Output:** Akut risikoreduktion + ledelsesoverblik.

## Fase 1: 3-9 måneder (fundament)
- Formalisér governance, roller og politikpakke.
- Segmentér netværk (mindst IT/OT-separation med firewall).
- Implementér MFA for admin, remote access og mail.
- Leverandørkontrakter opdateres med sikkerhedskrav/SLA.
- Start awareness-program (phishing, adgang, hændelsesrapportering).

**Output:** Kontrolleret basisdrift og auditspor.

## Fase 2: 9-18 måneder (modning)
- Central logning/monitorering + use cases.
- Regelmæssige restore-tests og OT-beredskabsøvelser.
- Data-/IP-beskyttelse i udviklingsmiljø (klassifikation, rettigheder, DLP-light).
- Compliance-gap-analyse mod NIS2/CER + handlingsplan.

**Output:** Forbedret modstandskraft og dokumenterbar fremdrift.

## Fase 3: 18-36 måneder (compliance og skalering)
- NIS2-ready dokumentationspakke (styring, risiko, hændelser, leverandører, test).
- Pen-test/red-team-light inkl. OT-scenarier.
- KPI-styring og årlig ledelsesreview.
- Integrer sikkerhed i nye investeringer (ny produktionshal, evt. forsvarsleverancer).

**Output:** Robust sikkerhedsdrift + konkurrencemæssig tillid hos kunder.

---

## 10) Ressourcebehov (overslagsniveau)

## Internt (minimum)
- 1 x ISM/sikkerhedsleder (kan starte som delt funktion).
- 1 x stærk IT-driftprofil (infrastruktur/identitet/endpoint).
- 0,5-1 x OT-sikkerhedsprofil (kan være kombi med automation).
- Nøglepersoner i forretningen som data/system owners (deltid).

## Eksternt
- Juridisk/compliance-rådgivning (NIS2/CER, kontraktkrav).
- Arkitektur/netværksspecialist (segmentering/OT DMZ).
- Incident response-retainer + evt. SOC/MDR-light.

---

## 11) KPI’er til direktionen (få, men stærke)

1. % kritiske aktiver med verificeret backup + seneste restore-test.
2. % remote-adgange med MFA + logning.
3. Antal højkritiske findings åbne > 30 dage.
4. MTTR ved sikkerhedshændelser.
5. Phishing resilience-rate / awareness gennemførsel.
6. Leverandører med underskrevet sikkerhedsbilag.
7. NIS2-gap closure (% lukket pr. kvartal).

---

## 12) Hvordan bør afdelingerne hænge sammen?

## Produktion (COO)
- Ejer OT-risici sammen med OT Security Lead.
- Måles på oppetid + sikker gendannelse, ikke kun output.

## Udvikling
- Ejer IP-klassifikation og sikker håndtering af CAD/prototyper.
- Samarbejder tæt med IT om adgangsstyring og datadeling.

## Kundeservice/Salg
- Må ikke drive egen infrastruktur uden governance.
- Skal have klare processer for kundespørgsmål om sikkerhed/compliance.

## Administration/Økonomi
- Ejer kritiske forretningssystemer (regnskab, HR, leverandører).
- Skal have robust BCM/DR og revisionsspor.

**Tværgående princip:** Ingen afdeling etablerer systemer alene; arkitektur- og sikkerhedsgodkendelse er obligatorisk.

---

## 13) Diskussionsafsnit – casen set fra forskellige vinkler

## A) Ledelsesperspektiv (forretning vs. sikkerhed)
- Styrke: Hurtig beslutningskraft og entreprenørånd.
- Udfordring: “Vi fikser det løbende”-kultur giver teknisk gæld og sikkerhedsgæld.
- Diskussion: Hvor meget central styring kan indføres uden at kvæle tempoet?

## B) Produktionsperspektiv (oppetid vs. kontrol)
- Styrke: Fokus på drift og output.
- Udfordring: Uformel OT-adgang og uklare leverandøransvar skaber driftsrisiko.
- Diskussion: Hvordan balanceres 24/7 drift med change windows og sikkerhedsvedligehold?

## C) Udviklings-/innovationsperspektiv (IP og time-to-market)
- Styrke: Høj innovationsgrad og nye markedsmuligheder.
- Udfordring: IP-beskyttelse er svag; designdata kan lække.
- Diskussion: Kan man accelerere innovation med *mere* sikkerhed (ikke mindre)?

## D) Medarbejder- og kulturperspektiv
- Styrke: Høj tillid og handlekraft.
- Udfordring: Personafhængighed, uklare roller og “vennetjenester” i kritiske funktioner.
- Diskussion: Hvordan professionaliseres uden at miste loyalitet og fleksibilitet?

## E) Kunde-/markedsperspektiv
- Styrke: Stærke relationer og stabil efterspørgsel.
- Udfordring: Store kunder kræver dokumenterbar sikkerhed/compliance.
- Diskussion: Sikkerhed som omkostning vs. sikkerhed som salgsargument.

## F) Angriberperspektiv (realistisk)
- Attraktive mål: CAD-filer, nye geardesigns, driftsstop i produktion, økonomisystemer.
- Angrebsveje: Fjernadgang, leverandørkæde, phishing, svage endpoints, fysisk adgang.
- Læring: Casen har allerede tegn på både cyber- og fysisk efterretning/tyveri.

---

## 14) Hvad bør urli præsentere på direktionsmødet (1. nov 2025)?

1. **Top 10 risici** med tydelig forretningspåvirkning.
2. **90-dages stabiliseringsplan** (med ansvarlige navne og datoer).
3. **2-3 års roadmap** med budgetramme i intervaller.
4. **NIS2/CER-position**: hvad er minimum, hvad er ambition.
5. **Beslutningspunkter i dag:**
   - Godkend governance-model.
   - Godkend segmenteringsprojekt IT/OT.
   - Godkend leverandør- og fjernadgangsstandard.
   - Godkend bemanding (internt + eksternt).

---

## 15) Kort konklusion

Hvedebro står ikke i en “teknisk detaljeudfordring”, men i en **forretningskritisk transformationsopgave**: fra personbåret, ad hoc sikkerhed til ledelsesforankret, dokumenterbar og driftsnær sikkerhed.

Hvis virksomheden handler nu, kan sikkerhed bruges offensivt: **højere leveringssikkerhed, stærkere kundetillid og bedre adgang til regulerede markeder**.
