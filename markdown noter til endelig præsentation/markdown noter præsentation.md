Hvad skal præsentationen handle om Cybersikkerhed? 

Slide 1 - Introduktion 

    Forretnings mål: Understøtte vækst, sikre udvikling, drift og bevare nøglekunder ved at opfylde compliance krav som NIS2 og ISO et eller andet. 

    Formål: Løfte digitalisering og dermed nødvendigt sikkerhedsniveau på baggrund af kendte risici og stigende trusselniveau næste 2-3 år. 

Slide 2 - Hvor står Hvedebro nu? 

Hvedebro har haft en række hændelser der dækker over forskellige områder omhandlende IT og sikkerhed: 

    Svagt IT/OT setup kan man kalde for shadow IT (OT nedbrud, Ransomware angreb og ingen kontrol, ansvar eller politik omkring hvem ejer hvad) 

    Svagt fysisk sikkerhed (indbrud, manglende nøglestyring og lagerkontrol)  

    Umodne politikker og kontrakter (supply-chain kræver NiS2 manglende generelt compliance i hele virksomheden) 

Slide 3 - Modenhedsanalyse 

Præsentation af modenhedsanalyse lavet på baggrund og inspiration fra fx NIST maturity model for at kortlægge, hvor hvedebro befinder sig på rejsen og hvilke mål giver mening at sigte efter?  
 
Levels/farver for at gøre analyse mere håndgribelig at forstå, har vi valgt at bruge to dimensioner.  
Levels (1-5) fortæller os objektivt hvor modne Hvedebro er på det gældende område. 
Farver (Trafiklys), farver fortæller os forretningsrisikoen indenfor den pågældende kategori, altså hvor stor handling der bør tages. 
 
Udefra analyse, kan vi sige at Hvedebro er meget early hvorfor hændelser også er sket. Her kan det være svært at vurdere hvor/hvad målet er og hvor man bør starte. Derfor har vi dykket mere ned i de forskellige hændelser der er sket under de forskellige områder ved brug af en risikoanalyse. 

 

 

Slide 4 – Risikoanalyse – Metode og kriterier  

Præsentation af risikoanalyse, lavet på baggrund af risikomatrix og CIA grundbegreber indenfor sikkerhed for at forstå sammenhæng mellem risiko og forretningsmæssigt konsekvens også lander på top 4 risic som der skal kigges på ligenu og her og arbejdes videre med R01, R02, R03 og R04. For at nå ønskede mål og digitalisering og nødvendigt sikkerhedsniveau. 

 

Matrix kriterier og begreber 

    Metode: 5x5-matrix og risikoregister efter ISO/IEC 27005, ISO 31000 og NIST SP 800-30. 

    Risikoscore: Sandsynlighed (1-5) x Konsekvens (1-5). 

    Risikoskala: 1-7 lav, 8-10 mellem, 11-25 høj. 

    Farvezoner: RØD (11-25), GUL (8-10), GRØN (1-7). 

    Perspektiv: CIA (fortrolighed, integritet, tilgængelighed) + forretningspåvirkning. 

    Vurdering lavet ud fra case-hændelser, organisation og kendte svagheder. 

Risikobehandling (4T): - Mitigere (Reducere) - Undgå (Avoid) - Overføre (Transfer/Share) - Acceptere (Accept) 

Beslutningsregel (udgangspunkt): - Score 15-25: Mitigere eller Undgå - Score 10-14: Mitigere eller Overføre - Score 6-9: Mitigere/Overføre/Acceptere efter kontekst - Score 1-5: Typisk Acceptere (med monitorering) 

CIA-fokus: - C = Fortrolighed, I = Integritet, A = Tilgængelighed. - Hver risiko mærkes med ét eller flere af C/I/A. - CIA bruges, så vi kan forklare præcist hvilken type skade risikoen giver, og vælge kontroller derefter. 

 

 

 

 

 

 

 

Det vi kan sige til Risikoanalyse overordnet:  

    "Vores metode er S x K med en fast rød/gul/grøn tærskel, så prioritering ikke bliver mavefornemmelse." 

    "Vi vurderer både teknisk effekt og forretningseffekt, og bruger CIA som check på hvad der rammes." 

    "Vi vælger samtidig behandlingstype pr. risiko: mitigere, undgå, overføre eller acceptere." 

Det vi kan sige til Risikoregister: 

    "Vi viser ikke kun score, men også zone (rød/gul/grøn), CIA-fokus, behandlingsvalg (4T), en kort beskrivelse og en konkret handling." 

    "Top 4 bliver mitigeret først, fordi de har størst samlet drifts- og forretningspåvirkning." 

    "CIA hjælper os med at forklare konsekvensen konkret: er det datafortrolighed, datakorrekthed eller drift der er truet." 

    "Dermed bliver planen operationel: hvem gør hvad, og hvorfor starter vi dér." 

 

Slide 5 – Intiativer og gantt chart (fase 1-4) 

Vi skal have opdateret roadmap/gantt chart så den aligner helt med virkeligheden. Fx kan vi sætte flueben ved nogle af de første mange firkanter fx har vi lavet it politik, it-sikkerhedspolitik, altså noget governance og noget forslag til ansvarsfordeling/områder bla bla. Punkter nedenunder skal der laves flere “kasser” af til roadmap og asset inventory tænker jeg skal fjernes  

 

    Godkend IT-sikkerhedspolitik v1.0 i direktionen (ejer, gyldighed, årlig revision, dispensationer). 

    Etabler roller og ansvar: RACI for direktion, IT-drift, OT, system-/dataejere og medarbejdere. 

    Luk/hærd fjernadgang: MFA, tidsbegrænset adgang, godkendelsesflow og sessionslog. 

    Implementer backup og gendannelse: 3-2-1, offline kopi og dokumenteret månedlig restore-test. 

    Kør IAM-baseline: MFA på kritiske konti, fjern gamle konti og least privilege på adminadgange og igangsætte fx Microsoft Entra ID / Azure Active directory for at få overblik og kontrol over adgang i virksomheden 

    Indfør incident/beredskab v1: kontaktliste, eskalation, roller og første tabletop-øvelse. 

    Start leverandør- og shadow-IT-styring: sikkerhedskrav i aftaler og stop for uautoriseret drift. 

    Sæt hjemmearbejdsstandard: godkendte enheder, VPN/MFA og forbud mod lokal lagring af kritiske data. 

 

Backup R02:  

 

 

 

 

Slide 6 – Ansvar og opgaver på Intiativer og faser hvem ejer hvad, hvordan og hvorfor fase 1 og 2? 

Opdateret roadmap samme layout og alting, men der står ligesom hvem tager sig af hvad og måske hvordan? Azure entra ID IAM for netop at opretholde nogle certificeringer måske NIS2 /CER, det samme med et cloud økonomi system måske et ERP som Microsoft Dynamics 365 for oogså at opretholde dansk bogføringslovgivning. Leverandør krav og compliance 

 

    Segmenteret netværksarkitektur (IT/OT/DMZ) og standard for nye integrationer. 

    OT-sikkerhedsprogram med asset-overblik, patch-plan og leverandørkrav (IEC62443-inspireret). 

    Sikker software/udviklingsmiljø for CAD og produktdata, inkl. klassifikation. 

    Leverandørstyring end-to-end: krav, kontrakter, audit-ret, exit-plan, SLA/KPI. 

    NIS2-alignment: politikker, risikoproces, hændelseshåndtering, træning, kryptografi, MFA. 

    Løbende awareness-program med målinger (phishing-træning, rollerettede moduler). 

    KPI-rapportering til direktion månedligt, bestyrelse kvartalsvist. 

 

 

 

Slide 7 – Ansvar og opgaver på Intiativer og faser hvem ejer hvad, hvordan og hvorfor fase 3 og 4? 

Opdateret roadmap samme layout og alting, men der står ligesom hvem tager sig af hvad og måske hvordan? Azure entra ID IAM for netop at opretholde nogle certificeringer måske NIS2 /CER, det samme med et cloud økonomi system måske et ERP som Microsoft Dynamics 365 for oogså at opretholde dansk bogføringslovgivning. Leverandør krav og compliance 

 

    Segmenteret netværksarkitektur (IT/OT/DMZ) og standard for nye integrationer. 

    OT-sikkerhedsprogram med asset-overblik, patch-plan og leverandørkrav (IEC62443-inspireret). 

    Sikker software/udviklingsmiljø for CAD og produktdata, inkl. klassifikation. 

    Leverandørstyring end-to-end: krav, kontrakter, audit-ret, exit-plan, SLA/KPI. 

    NIS2-alignment: politikker, risikoproces, hændelseshåndtering, træning, kryptografi, MFA. 

    Løbende awareness-program med målinger (phishing-træning, rollerettede moduler). 

    KPI-rapportering til direktion månedligt, bestyrelse kvartalsvist. 

 

 

Slide 8 – Konklusion tydeligt risiko reduktion efter 2-3 år KPI, vækst bla bla 

Måske dette skal være modul 10 fra victors slides? Altså her viser vi risiko reduktion hvis man går med ovenover nævnte roadmap og nogle KPIer og anbefaler noget logging/metrics på antal indicidents der gerne skulle falde. Her kunne det give mening at trække et katalog ind fra staten eller EU omkring risici der viser sig at være store i fremtiden / agtig nu her 2026. Jeg forestiller mig fx ai er en god del af roadmap når vi snakker fase 3 og 4. Så tideligt risiko reduktion i fase 1 og 2 ift risikoanalyse, men så skal vi også kigge ind i vækst og ai og andet fremtidssikring backup af katalog fra ekstern kilder som revisor kurt elsker 

 

 

Slide 9 – Ansvar roller og ressourcer udefra RACI Responsible, Accountable, Consulted og informed 

Interne kerne teams, styregrupper månedligt/ugentligt. Tabel der bare kort viser hvad/hvordan virksomheden bør fremadrettet bør organisere sig og sikre højt sikkerheds niveau og alle ansatte er informeret i sidste ende. 

 