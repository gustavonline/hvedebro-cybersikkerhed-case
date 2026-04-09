Side 1
Cybersikkerhed
version 0.97 – august 2025
Kurt Sejr Hansen
Noter til: Grundlæggende Cybersikkerhed
Indhold
Introduktion ................................................................................................................................................ 4
Dokumentændringer ................................................................................................................................... 4
Modul 1: Grundlæggende Cybersikkerhed ................................................................................................... 5
1.1 Cybersikkerhed hvad er det? .............................................................................................................. 5
1.1.2 Uddannelse i Cybersikkerhed....................................................................................................... 5
1.1.3 Hvad må Cybersikkerhed koste .................................................................................................... 5
1.2 CIA ..................................................................................................................................................... 6
1.3 Assets ................................................................................................................................................ 7
1.4 Trusler og sårbarheder ....................................................................................................................... 7
1.5 Identity, authentication and authorization ......................................................................................... 7
1.6 Accountability, audit and compliance ................................................................................................. 9
1.7 Sikkerhedskuben ...............................................................................................................................10
1.8 Assurance program ...........................................................................................................................11
1.9 Segregation of duties ........................................................................................................................11
Modul 2: Governance og Risk......................................................................................................................12
2.1 Governance.......................................................................................................................................12
2.1.1 Modenhed..................................................................................................................................13
2.1.2 Security Governance...................................................................................................................15
2.1.3 Sikkerhedspolitikker og detaljering .............................................................................................16
2.1.4 Sikkerhedsafdelingens organisatoriske placering ........................................................................16
2.2 Risikostyring ......................................................................................................................................17
2.2 Beredskabsstyring .............................................................................................................................21
Modul 3: Compliance ..................................................................................................................................21
3.1 Lovgivning .........................................................................................................................................22
3.1.1 EU-lovgivning .............................................................................................................................22
3.1.2 NIS2 ...........................................................................................................................................23
3.1.3 GDPR ..........................................................................................................................................31
Side 2
3.1.4 GDPR og NIS2 .............................................................................................................................32
3.1.5 CER-direktivet.............................................................................................................................32
3.2 Standarder ........................................................................................................................................33
3.2.1 ISO27000 familien ......................................................................................................................33
3.2.2 NIST............................................................................................................................................34
3.2.3 CIS Security Controls...................................................................................................................37
3.2.4 Andre standarder .......................................................................................................................38
3.2.5 ISF Security Model ......................................................................................................................39
3.3 Audit .................................................................................................................................................40
3.4 Rapportering .....................................................................................................................................40
3.5 Awareness ........................................................................................................................................43
3.6 Fysisk sikkerhed ................................................................................................................................46
Modul 4 – Teknik ........................................................................................................................................49
4.1 Internet historik ................................................................................................................................49
4.1.1 IP-version 4 vs. version 6 ............................................................................................................50
4.1.2 OSI-modellen og trafik ................................................................................................................50
4.2 IP-adresse .........................................................................................................................................51
4.2.1 MAC-adresse ..............................................................................................................................52
4.1.2 Typer af IP-adresser....................................................................................................................53
4.2.3 Port nummer ..............................................................................................................................56
4.2.4 NAT ............................................................................................................................................57
4.2.5 DHCP ..........................................................................................................................................57
4.2.6 UDP/TCP ....................................................................................................................................57
4.2.7 BGP ............................................................................................................................................58
4.3 Firewall og DMZ ................................................................................................................................58
4.3.1 Et praktisk eksempel...................................................................................................................60
4.3.2 Intrusion detection .....................................................................................................................62
4.3.3 Sårbarhedsscanning og PenTest..................................................................................................63
4.4 Netværksarkitektur ...........................................................................................................................63
4.4.1 WiFi ............................................................................................................................................64
4.4.2 Øvrige netværkskomponenter ....................................................................................................66
4.5 Log Management ..............................................................................................................................68
4.6 IoT.....................................................................................................................................................70
4.7 SCADA og OT .....................................................................................................................................75
Side 3
4.8 Kryptering .........................................................................................................................................77
4.9 Cloud ................................................................................................................................................80
4.10 Zero-trust ........................................................................................................................................82
Modul 5: Internetsikkerhed ........................................................................................................................83
5.1 Trusselsbillede ..................................................................................................................................85
5.1.1 Det nationale trusselsbillede ......................................................................................................85
5.1.2 Sektor trusselsbillede .................................................................................................................86
5.2 Malware............................................................................................................................................91
5.2.1 Malware typer ............................................................................................................................91
5.2.2 Malware indgange ......................................................................................................................92
5.2.3 Malware beskyttelse ..................................................................................................................92
5.2.4 Sociale medier ............................................................................................................................94
5.3 IoC ....................................................................................................................................................95
5.4 DLP ...................................................................................................................................................95
5.5 DDOS og botnet ................................................................................................................................95
5.6 Klassifikation af sårbarheder .............................................................................................................97
5.6 Hvem passer på Danmark ..................................................................................................................98
5.6.1 National strategi for cyber og informationssikkerhed .................................................................99
5.6.2 NOST ............................................................................................................................................100
5.6.3 Cyberværnepligt .......................................................................................................................101
5.7 Hvem passer på virksomhederne.....................................................................................................101
5.8 Hvordan sikre den enkelte borger sig ..............................................................................................101
Modul 6: Leverandørstyring ......................................................................................................................103
6.1 Leverandørtyper .............................................................................................................................104
6.2 Leverandør og NIS2 krav..................................................................................................................104
6.3 Leverandørprocessen ......................................................................................................................105
6.3.1 Planlægning .................................................................................................................................107
6.3.2 Kravstilleslse .............................................................................................................................108
6.3.3 Leverandørvalg .........................................................................................................................109
6.3.4 Aftalen .....................................................................................................................................109
6.3.5 Styring ......................................................................................................................................110
6.3.6 Afslutning .................................................................................................................................110
6.4 Leverandøradgang ..........................................................................................................................111
Modul 7: Konsulentrollen og Implementering ...........................................................................................111
Side 4
7.1 Konsulentrollen ...............................................................................................................................111
7.2 Hvad er god sikkerhed? ...................................................................................................................113
7.2.1 Hvad kan konsulenten gøre i praksis .............................................................................................113
7.3 Sikkerhedsprocesser........................................................................................................................118
7.3.1 ITIL ...............................................................................................................................................119
7.4 Implementering ..............................................................................................................................120
7.4.1 Implementering af Governance ................................................................................................121
7.4.2 Personlighedstyper ...................................................................................................................122
8 Afslutning ..............................................................................................................................................124
Introduktion
Formålet md disse noter er at skabe en forståelse for grundlæggende Cybersikkerhed, forklare de
grundlæggende begreber med vægten på praktisk anvendelse. Noterne indeholder derudover emner som
forfatteren har fundet nødvendige at medtage for at kunne behandle og introducerer de grundlæggende
begreber.
Noterne skal suppleres med de slides som tilhøre det enkelte modul, slides indeholder bl.a. øvelser som
skal medvirke til en dybere forståelse.
Noter og uddybende dokumenter samt slides er tænkt som tilstrækkeligt undervisningsmateriale, det
udelukker naturligvis ikke at bøger kan anvendes som supplement. Det er derfor op til den enkelte
studerende selv at afgøre om det eksisterende materiale skal suppleres med en lærebog.
Dokumentændringer
Dato Ændring
310124 Version 0.9 klar til brug for undervisning februar 2024
270324 Version 0.91, rettet fejl og lavet lidt bedre forklaringer
190424 Version 0.92, udvidelse med CIA og enkelte rettelser
050824 Version 0.93, nyt afsnit om hvem passer på DK, virksomhederne og den enkelte borger, samt
afsnit om CIS og diverse tyrkleif. Afsnit om NIS2 opdateret med hvad der sker efteråret 2024
211024 Version 0.94, opdatering af OT-afsnit, afsnit om CER-direktivet
171224/
120125
Version 0.96, Opdatering omkring NIS2 så det stemmer med 2025 forventningerne samt
mindre generelle rettelser
010825 Version 0.97, NIS2 opdatering der nu er vedtaget, generelle mindre rettelser.
Side 5
Modul 1: Grundlæggende Cybersikkerhed
1.1 Cybersikkerhed hvad er det?
Ord bruges i flæng, nogle er mere moderne end andre og der er ofte en blandet opfattelse af hvad man
mener med begreberne, fx:
• Cybersikkerhed: Handler det så også om sikkerhed for at kunden får sine leverancer til tiden, eller
om jeg har risiko for at falde ned af stigen?
• Cybersikkerhed: Er det ikke bare noget der relaterer sig til internet?
• IT-Sikkerhed: Nå, det er jo bare IT – eller er det mere generelt?
Over tid har tingene ændret sig en del, nu anvender man oftest ”Cybersikkerhed” som et generelt begreb. I
forbindelse med regeringens strategi for ”Information og Cybersikkerhed” fra 2014, har der været en ellers
udmærket opdeling mellem Cyber og Informationsområderne, men den forskel er udvisket i 2022
strategien, som i øvrigt kan findes her.
1.1.2 Uddannelse i Cybersikkerhed
Tidligere var der ikke egentlige uddannelser i ”Sikkerhed”, der opstod derfor et parallelt univers af
certificeringer – disse findes stadig og er en glimrende måde at specialiserer sig indenfor Cybersikkerhed
eller blot få en supplering. Mange certificeringer kan kun opretholdes hvis man årligt tilegner sig viden, fx
deltager i kurser, underviser eller lign.
CISSP er en generel overordnet certificering, med bl.a. et ledelsesfokus – men også ned i detaljen, så man
reelt kan tale med dem der har detail viden. Der findes flere CISSP uddannelser, fx denne.
1.1.3 Hvad må Cybersikkerhed koste
Generelt må sikkerhed ikke koste mere end det man kan tabe ved en hændelse, det er nemt sagt – men
ofte umuligt at håndterer i praksis. Ofte tegner man en forsikring, men som vi skal se senere handler det
ofte om at reducere risici til noget der er acceptabelt – ofte koster en 100% beskyttelse for meget, eller er
helt umulig i praksis. I forbindelse med udarbejdelse af risikoanalyser, kapitel 2, tages der ofte stilling til
hvad det vil koste at reducere eller fjerne risici.
Mærsk havde en alvorlig incident i 2017, kostede knap 2 milliarder Kr., yderligere info om hvad der skete og
hvordan man håndterede, det kan findes her. Der findes mange hændelser man kan henvise til og der er
mange flere hændelser der aldrig bliver rapporteret. I forbindelse med EU kommissionens forslag, kaldet
NIS2, bliver det for en lang række virksomheder et krav at rapportere hændelser til myndighederne.
Myndighederne får også en udvidet forpligtigelse til at føre tilsyn med Cybersikkerhed samt får mulighed
for at udskrive store bøder, som det kendes fra GDPR.
Et hostingselskab, Azerocloud, blev ramt af et ransomware angreb, man betalte ikke løsepengene og det
endte med at man hjalp kunderne over til andre selskaber og lukkede selskabet.
Side 6
I situationer som Mærsk og Azerocloud, har omkostningerne været høje, men det kunne man ikke have
forudset – så selvom man var bevidst om sårbarhederne der førte til angrebene, så havde det været
vanskeligt at lave en balance mellem costs. Men det er sikkert at fx Mærsk efter hændelsen har taget en
række initiativer for at undgå at noget tilsvarende sker igen.
Meget bygger på en risikovurdering, det gælder helt fra det nationale niveau til det lille firma henne på
vejen og os selv som privatpersoner. Alle laver en form for risikoanalyse, som oftest ikke særlig godt
dokumenteret. Oftest mitigeres risici til et forsikringsselskab i bedste fald – men desværre også ved at
tænke at det rammer naboen først.
1.2 CIA
Helt centrale begreber indenfor Cybersikkerhed, anvendes i alle sammenhæng, bl.a. i forbindelse med
risikostyring, planlægning og generel vurdering af om sikkerheden er på plads og ok. Man skal kunne disse
begreber i søvne
Der findes forskellige fortolkninger, der er flere måder at sige det samme på – men generelt så handler det
```
om:
```
Illustration er hentet her, hvor der også er yderligere information.
Oftest er der mest fokus på tilgængelighed, det er også det område der er udsat for fleste incidents.
Integritet er det område man normalt har vanskelig ved at identificere og der er da også områder der falder
i mere end en kategori, fx kryptering af data – kan være med til at beskytte datastrømmen, da data ikke
umiddelbart kan læses, men også fordi en manipulation af data vil bevirke at modtageren ikke vil kunne
lave dekryptering korrekt.
Side 7
```
Eksempler:
```
Fortrolighed Integritet Tilgængelighed
Kryptering Ansvarsopdeling Backup
Adgangskontrol fysisk/logisk Kryptering/Hashing DDOS-beskyttelse
Data klassifikation Backdoor beskyttelse Recover procedure
Procedure for hvem må hvad Data/system check Dublering
Social Engineering Database procedure Persillehakker
Brugertyper Malwarebeskyttelse
EU-organisationen, der håndterer Cyberområdet – har udarbejdet et trusselskatalog, kan bl.a. bruges i
forbindelse med risikostyring, her kan ses en detaljeret opdeling af de tre begreber. Mere om dette i modul
2.
1.3 Assets
Assets er et generelt begreb som bruges i mange sammenhænge, set med sikkerhedsbriller anvendes det i
forbindelse med noget der skal beskyttes. Men asset er et helt generelt begreb, kan både være en person,
en bygning, et datasæt, en proces, et system osv.
I praksis fokuserer man ofte på cyber beskyttelse af de vigtigste assets, men det kan være en udfordring at
blive enig om hvilke assets der er de vigtigste i en virksomhed.
1.4 Trusler og sårbarheder
Det er interessant at se på trusler og sårbarheder er fordi en risikoanalyse kunne afdække hvilke trusler en
virksomhed er udsat for, hvorfor det også er interessant at se på om virksomheden har nogle sårbarheder
som kan udbyttes af truslen, forløbet mod en hændelse kan illustreres på følgende måde:
Der er mere vedr. risikoanalyse senere, men oplagt er det når en trussel er identificeret også at tænke i
hvilke sårbarheder man har, for derigennem at få et bedre overblikover hvordan man kan beskytte sig.
1.5 Identity, authentication and authorization
Et bredt område, der ikke kun dækker adgang til IT-systemer, men også kan dække fysisk adgang. Specielt
godkendelse af adgange har været i en enorm udvikling over tid. Ofte tænker man på kodeord, kravene til
Side 8
disse er kraftig stigende og behovet for mere end en ”kilde” bliver oftere og oftere et krav – det som også
```
kaldes MFA (Multi factor authentification).
```
Det kan også være adgange med særlige beføjelser, dette kan fx være ”root” adgange, adgange til at ændre
på opsætning af sikkerhed, DataBase administration-adgange og lign.
```
En forholdsvis ny teknologi er PAM (Privileged Access Manager), dette er et lidt specielt markedet – men
```
brugen af PAM’s spreder sig. Der kan læses mere om PAM mange steder, fx her.
En PAM løsning knytter sig som oftest til privilegerede adgange, men kan anvendes helt generelt.
Man siger ofte at en PAM løsning er til for at beskytte guldet i virksomheden, de mest værdifulde assets.
```
Generelt er dette område en del af sikkerhedspolitikkens IAM (Identity and Access Management) – dette
```
kommer i et senere modul.
Man skal ikke have tildelt flere privilegier i et system end det er nødvendigt for at man kan udføre sine
arbejdsopgaver, dette kaldes ”Least privileged”.
Dette er ikke fordi man har mistillid til en bruger, men også for at beskytte brugeren. Har du fx privilegier
```
(root rettighed) til mange systemer, ja så er sandsynligheden også større for at en menneskelig fejl kan
```
forsage en større hændelse. I hændelsessammenhæng, siger man som oftest at det er den menneskelige
faktor der udgør den største trussel mod en virksomhed.
Side 9
1.6 Accountability, audit and compliance
RACI-modellen er yderst velegnet til at beskrive hvem der er ansvarlig for hvad, typisk er opgaverne
fortolket således:
```
A: Den der har ansvaret for at tingene sker
```
```
R: Den der i praksis udfører opgaven
```
```
C: Den der skal spørges undervejs
```
```
I: Den der skal holdes informeret
```
RACI modellen findes i flere udgaver, og kan ofte suppleres med hvad det så egentlig betyder at være fx
”Accountable”, ofte siger man den der er ”Accountable” den der er ansvarlig fx for et system fra ”vugge til
grav”, den der er ”Responsible” er den der er udførende på et givet område, det kan så være illustreret i
billedet ovenfor som ”Task x”.Audit, del af modul 2, er orienteret mod at få opgjort om man i praksis gør
som der er aftalt, om man følger processerne, audit er en metode der kan anvendes for at sikre
compliance.
Side 10
1.7 Sikkerhedskuben
Kan synes teoretisk, men på den anden side er den også med til at man kommer vejen rundt når der tages
initiativer, men det gør det ikke nødvendigvis nemmere - man skal stadig kunne sine grundbegreber!
I Canvas ligger en Excel model med dette indhold:
Beskriv område
Område Relevans Initiativ
Præventiv, fortrolighed og fysisk
Præventiv, fortrolighed og teknisk
Præventiv, fortrolighed og administrativ
Præventiv, integritet og fysisk
Præventiv, integritet og teknisk
Præventiv, integritet og administrativ
Præventiv, tilgængelighed og fysisk
Præventiv, tilgængelighed og teknisk
Præventiv, tilgængelighed og administrativ
Detekterende, fortrolighed og fysisk
Detekterende, fortrolighed og teknisk
Detekterende, fortrolighed og administrativ
Detekterende, integritet og fysisk
Detekterende, integritet og teknisk
Detekterende, integritet og administrativ
Detekterende, tilgængelighed og fysisk
Detekterende, tilgængelighed og teknisk
Detekterende, tilgængelighed og administrativ
Korrigerende, fortrolighed og fysisk
Korrigerende, fortrolighed og teknisk
Korrigerende, fortrolighed og administrativ
Korrigerende, integritet og fysisk
Korrigerende, integritet og teknisk
Korrigerende, integritet og administrativ
Korrigerende, tilgængelighed og fysisk
Korrigerende, tilgængelighed og teknisk
Korrigerende, tilgængelighed og administrativ
Relevans, kan bruges til at fremhæve områder som de vigtigste, eller måske er et område slet ikke relevant
for den skrevne problemstilling.
Side 11
1.8 Assurance program
Sammenlignes ofte med en strategi, men også ofte kaldet et program. Et program har nogle mål og nogle
```
delmål, disse omsættes til projekter og aktiviteter, som igen sikres med ressourcer (bemanding og
```
```
økonomi)
```
En virksomhedsledelse kan sagtens igangsætte et program, uden helt at være med på hvad der reelt skal
ske, så lederen af programmet skal løbende sikre sig ledelsens medvirken og forståelse. Det betyder i
praksis han der skal være løbende adgang til ledelsen. Rapportering er en kunst!
Samtidig handler de enkelte aktiviteter og projekter om at ændre noget i organisationen, programleder skal
derfor sammen med projektledere sikre sig at der er forståelse for baggrunden for initiativerne og villighed
til at ændre noget i hverdagen, det er nok i praksis den største udfordring. Det er som udgangspunkt
ALDRIG nok at direktøren siger at det SKAL vi!
Nærmere under dette i forbindelse med modulet der omhandler ”Implementering”
1.9 Segregation of duties
Sikring af at ikke en sidder på hele processen, men at der er en funktionsadskillelse som bl.a. sikrer mod
misbrug, det kan opfattes negativt – men det er også for at sikre den enkelte medarbejder, fx at man
kommer til at lave en fejl som får store konsekvenser og som ikke kan rettes før det er for sent.
Funktionsadskillelse kan sikre i mange forskellige områder, her skal nævnes et par eksempler:
Brugeradministration
En bruger ønsker adgang til et bestemt system, sender anmodningen til sin chef, der godkender og sender
den videre til en brugeradministrativ funktion som laver en registrering og sender beskeden videre til den
administrator der kan udføre opgaven i praksis. Sender svar retur og den brugeradministrative funktion
sender besked til brugeren med kopi til chefen.
Indkøb og fakturering
En medarbejder anmoder om et bestemt køb, opretter bestillingen i indkøbssystemet. Systemet sender en
godkendelsesanmodning til fx medarbejderens chef som skal redegøre for kontostrengen. Ved ok, sender
indkøbssystemet bestillingen videre til leverandøren. Leverandøren sender varen til medarbejderen, der
kvitterer for modtagelsen, leverandøren sender faktura og indkøbssystemet sender faktura videre til
godkendelse og slutteligt sikre betaling under visse forudsætninger
Side 12
Modul 2: Governance og Risk
Aktiviteter indenfor Cybersikkerhed opdeles typisk i tre hovedområder:
• Governance
• Risk
• Compliance
De to første områder behandles i dette modul, compliance i modul 3.
2.1 Governance
Governance bruges i mange sammenhænge i virksomheder og organisationer, der findes regler fx indenfor
økonomi, jura, HR og kommunikation som regulerer hvad den enkelt må og ikke må i en virksomhed. Dette
kaldes også governance.
Hvad er governance helt generelt?
Der findes ikke en egentlig definition af governance, men hvis vi alligevel skal forsøge os med en, må det
være noget i denne retning:
Governance er et system af processer, regler og retningslinjer, som en organisation kontrolleres og opererer
med. Etik, risikostyring, compliance og administration er alle elementer, der er omfattet af governance.
Det handler først og fremmest om struktur og processer for beslutningstagning, ansvarlighed, kontrol og
adfærd. Derudover er det et spørgsmål om at sikre, at alle i organisationen følger passende og transparente
processer, samt at alle interessenters interesser varetages/beskyttes. Der skal være åbenhed og styr på
sagerne!
```
Governance kan også ses som et sæt relationer mellem forskellige interessenter (ledelsen, bestyrelsen,
```
```
aktionærerne, medarbejdere etc.), og god governance opsætter tydelige roller og ansvar i organisationen.
```
For eksempel hvad kan man, som IT medarbejder og hvad skal man som bestyrelsesmedlem.
Governance har blandt andet indflydelse på:
• Hvordan organisationens mål sættes og nås
• Hvordan risici overvåges og håndteres
• Hvordan performance optimeres
Det er desuden vigtigt, at governance ses som et system og en løbende proces – ikke en enkelt aktivitet. En
vellykket governance strategi kræver derfor en systematisk tilgang til de regler, praksis og processer,
organisationen styres efter, så man sikrer, at de mekanismer, der driver organisationen, er velbygget og
løbende kan tilpasse og ændre sig, efterhånden som forskellige muligheder og/eller udfordringer/trusler
opstår.
I denne forbindelse er det valgt at ordet ”Governance” dækker over:
• Sikkerhedspolitik
```
• Overblik over hvem gør hvad hvornår (traditionelt anvendes ordet Governance på dette område)
```
Side 13
I ret mange tilfælde er en sikkerhedspolitik noget man bare skal have, men i realiteten burde en
sikkerhedspolitik være noget som var forankret i disse begreber:
• Skal være relevant for forretningen – kunderne
• Skal tage højde for virksomhedens risici
• Skal efterleve lovgivningen
• Skal, måske, efterleve standarder
• Skal tilpasses virksomhedens modenhedsniveau
En sikkerhedspolitik skal nødig være noget der udelukkende laves fordi man skal af hensyn til revision eller i
forbindelse med markedsføring, men det sker desværre ofte. Det er heller ikke et dokument som man
googler sig til, jo som inspiration måske.
Men man skal have et udgangspunkt, så en indledende sikkerhedspolitik kan sagtens være simpel og så
alligevel tage hensyn til hvor virksomheden er i trusselslandskabet og overfor sine kunder.
SANS har udgivet en række politikker på forskellige områder, disse kan findes her. En udmærket dansk
skabelon kan findes her.
Generelt er der mange vejledninger omkring specifikke emner – delpolitikker, se bl.a. hos ”Sikkerdigital”
her.
I forbindelse med analyse af en virksomhed er det interessant at se hvor virksomheden er omkring sin
sikkerhedspolitik, man kunne fx spørge:
• Hvor gammel er politikken
• Hvornår er den sidst revideret og hvorfor
• Hvor mange kender den
Svarene siger en hel del om virksomheden, herunder virksomhedens modenhedsniveau.
2.1.1 Modenhed
Skal man lave en sikkerhedspolitik fra grunden, vil det som oftest være en ide at have et oplæg og så bruge
dette i forbindelse med en dialog med forretningen og ledelsen. En internetsøgning kan være en god hjælp,
man behøver ikke at starte med et blankt papir.
Det kan tænkes at en ledelse gerne vil efterleve en standard, igen der er nogen der har tænkt på fx hvad
god sikkerhed er – indenfor EU er det som oftest ISO27000 familien af standarder der anvendes, mere om
disse i modul 3. Men disse standarder kan også bruges indledningsvis, så en ledelse får et overordnet
indblik i hvad en standard indeholder. Det skal understreges at man som oftest udvælger de dele af en
standard der giver mest mening for den aktuelle virksomhed – i den forbindelse kan man starte med at se
på virksomhedens modenhedsniveau. Også på dette område er der hjælp at hente, som eksempel herpå
kan denne eventuelt anvendes. Man kan også selv lave sin egen skala fx anvende disse vurderingspunkter:
• Processer omkring informationssikkerhed
• Politik for informationssikkerhed
• Ressourcer, kompetencer og bevidsthed
• Leverandørstyring
• Risikostyring
• Måling, audit og evaluering
• Beredskabsplaner
Side 14
Man skal naturligvis lige være klar over, hvad man mener med de enkelte områder, hvad der er relevant og
hvilken skala man anvender. Om fokus er på Cybersikkerhed, eller om det er mere bredt, er også relevant.
At se på modenhedsniveauet fra en start, bør kunne sikre at man hverken skyder over eller under målet i
formuleringen af en sikkerhedspolitik.
```
Modenhedsniveauer i CSF-standarden (Cybersecurity Framework)
```
```
Modenheden (eller paratheden) findes ved at besvare en række udvalgte spørgsmål fra CSF-standarden og
```
kommer til udtryk med en værdi, som beskriver modenhedsniveauet i organisationen, fx omkring
```
risikostyring:
```
Modenhed 1: Begyndende
Organisationen har ingen eller få risikohåndterings-processer og arbejder meget lidt med cyber- og
informationssikkerhed.
Modenhed 2: Delvis
Organisationens risikohåndterings-processer inden for informationssikkerhed er ikke formaliserede, og
risiko håndteres ad hoc.
Modenhed 3: Gentagende
Der er etableret en metode til risikohåndtering, som er udbredt i organisationen og godkendt af ledelsen,
men ikke er forankret gennem dækkende politikker.
Modenhed 4: Styret
Organisationens risikohåndtering er ledelsesgodkendt og forankret gennem dækkende politikker. Praksis
opdateres regelmæssigt på baggrund af ændringer i forretningskrav og -miljø.
Modenhed 5: Optimeret
Organisationen optimerer løbende implementerede processer eller godkendte politiker på baggrund af
aktiviteter og erfaringer. Gennem en vedvarende forbedringsproces tilpasser organisationen sig aktivt til
ændringer i trussels- og teknologilandskabet.
Det samlede modenhedsniveau for en organisation er med til at definere sårbarhedsniveauet. Det betyder
konkret, at jo lavere en organisations modenhed inden for Cybersikkerhed er, jo højere er sandsynligheden
for, at risici indtræffer.
Uanset hvilken model man anvender, så er det en god indgangsvinkel til at få bevidsthed sammen med
ledelsen, om hvor moden virksomheden er indenfor Cybersikkerhed. Det vil ofte være grobund for at
komme op på et højere modenhedsniveau.
Som nævnt er der flere gode modeller der dels beskriver modenheden, men også kommer med forslag til
next-step. Blandt disse er denne fra ICO, en uafhængig Engelsk organisation. Modellen kan anbefales. Da
den udover at give en assessment også giver forslag til forbedringer. Det kan synes som en større opgave,
men vigtigt er det så at udvælge de områder der er mest relevant for virksomheden. Som tidligere omtakt
kan man bl.a. se på de vigtigste assets først.
Side 15
Uanset hvilket model man anvender, så kræver det et kendskab til virksomheden, alternativt at man
opstiller nogle forudsætninger og er sig disse bevidst.
2.1.2 Security Governance
Hvem har ansvaret for hvad omkring informations og Cybersikkerhed i en virksomhed, er ofte noget der
kræver en del implementeringsarbejde. Man i en organisation tænker som oftest at ansvaret for
Cybersikkerhed ligger i sikkerhedsafdelingen, det er en helt forkert opfattelse – den enkelte afdeling og den
enkelte medarbejder har ansvaret på området, sikkerhed skal være bygget ind i de daglige forretningsgange
og ikke bare være noget man tager frem ved festlige lejligheder!
Sikkerhedsafdelingen har ansvaret for at politikker og standarder er på plads og at disse afspejler
trusselsbillede og virksomhedens modenhedsniveau.
Til det mere praktiske:
En typisk governance definere følgende ansvar og rolle
Organisation Rolle og ansvar
Bestyrelsen Skal fastlægge og godkende det overordnede sikkerhedsniveau
Direktionen Overordnede ansvar for at det fastlagte sikkerhedsniveau
efterleves, direktion er ansvarlig for:
• Godkende sikkergedspolitikker og governance
• Sikre en effektiv sikkerhedsorganisation
• Fastlægge risikoappetit
• Godkende overordnede sikkerhedsinitiativer
• Godkende årlig rapportering, inden den fremlægges for
bestyrelsen
Sikkerhedsansvarlige Består at linjeledelsens sikkerhedsansvarlige og er ansvarlig for:
• Godkende tværorganisatoriske initiativer
• Godkende årligrapportering inden aflevering ti direktion
• Godkende risikoanalyser
• Godkende politikker, governance og standarder inden de
sendes til formel godkendelse i direktionen
• Godkende sikkerhedsinitiativer
Sikkerhedsorganisation Ansvarlig for:
• Udarbejdelse af sikkerheds risikoanalyser
• Udarbejde sikkerhedspolitikker, governance og standarder
• Assistere og rådgive linjeledelsen
• Udføre sikkerhedsaudit og penetration tests
• Løbende udarbejde relevant sikkerhedsrapportering
• Overvåge virksomhedens trusselsniveau
• Awareness
Linjeledelse Har ansvaret for
• Sikre viden på sikkerhedsområdet er kommunikeret til
relevante medarbejdere
• Implementering af politikker og standarder, sikre
indbygning i de daglige processer
• Beredskabsstyring
Side 16
• Udføre/Deltage i risikoanalyser
• Rapportering af status på sikkerhedsinitiativer til
Sikkerhedsorganisationen
• Incident management
Den enkelte medarbejder Har svaret for:
• Overholdelse af sikkerhedsprocedure og standarder
• Kendskab til sikkerhedspolitikker
• Løbende rapportering af sikkerhedshændelser i henhold til
procedure
• Deltage i Awareness kampagner
Governance kaldes også i flere sammenhænge ”Code of Conduct”
2.1.3 Sikkerhedspolitikker og detaljering
Hvor detaljeret skal en sikkerhedspolitik være, hvor meget skal en central sikkerhedsorganisation overlade
til de enkelte afdelinger? – det er spørgsmål som må stilles inden politikkerne udarbejdes. Igen vil det typisk
hænge sammen med virksomhedens modenhedsniveau. Det er fristende for den centrale
sikkerhedsorganisation at gå i dybden og detaljere politikkerne, men det indebærer den risiko at den
centrale sikkerhedsorganisation gør sig klog på noget som måske er umuligt, eller man kunne opnå den
tilsvarende eller bedre sikkerhed på anden vis.
Det betyder at detaljeringsniveauet bl.a. afhænger af hvad der er af decentrale ressourcer på området.
Uanset hvad så bør den centrale sikkerhedsorganisation samarbejde med de decentrale afdelinger omkring
udarbejdelse af politikker og være meget lyttende for hvad der fortælles decentralt. Så er der naturligvis en
basline som ikke kan overskrides: National lovgivning og dermed compliance mod bl.a. bekendtgørelser.
Men det tjener ikke noget formål hvis den centrale sikkerhedsorganisation blot laver politikker som ingen i
organisationen forholder sig til, så er det blot papir og noget som kun kan tages frem ved festlige
lejligheder.
2.1.4 Sikkerhedsafdelingens organisatoriske placering
Mindre virksomheder har typisk ikke en sikkerhedsafdeling, de mindre der har ser som oftest sikkerhed
som en del af en IT-afdeling, en IT-afdeling kan typisk også findes i sammenhæng med en finansafdeling.
Men hvor bør en sikkerhedsafdeling organisatorisk placeres? – det findes der ikke en entydig forklaring på,
der er da også meget store forskelle. Sikkerhedsafdelingen kan være helt uafhængig og knyttet til
bestyrelsen – dette ses fx i finansindustrien. Sikkerhedsafdelingen kan være placeret dybt nede i
organisationen, dette er som oftest tilfældet for de virksomheder der endnu ikke har oplevet
sikkerhedshændelser af betydning. Der er meget normalt at en sikkerhedsafdeling får mest fokus når der
har været en hændelse og virksomheden har set værdien af øget sikkerhed.
Afgørende for placeringen er:
• At sikkerhedsafdelingen har kontakt til forretningen
• At sikkerhedsafdelingen har adgang til et senior ledelsesniveau
• At sikkerhedsafdelingen formår at samarbejde generelt i virksomheden, ikke bare sige nej
Side 17
I større virksomheder kan en sikkerhedsafdeling være opdelt i en operativ afdeling og så en mere
governance/strategisk orienteret afdeling. Er dette tilfældet, så er den organisatoriske placering naturligvis
forskellig.
Så der findes ikke en klar anbefaling, men de tre punkter ovenfor er vigtige for enhver sikkerhedsafdeling.
2.2 Risikostyring
Risikostyring er et helt generelt begreb, der fx også bruges i projektstyring.
Risikostyring kan være meget simpelt og kan være overordentlig teoretisk, den teoretiske indfaldsvinkel er
ofte brugt og resultere som oftest i at risici bliver illustreret og ikke håndteret i praksis – det bliver for
komplekst for en ledelse at forstå det. Men derfor kan den akademiske tilgang være udmærket, kunsten er
så at få det illustreret på en måde som kan forstås af ledelse så der kan handles!
Der tales ofte om forskellige former for risikostyrings:
• Financiel risikostyring
• Operationel risikostyring
• Projekt risikostyring
• Miljø risikostyring
• Sikkerheds risikostyring
• Mv.
Som oftest handler det om at reducere risici til noget acceptabelt:
I slides er der gennemgået to modeller, en simpel og ENISA modellen. Disse skal ikke yderligere beskrives
her, men specielt omkring ENISA er der meget udmærket materiale at finde her.
Side 18
En vigtig måde at kommunikere effekten af risikostyring, er at estimere hvordan risikoen ændre sig via et
initiativ, et eksempel kunne være at indføre et system til brugeradministration, et system der fx vil lukke
brugeradgange, så snart en medarbejder forlader virksomheden. Man har måske identificeret at man har
haft åbne brugeradgange, selvom medarbejderne har forladt virksomheden for længe siden.
Det kan måske fremmeforståelse for at det fx kostede 250 Kr. at anskaffe et nyt brugeradministrativt
system.
I markedet findes der en lang række software modeller der kan hjælpe med risikostyring og en række
konsulenthuse tilbyder deres assistance på området.
Det vigtigste er at anvende en metode/model som er acceptabel og mulig at kommunikerer – det skal sikres
at risici håndteres og ikke bare illustreres. Dvs. det afhænger meget af virksomhedens modenhedsniveau,
som oftest er det bedst at starte med en simpel model.
Der er en række gode kilder også bland kommercielle konsulenthuse, også konsulenter som har indset at
det ikke behøver at være meget teoretisk, men kan gøres ganske praktisk. Bl.a. Cyberpilot, som har denne
model som også findes i fællesarkivet til dette kursus.
Side 19
Dansk Standard har udgivet en guide til risikostyring, findes her. Guiden henvender sig bl.a. til SMV-
segmentet og er også en rimelig pragmatisk måde at se på risikostyring. Guide findes i fællesarkivet.
Guiden ser bl.a. på disse tre virksomhedstyper:
Guiden beskriver de overordnede procestrin:
For autoværkstedet er risikoanalysen hjulpet på vej af disse vedtagelser, som naturligvis blot er et
eksempel, men dog en god illustration:
Side 20
Det handler om: Hvad vil man gøre noget ved i praksis?
Hvor stor en risikoappetit har værkstedet?
Vil modellen for ”Produktionsvirksomhed” kunne bruges på eksempel virksomheden?
SikkerDigtital har ligeledes udgivet en vejledning, se her – byggende på ISO27001 standarden har beskrevet
processen således:
Så der er mange modeller at vælge imellem, det vigtigste er at anvende en model som er mulig at
kommunikere og som sikrer at der i praksis sker noget, at ”nogen” vælger hvad man vil med de
Side 21
identificerede risici og ikke blot overlader det til en form for logning af risici. I slideserien er yderligere
nævnt en ENISA model som er en del mere avanceret, som typisk henvender sig til større virksomheder.
Indenfor risikostyring anvendes CIA naturligvis også, skal man lave en risikovurdering kan man anvende
sikkerhedskuben for at sikre man har nået hele vejen rundt. Det vil i praksis være en større opgave at lave
en sandsynlighed og konsekvens vurdering for de relevante områder af sikkerhedskuben. Oftest tænker
man mere eller mindre bevidst CIA ind i risikoanalysen, dermed ses det som hen helheds betragtning.
Udover at vurderer på CIA området kan man på tilsvarende vis vurderer om et scenarie kan opdeles i
forsætlig og uforsætlig.
2.2 Beredskabsstyring
Et område der får stigende og stigende betydning, samfundet bliver mere og mere afhængig af fx digital
infrastruktur – men en lang række områder er også vigtige, Des bl.a. af at EU har direktiver der skal sikre at
samfundsvigtige virksomheder har et tilstrækkeligt sikkerhedsniveau – herunder også er klar til håndtering
af kriser, have styr på sit beredskab.
Som anført i undervisningsslides handler beredskab om at forberede sig på hændelser, dette sker igennem
```
at lave en BIA (Business Impact Analyse) – basalt set en risikoanalyse, hvor de største risici er medtaget. Ud
```
fra denne kan der lave detaljerede planer for hvad skal ske.
Der findes andre mere pragmatiske måde at gøre det på, fx ved at samle potentielle risici identificeret i en
BIA eller en risikoanalyse. Med samling af potentielle risci menes at man har identificeret HVEM der skal
træde sammen med kort varsel og ikke HVAD de skal gøre ned i mindste detalje. Men for store
virksomheder kan den store model være ganske udmærket og det rigtige at gøre.
Tages ”Autoværkstedet” som udgangspunkt, behandlet ovenfor, så vil det nok være på sin plads at tage
stilling til HVEM der skal træde sammen hvis en Høj/Høj hændelse skulle indtræffe.
Beredskabsstyrelsen har udarbejdet en skabelon for beredskabsplaner, den kan hentes her, findes også i
Canvas.
I Canvas er yderligere en skabelon for IT beredskabspolitik, også med denne er der for den enkelte
virksomhed et behov for at finde det rette niveau, det nytter ikke at lave store tunge dokumenter der skal
vedligeholdes ofte, hvis fx virksomheden har en meget flad struktur. Men dokumenter som disse er
glimrende inspirationskilder. Se også afsnittet vedr. ”Implementering” i et senere modul.
Beredskabsstyring og håndtering er beskrevet i yderligere detaljer i slideserien
Modul 3: Compliance
I samfundet er der et stigende krav omkring compliance mod diverse regler sat af det offentlige”. Cyber
området er ingen undtagelse, det handler også her om at efterleve diverse standarder og normer. Kravene
til Cybersikkerhedshåndtering i virksomheder har været stigende og EU har gennem diverse direktiver
skærpet kravene og sikret sig bevågenhed ved bl.a. at fastlægge store bødestørrelser. GDPR-reglerne er et
af de første generelle områder der rammer private virksomheder, næsten uanset størrelse.
```
Helt det samme sker på NIS (Netværk og Informationssikkerhed) området, derom senere.
```
Side 22
En virksomhed kan/skal være compliant på flere områder, også internt kan der fra direktionen være et
ønske om at sikre at man overholder interne regler og standarder.
Sikring af compliance, er ofte en form for revision, hvorfor det ofte udføres af revisions uddannet
personale. Typisk anvendes ”audit teknikker” ved compliance målinger, der findes derfor også en række
forskellige audit uddannelser, fx har Teknologisk institut denne, men der er en lang række udbydere på
dette område.
3.1 Lovgivning
For rigtig mange virksomheder er der lovgivningskrav der skal efterleves, fx indenfor GDPR-området.
Mange love forudsætter at der laves en selvevaluering af om man nu gør det som loven siger man skal. Ved
gennemførelse af love er der, stort set altid, en høringsproces – denne anvendes positivt af juristerne i
staten til at få bl.a. brancheorganisationer i tale for at sikre sig at loven er balanceret og proportionel i
forhold til hvad der ønskes opnået.
Lovgivning udmøntes typisk i bekendtgørelser, det er juristernes måde at operationaliserer tingene på. En
bekendtgørelse kan nu være ganske vanskelig at læse og forstå, kunsten for sikkerhedsfolk er derfor ofte at
oversætte bekendtgørelsens tekst til: Og hvad skal vi så gøre i praksis?
GDPR skulle ikke indarbejdes i dansk lovgivning, men skulle anvendes som formuleret af EU kommissionen,
derved sikres at der er ensartede forhold i hele EU – støtte til det åbne markede.
3.1.1 EU-lovgivning
Mange forskellige love kommer vi EU-systemet, der kan læses om processen her. Nogle af disse skal så
omsættes i Dansk lovgivning andet skal ikke, principperne er følgende:
Forordning
En forordning er en af de retsakter, der anvendes i EU-lovgivning. En forordning er almengyldig, dvs. at den
ikke retter sig mod en bestemt personkreds eller institution.
En forordning er umiddelbart gældende i medlemslandene, hvilket betyder, at forordningen uden
forudgående national indarbejdelse bliver en del af medlemsstaternes love. Forordninger er bindende og
indfører dermed rettigheder og pligter på lige fod med national lovgivning.
Direktiver
Et direktiv fastsætter et mål, men det er op til hvert medlemsland at bestemme, hvordan det vil opnå
målet.
I modsætning til en forordning gælder et direktiv først for borgerne, når de enkelte medlemslande har
indarbejdet bestemmelserne i deres egen lovgivning inden for en bestemt tidsfrist. I Danmark kan et
direktiv f.eks. gennemføres ved en lov eller en bekendtgørelse.
Når et medlemsland har gennemført direktivet i sin lovgivning, skal landet underrette EU kommissionen om
status.
Afgørelser
En afgørelse binder også EU’s medlemslande.
```
En afgørelse har direkte virkning (altså uden vedtagelse i de enkelte EU-landes nationale parlamenter), hvis
```
den er rettet mod en bestemt modtager, f.eks. en virksomhed.
Side 23
Er afgørelsen derimod rettet til medlemslandene, gælder den som et direktiv og dermed for alle EU-lande
```
(som derefter selv må finde ud af, hvordan de hver især vil implementere afgørelsen).
```
3.1.2 NIS2
Netværks- og informationssikkerhedssystemer er blevet en central bekymring i den digitale tidsalder, hvor
vores samfund i stigende grad er afhængigt af en velfungerende og sikker digital infrastruktur. Med den
hurtige digitale udvikling og stigende trusler fra cyberangreb er det blevet afgørende at styrke den
kollektive indsats på området, og EU har derfor vedtaget NIS2-direktivet.
```
NIS2 er en opdateret version af det oprindelige NIS-direktiv (også kaldet Net- og
```
```
Informationssikkerhedsdirektivet), som blev vedtaget i 2016 og trådte i kraft i 2018. Formålet med NIS2 er
```
at styrke cybersikkerheden og beskytte kritiske infrastrukturer og tjenester i EU. Ordet kritisk infrastruktur
skal fortolkes bredt.
NIS2-direktivet regulerer virksomheder og myndigheder på cyber- og informationssikkerhedsområdet, og
lovgivningen stiller krav til implementering af tekniske, driftsmæssige og organisatoriske foranstaltninger
for at kunne håndtere de risici, der truer systemerne.
Det nye NIS2-direktiv er en vigtig milepæl i EU's indsats for at beskytte kritiske infrastrukturer, og det
udmønter sig i nationale bekendtgørelser, som organisationer skal efterleve. I forhold til det oprindelige
direktiv introducerer NIS2 en række forbedringer og opdateringer – herunder:
Udvidet anvendelsesområde: NIS2 dækker et bredere spektrum af sektorer og tjenester, fx
fødevareproduktion og affaldshåndtering samt hele forsyningskæden i de omfattede sektorer.
Forbedret tilsyn og håndhævelse: NIS2 indeholder skærpede krav til tilsyn og håndhævelse af
cybersikkerhedsregler, hvilket giver organisationerne et større ansvar for at sikre overholdelse. I Danmark
er det ”Sektoransvarlige myndigheder”, der fører tilsyn med NIS-loven.
Skærpede krav til sikkerhedsforanstaltninger: NIS2 stiller øgede krav til risikostyring og implementering af
skadesforebyggende og -begrænsende foranstaltninger, der reducerer risici og konsekvenser.
Ved at forstå, hvad NIS2-direktivet er, og hvordan det påvirker organisationen, kan en virksomhed
imødekomme de skærpede krav og undgå sanktionering – og ikke mindst minimere risikoen for
cyberangreb.
I Danmark implementeres NIS 2 gennem en model, hvor de fleste sektorer omfattes af en generel NIS 2-lov,
der er foreslået som lov om foranstaltninger til sikring af et højt cybersikkerhedsniveau. Samtidig sker der
en sektorspecifik implementering for energi-, finans- og telesektorerne på grund af den eksisterende og
omfattende regulering, der allerede gælder på disse områder.
Det betyder dermed at for energi, finans og teleområdet sker der en udbygning af den de eksisterende
reguleringer på deres respektive områder, hvorimod den generelle NIS2 lov gælder for de øvrige sektorer.
Det forventes at der vi ske en opdatering af de eksisterende bekendtgørelser på energi, finans og
teleområdet i løbet af 2025.
Den generelle NIS2 loven blev sendt i høring i sommer 2024, høringsfrist var den 22. august 2024, herefter
skal loven revideres og dens ikrafttrædelse blev sat til den 1. marts 2025, det er i loven anbefalet at der
laves sektorspecifikke bekendtgørelser som der i øvrigt er på fx teleområdet. Hvornår disse sektorspecifikke
Side 24
bekendtgørelser skal være færdig, er ikke specificeret endnu. Det bevirker dog ikke at disse sektorer
dermed ikke behøver at se på NIS2 loven.
I forbindelse med oprettelse af ministerie for Samfundssikkerhed og Beredskab, er det meldt ud at NIS2
endnu engang er udsat til 1. juli 2025, men det er stadig uklart hvilke bekendtgørelser der er færdige til den
tid.
Hvad indeholder NIS2 lovgivningen i praksis
Ledelsesansvar
Organisationens ledelse skal have bekendtskab til direktivets krav, samt dens risikostyringsindsats. Der
kommer således til at være et direkte ledelsesansvar i forhold til at identificere og håndtere cyberrisici samt
sikre, at kravene i NIS2-direktivet overholdes.
Risikoanalyse og -styring
Organisationer, som er omfattet af NIS2-direktivet, skal løbende gennemføre en risikoanalyse og
identificere og vurdere alle væsentlige risici i forbindelse med sårbarheder og trusler. Herefter skal der
indføres passende sikkerhedsforanstaltninger.
Sikkerhedsforanstaltninger
Berørte organisationer skal implementere passende tekniske og organisatoriske sikkerhedsforanstaltninger
for at beskytte deres netværks- og informationssystemer mod cyberrisici. Det kan blandt andet omfatte
opdatering af software og hardware, anvendelse af kryptering, styrkelse af adgangskontrol og etablering af
regelmæssige sikkerhedsrevisioner.
```
Forretningskontinuitet (Beredskab)
```
Organisationen skal forholde sig til – og have en plan for – hvordan kontinuiteten sikres skulle en
cybersikkerhedshændelse opstå. Herunder nødprocedurer og etablering af en kriseorganisation.
Rapportering
NIS2-direktivet kræver, at berørte organisationer rapporterer cybersikkerhedshændelser, der har en
væsentlig indvirkning på kontinuiteten af de tjenester, de leverer. Det betyder, at der skal etableres
processer for, hvordan der rapporteres rettidigt og inden for rammerne.
Hvis ovenstående hændelser indtræffer, skal det indberettes hurtigst muligt på Virk.dk – og senest inden
for 24 timer. Organisationen skal blandt andet oplyse om:
• antallet af brugere berørt af hændelsen
• hændelsens årsag og varighed
• det berørte geografiske område, herunder andre EU-lande
• håndtering af hændelsen
Når indberetningen sker på Virk.dk, bliver den automatisk sendt til både Erhvervsstyrelsen og Center for
Cybersikkerhed.
Forsyningskæden
Side 25
Under NIS2-direktivet skal de omfattede organisationer også tage hensyn til deres forsyningskæders
sikkerhed. Det betyder, at virksomheden skal vurdere og håndtere risiciene forbundet med virksomhedens
leverandører og andre samarbejdspartnere i forsyningskæden.
I praksis opfordrer NIS2 organisationer til at implementere passende sikkerhedsforanstaltninger og
overvåge forsyningskæden for at minimere risikoen for cyberangreb. Det kan blandt andet ske ved at
indføre krav til leverandører om at overholde specifikke sikkerhedsstandarder, gennemføre regelmæssige
sikkerhedsrevisioner og kræve, at leverandører rapporterer eventuelle cybersikkerhedshændelser.
Man kan afprøve en virksomheds NIS2 parathed gennem denne test. Dette er en større afklaring som kan
være ganske nyttig at gennemføre for en virksomhed og peger på hvor der skal sættes ind.
Overvej at gennemføre testen for Hvedebro Maskinfabrik.
Hvem er omfattet, NIS2 skelner mellem essentielle og vigtige virksomheder – alle skal ses som
```
samfundsvigtige:
```
Side 26
I loven, bilag 1 og bilag 2 findes detaljen om hvem der er omfattet, desværre henviser bilagene til EU-
direktivet, så man skal også forbi dette for at få det fulde overblik – direktivet kan henvise til tidligere
direktiver, så det kan være en vanskelig proces. Dansk lovgivning kan hjælpe med en afklaring.
Men hvordan kan man nu være sikker på om man er omfattet i praksis? – det er ikke altid indlysende,
compliancekravet omfatter virksomheder indenfor disse kategorier:
1. Omfattet direkte af lovgivningen, dvs. det er indlysende da branchen/området er nævnt i bilag 1
eller bilag 2
2. Man er som virksomhed specifikt udpeget af myndighederne
3. Det er et krav fra vigtige kunder
4. Virksomheden ser det som en konkurrencefordel
Styrelsen for Samfundssikkerhed har udarbejdet en lang række gode og anvendelige dokumenter som kan
hjælpe virksomheder med, dels af finde ud af om man er omfattet og hjælpe med implementering.
Et mere uddybende spørgeskema kan findes her.
For en virksomhed som Hvedebro Maskinfabrik, der laver komponenter til de virksomheder der laver
maskiner til fødevareproducenter, er man ikke umiddelbar omfattet af NIS2. Men som beskrevet ovenfor,
kan der være andre grunde. Det konkrete område er omfattet af ”Fødevarestyrelsens” tilsyn – yderligere
information vedr. eventuel omfatning af NIS2 kan findes her.
Side 27
Har man fundet ud af at man kan være omfattet, er næste step om man er en ”Væsentlig” eller ”Vigtig”
virksomhed, set med NOS2 definition. Dernæst størrelse og omsætningsforhold. Er det på plads handler det
om hvad der egentlig står i loven og om der er sektorspecifikke anvisninger, bekendtgørelser eller lign.
Det har yderligere været til debat om hvorvidt det er hele virksomheden, eller kun dele af en virksomhed,
der er omfattet – det er fastslået at er en virksomhed omfattet, så er det hele virksomheden. Det samme
gælder for offentlige forvaltninger og virksomheder.
Er man omfattet skal man registres se her
Kapitel 2 i loven starter med at definere hvad det i praksis går ud på:
§ 6. Væsentlige og vigtige enheder skal træffe passende og forholdsmæssige tekniske, operationelle og
organisatoriske foranstaltninger for at styre risiciene for sikkerheden i net- og informationssystemer, som
disse enheder anvender til deres operationer eller til at levere deres tjenester, og for at forhindre hændelser
eller minimere deres indvirkning på modtagere af deres tjenester og på andre tjenester. Foranstaltningerne
skal som minimum omfatte følgende:
```
1) Politikker for risikoanalyse og informationssystemsikkerhed.
```
```
2) Håndtering af hændelser.
```
```
3) Driftskontinuitet, herunder backupstyring og reetablering efter en katastrofe og krisestyring.
```
```
4) Forsyningskædesikkerhed, herunder sikkerhedsrelaterede aspekter vedrørende forholdene mellem den
```
enkelte enhed og dens direkte leverandører eller tjenesteudbydere.
```
5) Sikkerhed i forbindelse med erhvervelse, udvikling og vedligeholdelse af net- og informationssystemer,
```
herunder håndtering og offentliggørelse af sårbarheder.
```
6) Politikker og procedurer til vurdering af effektiviteten af foranstaltninger til styring af
```
cybersikkerhedsrisici.
```
7) Grundlæggende cyberhygiejnepraksisser og cybersikkerhedsuddannelse.
```
```
8) Politikker og procedurer vedrørende brug af kryptografi og, hvor det er relevant, kryptering.
```
```
9) Personalesikkerhed, adgangskontrolpolitikker og forvaltning af aktiver.
```
```
10) Brug af løsninger med multifaktorautentificering eller kontinuerlig autentificering, sikret tale-, video- og
```
tekstkommunikation og sikrede nødkommunikationssystemer internt hos enheden, hvor det er relevant.
Måske ikke det mest operationelle, men nok til at give et tydeligt billede af hvad compliance kræver
Lovgivningen indeholder også krav til underretning ved hændelser, i praksis skal disse ske til virk.dk, i §12
fremgår følgende:
§ 12. Væsentlige og vigtige enheder skal underrette den relevante kompetente myndighed og Computer
```
Security Incident Response Team (CSIRT) om enhver væsentlig hændelse. En underretning skal indeholde
```
oplysninger, der gør det muligt at fastslå eventuelle grænseoverskridende virkninger af hændelsen.
Stk. 2. En hændelse anses for at være væsentlig, hvis en af følgende betingelser er opfyldt:
Side 28
```
1) Hændelsen har forårsaget eller er i stand til at forårsage alvorlige driftsforstyrrelser af tjenesterne eller
```
økonomiske tab for den berørte enhed.
```
2) Hændelsen har påvirket eller er i stand til at påvirke andre fysiske eller juridiske personer ved at forårsage
```
betydelig fysisk eller ikkefysisk skade. Stk. 3. Vedkommende minister kan efter forhandling med ministeren
for samfundssikkerhed og beredskab fastsætte nærmere regler om, hvornår en hændelse kan anses for at
være væsentlig.
I praksis er noget rummeligt, men alene at ”Økonomisk tab” indgår, bevirker at en del skal rapporteres, det
vil typisk fremgå felter i virk.dk hvad underretningen skal indeholde. Bemærk også, som tidligere nævnt,
tidsfristerne for anmeldelse. Myndighederne kan derudover kræve en mere stringent opfølgning.
For primært større virksomheder:
Dansk Industri har udarbejdet en model for afklaring nogle af de vigtigste områder for at blive NIS2
compliant, og hvem der skal have ejerskab af at det sker indenfor hvert hovedområde:
Områder/foranstaltninger Status
Roller i
store/større
organisationer
Roller i små/mindre
organisationer
```
Politikker: Defineret risikoanalyse og informations
```
sikkerhed politikker Ledelses-team Adm. direktør
Hændelser: Defineret procedure for håndtering af
hændelser SOC/CDC Sikkerhedspersonale
Beredskab, BCM og IT-katastrofeberedskab skal
være beskrevet og implementeret Krisestyringsteam Øverste ledelse
Supply-chain: Risikovurdering af forsyningskæden
med detaljeret oplysninger og risiko og relationer
mellem hver enhed
Risikostyringsteam Øverste ledelse
Leverandør håndtering GRC-team IT-drift
Politikker og procedure for løbende at vurdere
effektiviteten til styring af cybersikkerhedsrisici GRC-team Sikkerhedspersonale
Implementeret awareness træning af alle relevante Awareness team IT-drift
Politikker og procedure for kryptografi GRC-team Adm. direktør
Politikker for adgangskontrol og håndtering af
aktiver IT og Jura
Sikkerheds
personale
Brug af MFA og tilsvarende løsninger hvor relevant IT-drift IT-drift
Side 29
Advokatfirmaet ”Kromann og Reumert” har udarbejdet hvad de kalder ”Pejlemærker og
observationspunkter til NIS2 compliance, findes her og i Canvas. Det er en glimrende oversigt over hvad de
også kalder minimumskrav, det skal huskes at der er mange forskellige måder at implementere på alt efter
virksomhedens modenhedsniveau, men uanset modenhed så er der minimumskrav som for mange
virksomheder vil være en overraskelse.
Side 30Side 31
Det må forventes at brancheorganisationerne vil komme med yderligere vejledninger og anbefalinger fra
efteråret 2025 og frem.
3.1.3 GDPR
GDPR-forordningen havde virkning fra april 2018 og har således været en integreret del i mange
virksomheder i en årrække. I mange sammenhæng er Cybersikkerhed kontroller tænkt som en måde at
sikre compliance mod GDPR, det er delvis rigtig – men også kun delvis. GDPR handler om at beskytte
persondata, medarbejderes og kunders. På kundesiden er det forretningen der ejer kundedata og det er
derfor i de fleste virksomheder et forretningsansvar at sikre GDPR overholdelse, godt hjulpen af de
sikkerhedspolitikker og standarder virksomheden har. Det er ofte også forretningen der anmelder brud til
virk.dk og ikke Sikkerhedsafdelingen. Større virksomheder skal have en person der er ansvarlig for
```
persondata, kaldet en DPO (Data Privacy Officer).
```
Side 32
Der skal ikke her ske en gennemgang af GDPR, men det er vigtig at GDPR er reflekteret i bl.a.
sikkerhedspolitikker og processer. Hovedprincipperne er:
• Der skal være et lovligt behandlingsgrundlag for at indsamle og behandle persondata
• Der skal være en grund til at behandle og gemme persondata, man kan ikke bare gemme
persondata fordi de er gide at have
• Der skal være en slette politik, der skal tages stilling til hvor længe persondata må opbevares, for at
opfylde de formål de er indsamlet til.
• Man skal sikre sig at data er korrekte
• Man skal sikre integritet og fortrolighed omkring persondata
• Man skal kunne dokumentere hvordan persondata behandles
Dertil kommer en række processer, hvis fx en kunde udbeder sig oplysninger om hvilke persondata der er
indsamlet, proces for anmeldelse af brud osv.
Typiske anmeldelser af GDPR-brud handler om:
• Dårlig datakvalitet
• At man sender persondata til den forkerte
• At man offentliggør persondata uden viden
En interessant ting ved GDPR-forordningen er at det kun er private virksomheder der kan få bøder, ikke den
offentlige sektor.
3.1.4 GDPR og NIS2
Er NIS2 regler og GDPR så ikke bare det samme?
Nej, det er det bestemt ikke, men er der styr på GDPR-området må det forventes at der godt styr på den
basale sikkerhed, er man så samtidig ISO27001 certificeret eller compliant, ja så er man rigtig godt på vej.
Men der mangler stadig hele supplychain området, sikre at topledelsen er orienteret i detaljer samt
rapportering til myndighederne ved hændelser og hvad der ellers måtte komme når lovgivning kommer på
plads i 2025
Ovenstående er forventningen, men staten er velkommen til at indfører yderligere end det der fremgår af
NIS2 direktivet, dette vil så fremgå af de bekendtgørelser der forventes i 2025.
3.1.5 CER-direktivet
CER-direktivet omhandler som NIS2 de samfundskritiske sektorer, rammer derfor nogenlunde de samme
brancher som listet i NIS2 – dog knap så mange sektorer. CER har mest fokus på fysiske
sikkerhedsforanstaltninger og hvad der følger med i den anledning. Som ved NIS2 er der fokus på
beredskab og krisestyring, med det formål at gøre hver enkelt omfattet virksomhed bedre og mere robuste
ved kriser.
CER-direktivet er vedtaget samtidig med NIS2 og DORA, DORA har fokus på den financielles sektor.
De tre reguleringer, NIS2, DORA og CER, supplerer hinanden på tværs af samfundskritiske sektorer. De
afspejler dels prioriteterne i Kommissionens strategi for EU's sikkerhedsunion, der opfordrer til en revideret
tilgang til fysisk og cyberrelateret modstandsdygtighed i kritisk infrastruktur, dels den stadig tættere
```
indbyrdes afhængighed mellem forskellige sektorer og deres fysiske og digitale infrastrukturer og (hybride)
```
Side 33
risikolandskab. Det forventes at CER-direktivet vil dække 100-150 udpegede virksomheder indenfor 10
sektorer
Den stigende anvendelse af cyberfysiske systemer, hvor mennesker, produkter og maskiner kommunikerer
med hinanden via intelligente og internetopkoblede systemer, får det fysiske og det digitale domæne til at
smelte sammen. Det øger risikoen for, at eksempelvis et cyberangreb også kan forstyrre eller ødelægge
fysisk infrastruktur, eller at sabotage mod fysisk infrastruktur gør digitale services utilgængelige eller
kompromitterer data.
Det har været debatteret hvad modstandsdygtighed egentlig betyder i forbindelse med de tre områder, i
EU har man forsøgt sig med denne definition fra 2022:
en kritisk infrastrukturs evne til at forebygge, beskytte sig mod, reagere på, modstå, afbøde, absorbere,
tilpasse sig til eller komme sig over hændelser, som i væsentlig grad forstyrrer eller har potentiale til i
væsentlig grad at forstyrre leveringen af væsentlige tjenester på det indre marked, dvs. tjenester, som er
afgørende for opretholdelsen af vitale samfundsmæssige og økonomiske funktioner, den offentlige
sikkerhed og sikring, befolkningens sundhed eller miljøet.
3.2 Standarder
Man, siger ofte at en af de gode ting ved standarder er at der er så mange af dem, det er også rigtigt – der
er dog standarder som er internationale og som man kan blive certificeret efter. Fremfor selv at skulle
```
opfinde sikkerhedsregler (kontroller, foranstaltninger), er det naturligt at se til standarderne og så udvælge
```
sig de regler/kontroller som passer i den givne situation – fx relevant for den givne sikkerhedspolitik – for
de risici virksomheden står overfor.
3.2.1 ISO27000 familien
ISO27000 familien indeholder på global basis de mest kendte standarder indenfor Cybersikkerhed – kaldes
også for” Information Security Management”. Et overblik over aktuelle standarder i familien kan findes her.
Søger man certificering eller compliance ses der som udgangspunkt på ISO27001, her skal ISO27002
anvendes som implementeringsvejledning, for hvad der reelt skal ske. ISO27001 er som det fremgår meget
overordnet.
SOA
Hvis man ønsker compliance eller certificering på bestemte områder, skal dette noteres i hvad der kaldes
```
en SOA (Statement of Applicability) mere herom fx her.
```
I en SOA skal det forklares:
• Hvilke kontroller der er valgt
• Om hvorvidt kontrollen er fuldt implementeret
• Hvorfor disse er valgt
• Hvorfor andre er fravalgte
Man bør søge råd og vejledning hos et certificeringsfirma, hvis der ønskes en certificering. Der kan blive tale
om at udvide scope for at få en certificering. Er der tale om at anvende standarden i forbindelse med intern
compliance, er det en god øvelse at begrunde sine valg og fravalg i en SOA.
Side 34
Med udgangspunkt i sikkerhedspolitikker, så skal man sikre sig at man har vedtagne politikker der dækker
de områder man har tilvalgt i sin SOA.
ISMS
Oftest tænkes ISMS som et system, hvilket det også er ofte, men det kan også blot være en række
processer, der sikrer at man efterlever standardens processer, i praksis vil det sige det der kommer før
Annex A i standarden. Denne del behandles ofte lemfældigt, men processerne skal være på plads for at
kunne få en certificering – uanset hvor meget man har begrænset sig i SOA.
Et ISMS betegnes på dansk som et ”Ledelsessystem”, som skal være med til at sikre sig at man løbende
forbedre sig og løbende identificerer om virksomhedens risikobille er reflekteret i politikker og standarder,
dette er ofte illustreret som:
Løbende at forbedre sig er en fundamental del af alle ISO-dokumenter. Som nævnt findes der en række IT-
systemer der kan understøtte arbejdet, disse kan være cloud baserede – men ofte ønsker at man denne
type information er gemt lokalt. I Danmark bruges ofte den dansk udviklede system fra Neupart.
3.2.2 NIST
NIST er en organisation, hjemmehørende i USA. NIST udgiver en lang række standarder, vejledninger mv.
indenfor en række områder, herunder indenfor Cybersikkerhed, se eventuelt her.
```
De bagvedliggende vejledninger (guidlines og best practices) er ganske glimrende og udmærket at bruge i
```
specifikke politikker og standarder.
Også i NIST bruges orden ”Cybersecurity Framework”, dette er løbende under udvikling og blver tilpasset
bl.a. det risikobillede man ser. Man kan følge med i udviklingen via denne side.
```
Framework:
```
Side 35
Indenfor hver af disse 5 områder kan der laves en assessment, dvs. en vurdering af hvor god man er på det
givne område indenfor fx en bestemt teknologi eller organisation. På den måde er NIST et ganske
udmærket værktøj til at anskueliggøre hvor virksomheden er i sit modenhedsniveau og samtidig anvende
metoden til at fastsætte en ambition for hvor man vil hen:
Side 36
Mange konsulenthuse anvender denne model, dels for at dokumenterer hvor virksomheden er i praksis,
også fastsætte et ambitionsniveau.
Man anvender værktøjet til at komme nærmere ind på hvilket modenhedsniveau man er, en konkret
metode til dette er i Canvas. Fra denne er her et eksempel indenfor ”Asset Management”
Indenfor de 6 områder ”ID.AM-X
Indenfor de 6 områder kaldet ”ID.AM-x” er det så vurderet, fx ID.AM-1, ses under ”UD Observations” og UR
Recomendations” – se ovenfor.
I eksemplet er der for alle 6 områder lavet en vurdering der har resulteret i en score på:
Side 37
```
Established = Defined I de to figurer og dermed “Risks to IT assets are identified and managed in a standard
```
and defined process”.
Eksemplet ovenfor tydelig illustrere at det er et omfattende kompleks af vurderingsmekanismer.
3.2.3 CIS Security Controls
I mange sammenhænge anvendes ”CIS Security Controls”, anvendes ofte i forbindelse med assessment af
sikkerheden i en virksomhed. Er som sådan ikke en officiel standard, men en god rettesnor for hvad der er
vigtig af fokuserer på. I Canvas er der en yderligere detaljering, poster og et Excel tool der kan bruges til
assessment af hvor virksomheden er.
Som det fremgår, er kontrollerne meget IT orienteret og er meget langt fra det generelle kontrolkatalog
som ISO 27001 eller 27002 indeholder, man kan sige at CIS har et Cyber fokus.
CIS-kontrollerne er opdelt i disse områder:
Side 38
Bruger man værktøjer her, kan man komme direkte til detaljen i her enkelt kontrol.
IG1, IG2 og IG3 kaldes ”Implementation Groups”, reelt er det hvor mange kontroller der er indeholdt.
Således indeholder IG1 56 ”Safeguards” og IG2 yderligere 74 ”Safeguards”, IG3 er så igen yderligere 23
”Safeguards”. Dermed kan det samlede kontrolkatalog komme op på 153 kontroller eller ”Safeguards” som
det hedder i CIS sproget.
Kan man så kalde CIS for en standard, det er der forskellige meninger om, men forskellige konsulenthuse
bruger kontrollerne til at få en mål for hvor langt en virksomhed er på cyberområdet.
3.2.4 Andre standarder
Som nævnt er en af de gode ting ved standarder at der er så mange af dem
PCI-DSS
Dækker betalingskortområdet og anvendes derfor globalt da både MasterCard, VISA og andre kræver
denne standard overholdt for at man må håndtere kreditkort transaktioner, en del virksomheder behandler
i realiteten ikke kreditkort information, dvs. når man betaler kommer der et vindue hvor man taster
informationen, disse data går til en service provider, som hvis transaktionen er ok sender en token retur til
Side 39
butikken. Token indeholder så godkendelse eller afvisning af transaktionen. På deres hjemmeside er der en
del information. Et overblik over hvilke sikkerhedskontroller standarden kræver findes her.
Common Criteria
Også en anvendt international standard, udstyr/IT-systemer kan blive certificeret i 7 forskellige niveauer,
detaljeret information her. På hjemmesiden kan man også finde information om hvilke produkter der er
certificeret, se her.
De firmaer der laver testene skal være certificerede til at gøre det. De 7 niveauer dækker over:
Der er tale om en meget omstændig test og blot få ændringer, fx patches, forudsætter at test gentages.
Militæret anvender CC testene, men også en række større private og offentlige anvender disse tests.
3.2.5 ISF Security Model
```
ISF (Information Security Forum) har en udmærket standard med praktisk tilgang kaldet ”Standard of Good
```
Practice”. ISF er en forening, så det er medlemmerne der bidrager og ansatte samler s sammen. Udover
standarden udgiver ISF en række andre dokumenter og vejledninger. En del danske virksomhed er medlem
af ISF, der er da også en dansk Erfagruppe som er aktiv som det kan være interessant at være medlem af.
Side 40
3.3 Audit
Audit er en metode, dvs. hvis man er auditor er det nogenlunde ligegyldig hvad der skal auditeres. Som
auditor lænder du dig op af regler/kontroller og spørger så til overholdelse og noterer afvigelser. Audit er
derfor en formel proces, hvorimod ”review” ”Compliance måling” eller ”assessment” kan være mere
uformelle og ofte det man anvender internt i virksomheder. Men kalder man på et eksternt firma, vil det
oftest være en formel proces. Ofte bruges audit lidt i flæng
Ved en audit skal der først laves et audit-scope, dette vil typisk indeholde:
• Hvad audit skal omhandle
• Hvad der forventes leveret som evidens
• Hvem der skal deltage
• Forventet tidsforbrug
Man kan lave audit på hvad som helst. Resultatet af en audit er en auditrapport, indeholder typisk:
• Ledelses opsummering
• Audit scope, måske i lidt reduceret form
• Hvem der var auditor, deltagere og observatører
• Resultat af det enkelte auditpunkt
• Observationsliste med prioritering
Har man lavet en tilsvarende audit, fx året før vil audit også omhandle om de observationer der blev lavet
sidst, er håndteret, evt. at se evidens herfor. Auditrapporten sendes altid til de involverede for deres
kommentering, auditor kan have misforstået noget, når endelig auditrapport er færdig sendes den til senior
ledelse.
Observationer vil normalt medføre at der er identificeret en risk, så måske skal et risk register opdateres
eller der skal laves en ny risikoanalyse.
3.4 Rapportering
Rapportering af status på sikkerhed er en vigtig aktivitet for enhver sikkerhedsafdeling, rapporteringen
udgør ofte både en fortrolig del og en del der er tilgængelig for relevante medarbejder og ledere i
virksomheden. Den fortrolige del er oftest mere tilegnet topledelsen, da den f.eks. kan indeholde detaljer
om sårbarheder og hændelser som ikke skal være almenkendt i virksomheden.
Præsentationsformer:
```
KPI (Key Performance Indicator), er ofte metoden der anvendes også til sikkerhedsrapportering, men også
```
```
KSI (Key Security Indicator) kan anvendes – men de to kan også hænge sammen.
```
Der findes mange kilder til relevante KPI’er, ofte arbejder brancher sammen omkring dette – men der er
produkter og konsulenthuse der har det som produkt, et eksempel er her.
Et alternativ til at udsende rapporter er at have et Dashboard, dvs. en portal hvor man løbende kan se
status indenfor det område man har defineret som relevant at rapportere omkring. Dashboards er ofte
noget der følger med når han kører fx beskyttelse mod malware og et administrationsmodul. Et eksempel
herpå:
Side 41
```
SOC (Security Operation Centers) har ofte sine egne KPI’er, bl.a. for løbende selv at overvåge om de er
```
hurtige nok til at reagere på hændelser, eksempel på SOC KPI’er hentet herfra: :
Et eksempel på en omfattende månedsrapport findes i Canvas, uddrag på slides.
Side 42
Generelt er måling på hvor mange ”Incidents” der detekteres pr. tidsenhed en god parameter for enhver
virksomhed, sig ikke nødvendigvis noget om hvor god man er til at opdage incidents, men fortæller mest
noget om en trend, hvilket også er nyttig.
Kan skal ikke underkende at sikkerhedsrapportering også er god intern markedsføring. Via rapportering
dokumenterer sikkerhedsafdeling hvilken betydning den har – ja medmindre der ikke er noget at
rapporterer.
Side 43
Et er hvordan den enkelte virksomhed vælger at lave sikkerhedsrapportering, noget andet er hvad man på
national og global basis gør, interessant er bl.a.:
Dansk trusselsrapportering
Global sikkerhedsrapportering
Dertil kommer at en del sektorer udgiver diverse rapporteringer, set med danske øjne kan disse være
```
interessante:
```
Sundhedsvæsen i Danmark
```
Undersøgelsesrapporter udgivet af CFCS (Center for Cybersikkerhed) i Danmark
```
EnergiCERT trusselsvurdering
3.5 Awareness
En vigtig aktivitet for en sikkerhedsafdeling er at sikre at organisationen har viden om hvilke
sikkerhedspolitikker der findes og som forventes efterlevet, men derudover rummer awareness også
muligheden for løbende at uddanne medarbejdere i ”god sikkerhed” eller hvad man nu vælger at kaldet
det.
Ofte er det en god ide at en awareness kampagne både er morsom og relaterer sig til både noget firma og
privatrettet, derudover kan awareness kampagner naturligvis være rettet specifik mod fx en
udviklingsafdeling.
Uanset hvor man beskyttelsessystemer man har i en virksomhed, så er den enkelte medarbejder ofte den
største trussel mod virksomheden, man anvender ofte orden ”The Human Firewall”, så det handler om at
den enkelte medarbejder skal være bevidst om hvad vedkommende gør og samtidig ved hvem man skal
henvende sig til hvis man oplever noget mistænkeligt.
```
Eksempler:
```
Side 44
Omkring kodeord er denne tankevækkende:
Side 45
Generelt anvend illustrationer som siger noget, der findes en række udbydere som tilbyder pakker med
awareness træning, et eksempel er CyberPilot som har opsummeret deres erfaringer her:
1. Start med at få dine medarbejdere ombord
2. Kommunikér og frem indsatsen
3. Vis både den personlige og arbejdsmæssige vigtighed ved Cybersikkerhed
4. Hold det simpelt
5. Tilbyd træningen i små stykker
6. Lav relevant indhold
7. Lav det interaktivt
8. Gør det let tilgængeligt
9. Brug forskellige læringsmetoder
10. Gør træningen kontinuerlig
11. Evaluer og følg op med dine medarbejdere
De 11 punkter er detaljeret yderligere i link ovenfor.
Awareness træning får et større og større prioritering i danske virksomheder, ifølge PwC undersøgelse
”Cybercrime survey”, yderligere information i modul 5 hvor også rapporten findes. Her konkluderer PwC
følgende:
Side 46
Det er en ganske interessant udvikling og en tydelig erkendelse af at den menneskelige faktor betyder
meget. Ind imellem anvendes termen at den vigtigste firewall er den menneskelige.
3.6 Fysisk sikkerhed
Fysisk sikkerhed har traditionel haft større bevågenhed en ”logisk sikkerhed”, sådan er det ikke længere. I
mange virksomheder er fysisk sikkerhed noget der følger med og ikke noget der tiltrækker sig megen
opmærksomhed. Fysisk sikkerhed handler om at beskytte aktiver, herunder personer.
ISO27001 har en særskidt sæt af kontroller der relaterer sig til fysisk sikkerhed:
Side 47
Derudover kan der være tale om sikring af at personer der skal ansættes, eller have adgang til bestemte
områder, skal være fx sikkerhedsgodkendte eller som minimum have en ren straffeattest.
Side 48
Et område der ofte har særlig interesse er datacentre, for disse findes der særlige standarder, ofte kaldet
SOC x, hvor x er udgaven – kan være 1,2 eller 3. En meget stor del af de kontroller der er i ISO27001 findes
også i SOC 2. Der kan læses mere om SOC er.
Søger man viden om danske anbefalinger, så er ”Forsikring og Pension” en god kilde, prøv eventuelt deres
Sikringsguide. For virksomheder er der god inspiration at hente her. Vil man mere detaljeret, fx hvis der skal
beskyttes en fabrikshal, så kan sikringsniveauerne være en god indgang. Som det ses, er der 6 forskellige
niveauer. En produktionshal kunne fx være skalsikret i henhold til sikringsniveau 30. Men der skal som altid
anvendes en risikobetragtning.
F&P opdeler de fleste sikringsniveauer i tre områder:
• Skalsikring
• Cellesikring
• Objektsikring
Generelt indeholder vejledninger/standarder fra F&Å en lang række både gode og inspirerende specifikke
detaljer om fysisk sikkerhed og sikring.
Side 49
Modul 4 – Teknik
Dette modul omhandler en række tekniske områder:
• Grundlæggende IP-viden
• IP-protokollen
• Netværkskomponenter og arkitektur
• Log Management
• IoT
• OT
• WiFi
• Kryptering
• Cloud
Men først skal der etableres en grundlæggende IP-forståelse
4.1 Internet historik
```
IP-protokollen styres af IEFT (Internet Engineering Task Force) og er den teknisk kyndig ansvarlig for IP-
```
protokol og dermed basis i internettet, IEFT kan findes her. Man kunne fristes til at tro at alt var
færdigudviklet, men nej der sker til stadighed ændringer. Disse ændringer sker i en meget demokratisk
```
proces og alle protokoller er detaljeret beskrevet i det der kaldes en ”rfc” (Request for Comments”).
```
Processen er beskrevet her og en oversigt over rfc’er er her.
Historien er beskrevet yderligere her, interessant er det dog at vide at det er det amerikanske militær der
står bag IP protokollen og dermed internet, det var behovet for sikker kommunikation. Internet er en af de
største revolutioner i det 20 århundrede. Det hele startede med ARPANET, ønsket om i 1960 årene at
forbinde Pentagon systemer sammen på en sikker måde. Arpanet kørt i praksis helt til 1990 og var en vigtig
kommunikations kanal under ”den kolde krig”.
Arpanet udviklede sig til det vi i dag kalder Internet. Den første e-mail blev sendt over ARPANET i 1971. IP-
version 4 blev ret hurtig givet fri og industrien kastede sig over den og producerede hurtigt en lang række
systemer og netværkskort.
Hvis man peget på personer der har ”opfundet” internet, så peges der oftest på:
Side 50
4.1.1 IP-version 4 vs. version 6
IP-version 4 er den vi kender og bruger, så når vi blot sikre IP, så er det i praksis version 4 der refereres til.
IP-version 6 blev udviklet for bl.a. at sikre en mere sikker kommunikation og få et langt større adresserum.
IP-version 6 kaldes ofte næste generations internet protokol og er i realiteten udviklet og klar til brug, det
er yderst begrænset hvor meget version 6 anvendes i praksis, men de fleste netværkssystemer kan
anvende version 6, man kan følge med i udviklingen her. Som ved version 4 er det IEFT der er ansvarlig for
udviklingen.
Hvad blev der af IP-version 5?
Allerede i 2011, blev den sidste blok af version 4 IP-adresser allokeret, så den udvikling der reelt var i gang
omkring version 5 blev stoppet. I praksis blev version 5 aldrig til noget
4.1.2 OSI-modellen og trafik
OSI-modellen er grundlaget for IP-trafik, denne skal ikke kendes i detaljer i forbindelse med dette kursus,
men dog skal man kende navnene på de overordnede lag, og fx være opmærksom på at IP-routing sker på
lag 3.
Der findes mange gode beskrivelser af modellen, i denne figur er modellen relateret til de forskellige IP-
```
protokoller:
```
Flere detaljer kan fx findes her.
Der flyttes enorme mængder trafik i internettet, figurer som disse taler deres tydelige sprog:
Side 51
4.2 IP-adresse
En IP-adresse er en unik adresse, der identificerer en enhed på internettet eller et lokalt netværk. IP står i
denne forbindelse for "Internet Protocol", som er det sæt regler, der styrer formatet af data sendt via
internettet eller det lokale netværk.
I bund og grund er IP-adresser den identifikator, der gør det muligt at sende information mellem enheder
på et netværk: de indeholder placeringsoplysninger og gør enheder tilgængelige for
kommunikation. Internettet har brug for en måde at skelne mellem forskellige computere, routere og
websteder på. IP-adresser er en måde at gøre det på og udgør en væsentlig del af, hvordan internettet
fungerer.
En IP-adresse er en række tal adskilt af punktum. IP-adresser er udtrykt som et sæt af fire tal - et eksempel
på en adresse kan være 192.158.1.38. Hvert tal i sættet kan variere fra 0 til 255. Så det fulde IP-
adresseringsinterval går fra 0.0.0.0 til 255.255.255.255.
```
IP-adresser er ikke tilfældige. De er tildelt af Internet Assigned Numbers Authority (IANA), en afdeling
```
```
af Internet Corporation for Assigned Names and Numbers (ICANN). ICANN er en non-profit organisation,
```
der blev etableret i USA i 1998 for at hjælpe med at opretholde sikkerheden på internettet og gøre det
muligt for alle at bruge det. Hver gang nogen registrerer et domæne på internettet, går de gennem en
domænenavnsregistrator, som betaler et mindre gebyr til ICANN for at registrere domænet. Man kunne så
godt tro at ICANN var en form for ”Internet politi”, men en sådan enhed findes ikke. EU har kritiseret USA
for at være for lukkede omkring ICANN arbejdet og EU har da også sæde i ICANN nu, Se eventuelt her
Det at udstede IP-adresser er decentraliseret, i Europa er det RIPE, etableret i 1992 med hovedsæde i
Amsterdam. De regionale registre fremgår af denne oversigt:
Side 52
```
• ARIN (American Registry for Internet Numbers): inklusive Canada, USA og nogle caribiske øer
```
```
• APNIC (Asia Pacific Network Information Centre): inklusive Asien/Stillehavsregionen
```
```
• RIPE NCC (Réseaux IP Européens Network Coordination Centre): inklusive Europa,
```
Mellemøsten og Centralasien
```
• LACNIC (Latin America and Caribbean Network Information Centre): inklusive Latinamerika og
```
nogle caribiske øer
```
• AFRINIC (African Network Information Centre): inklusive Afrika-regionen
```
4.2.1 MAC-adresse
Hver enhed på et Ethernet/WiFi og Bluetooth har en MAC adresse, en helt unik adresse som kun det ene
```
interface har, MAC adressen har således stor betydning for identifikation af NIC (netværks interface) og
```
dermed enheden. Det er den enkelte leverandør der skal sikre at MAC adressen bliver tildelt hver enhed
der produceres, men leverandøren for tildelte et adresserum. MAC adressen kaldes ofte ”Hardware
adressen”.
MAC adressen består af en 48 bit adresse rum og der er således 248 forskellige muligheder – det er mange.
Det er de tre første oktetter der identificerer leverandøren:
Side 53
Det skal ikke her detaljeres yderligere, man kan selv søge mere information fx her.
4.1.2 Typer af IP-adresser
Som almindelig forbruger har man sit eget adresserum på ens eget lokalnet og ISP’en stiller så ofte en
dynamisk eller statisk IP-adresse til rådighed på internettet. Har man adgang til ISP-routeren, vil man kunne
se hvilke adresser der er tildelt hvilke enheder internt – det er fra TV, PC, MAC, Telefoner, printere og IoT
enheder – alt hvad der har en IP-adresse, fra egen routeroversigt:
Det kan være ganske spændende at følge hvad der er forbundet til ens eget lokalnet, man kan blive
overrasket. Mange routere giver også mulighed for at der kan leveres alarmer hvis nye enheder tilslutter
sig.
Offentlige IP-adresser findes i to former – dynamiske og statiske.
Dynamiske IP-adresser ændres automatisk og regelmæssigt. Internetudbydere køber en stor pulje af IP-
adresser og tildeler dem automatisk til deres kunder. Med jævne mellemrum tildeler de dem igen og sætter
de ældre IP-adresser tilbage i puljen for at blive brugt til andre kunde har man fx egen game eller
mailserver, vil man som oftest gerne have en statisk IP-adresse og en sådan kan normal købes for en fast
pris på måned.
Mange fx webhoteller deler IP-adressen med forskellige websider, men det er udenfor dette scope.
Side 54
Vil man gerne kunne se hvilken offentlig IP-adresse man har, så kan man slå den op her. Forfatteren til disse
noter har hjemme følgende:
Ovenstående link kan også anvendes til at finde IP-adressen på fx en given URL – man kan som firmaer og
WEB udbydere skjuler oplysninger, så man i praksis kun kan se den rå IP-adresse. Dette er af
sikkerhedsgrunde.
Hvis man nu opdager at en underlige IP-adresse optræder på sit lokalnet, ellers ene router har detekteret i
en log at der er forsøgt en indtrængning, så kan man på basis af IP-adressen finde ud af hvorfra
kommunikationen er kommet. Her er ICANN en god indgang. Man kan her få en del oplysninger om IP-
adressen, fx hvem man kan kontakte hvis man vil klage over noget.
Som nævnt er det muligt at anvende et privat adresserum på sit eget lokalnet, dvs. nogle adresserum er
forbeholdt ”private”, en oversigt findes her:
Side 55
TDC/YouSee anvender typisk adresserummet ”192.168.0.0”, hvilket betyder at man som privatperson har
fra 192.168.0.2 til 192.168.0.254 som adresserum, 192.168.0.1 er typisk routerens adresse og
192.168.0.255 er reserveret
```
Som det ses ovenfor, kan et IP adresserum angives som ”192.168.0.0/24”, dette betyder at 24 bit (3
```
```
oktetter) er netværksadressen og de sidste 8 er så host adresser. Adresserummet 192.168.0.0 til
```
192.168.0.255, tidligere blev dette kaldet en klasse C adresse, men det anvendes ikke så ofte mere.
”/x” kaldes også for subnetmask.
Side 56
Adressekonverteringen, dvs. fra den adresse man har på den offentlige del af sin router til den private del,
```
kaldes NAT (Network Address Translation) og er noget der kom til via en rfc da det begyndte at knibe med
```
IP version 4 adresser.
4.2.3 Port nummer
En IP-adresse identificerer hvem der kommunikeres med, port nummer identificerer hvilken type
```
kommunikation (protokol) der er tale om. port nummer er således utrolig vigtig og en del af IP pakkens
```
adresse. Port nummer kan også angives når man fx henvender sig til en web-server: 192.168.0.12:80 – her
er anført at port ”80” skal anvendes.
Ud fra et sikkerhedssynspunkt er port nummer overordentlig vigtig, anvendes typisk i konfigurering af
firewalls – dvs. hvilke protokoller der tillades inbound eller outbound, de vigtigste port nummer er
følgende:
Port 0 til 1023: Disse TCP/UDP-port numre betragtes som velkendte porte. Disse porte er tildelt til specifik
```
servertjeneste af Internet Assigned Numbers Authority (IANA). For eksempel bruges port 80 af webservere.
```
Port 1024 til 49151: Dette er porte, som en organisation, såsom applikationsudviklere, kan registrere hos
IAMA for at blive brugt til en bestemt tjeneste. Disse skal behandles som semi-reserverede.
Port 49152 til 65535: Disse er portnumre, der bruges af klientprogrammer, såsom en webbrowser. Når du
besøger et websted, vil din webbrowser tildele sessionen et portnummer inden for dette område. Som
applikationsudvikler kan du frit bruge enhver af disse porte.
Port 20 – FTP data
Port 21 – FTP kontrol
Port 22 – SSH
Port 23 – Telnet
Port 25 – SMTP
Port43 – Whois
Port 49 TACACS
Port 53 – DNS
Port 69 - tftp
Port 80 - HTTP
Port 123 – NTP
Port 143 IMAP4
Port 161 SNMP
Port 179 BGP
- + + + +
Side 57
En mere detaljeret oversigt findes her.
4.2.4 NAT
Omsætning mellem ens offentlige IP-adresse og ens private adresserum, sker vi routerfunktionen kaldet
```
NAT (Network Address Translation), se eventuelt mere her. NAT er noget der er kommet til som en IP-
```
funktion og var ikke tilgængelig i starten, der kan læses mere vedr. NAT her.
4.2.5 DHCP
```
Den router man har i sit netværk, har en vigtig funktion, kaldet DHCP (Dynamic Host Configuration
```
```
Protocol), denne funktion har til opgave at tildele IP-adresser til de enheder der anmoder om det på ens
```
lokalnet, der kan læses mere om DHCP her. Det kan være en sikkerhedsudfordring hvis der er flere DHCP
servere på lokalnettet, så en kriminel vil kunne udnytte dette til at tildele IP adresser til enheder som der
dermed ikke vil kunne kommunikeres til og med.
Når en enhed skal have tildelt en IP-adresse, sker det typisk når enheden tændes, der spørges med MAC
adressen om der findes en DHCP server, hvis ja anmodes om en IP-adresse og en sådan tildeles derefter af
```
DHCP funktionen (serveren) som normalt er en del af en router.
```
4.2.6 UDP/TCP
To vigtige områder som er interessante at kende
```
TCP (Transmission Control Protocol) er den pålidelige form for kommunikation, idet der for hver pakke sker
```
en synkronisering der bevirker at man kan være sikker på at pakken er kommet rigtig frem, ulempen er til
```
gengæld at TCP er langsom i forhold til UDP (User Datagram Protocol). Ved UDP sendes data af sted og der
```
håbes så på at de når frem uden problemer, anvend ofte i streaming af fx video, da sker der noget med en
pakke så kommer den næste sikkert korrekt frem, så når der kommer pixelering, kan det være dårlige UDP-
pakker. Men skal man være sikker, så skal den forbindelsesorienterede TCP-protokol anvendes og ikke den
datagram orienterede protokol anvendes.
Side 58
4.2.7 BGP
Border Gateway Protocol er den protokol der anvendes i internettet, en utrolig vigtig komponent når
trafikken skal routes rundt globalt. Er beskrevet her og findes også som rfc her.
Hvordan protokollen virker, skal ikke medtages her og skal blot nævnes for den overordnede forståelses
skyld.
4.3 Firewall og DMZ
Formålet med en firewall er at adskille trafikken mellem to netværk, ofte er denne adskillelse begrundet i
flere forhold fx:
- Regulere hvilken type af trafik der må komme hvorfra og hvortil
- Liste IP-adresser der må kommunikere
- Sikre at trafik på den ene net ikke flyder over i det andet net
Der findes forskellige typer af firewalls, opdelingen kan ofte være afhængig af hvilken leverandør man har
set på:
- Software FW, fx den man kender fra sin PC
- Hardware FW, en fysisk boks mellem to netværk
- Proxy FW, typisk den funktion der er bygget ind i en router
- Cloud FW, normalt det samme som en software FW, bare i skyen – måske på en selvstændig server
- Next-generation FW. En mere intelligent FW
Man taler også ofte om en ”menneskelig FW”, ja måske er det den vigtigste – at den enkelte medarbejder
er i stand til at beskytte sig selv og virksomheden mod Cyberangreb.
En firewall håndterer hver pakke for sig selv, dvs. en IP-pakke analyseres og baseret på regler tages der
stilling til hvad der skal ske, skal pakken skrottes eller sendes videre. Visse firewalltyper kan analysere den
enkelte pakke endnu dybere, kaldes derfor ofte deep package inspection, en funktion der bl.a. er knyttet til
”intrusion detection”.
Side 59
Som oftest er router og firewall bygget sammen, et typisk hjemmenetværk:
I en virksomhed, der har behov for at kunder får data fra virksomheden, har man ofte indrettet hvad der
```
kaldes et DMZ (Demilitariseret Zone), arkitekturen ser typisk således ud:
```
Formålet er at sikre at de kunder der, via internet, har brug for data kun kommer ind i DMZ, mn vil så som
oftest løbende skulle opdatere data på fx webserver fra den interne database. DMZ er en meget sikker
metode og anbefales.
Generelt kan man sige at ingen trafik fra internet bør komme længere ind i virksomhedens net end
nødvendig, der kan derfor udmærket etableres flere DMZ’er. Som eksempel kunne et kunde WiFi og IoT
enheder være på hvert sit DMZ.
Der findes en lang række Firewall typer på markedet, nogle ganske avancerede og som det kræver en
dybgående viden for at installerer og drifte:
Side 60
Type Anvendelse Begrænsninger
Pakkefiltrering Den mest anvendte, er installeret
som standard i næsten alle
routere
Ikke i stand til at inspicere
```
indholdet af pakkerne (dvs. ingen
```
dybdegående analyse af
applikationstransaktioner eller
```
data), hvilket gør den sårbar over
```
for visse angreb som f.eks. IP-
spoofing
Stateful Inspection FW Kaldes også en dynamisk FW.
Tillader fx kun pakker der er en
del af en eksisterende session
Mere kompleks og
ressourcekrævende end
pakkefiltrering, men stadig ikke i
stand til at analysere indholdet af
applikationstransaktioner.
Proxy FW Et mellemled mellem bruger og
ressourcer som der ønskes
adgang til. Mulighed for mere
dyberegående inspektion
Kan introducere forsinkelse og er
mere ressourcekrævende. Kan
kun arbejde med specifikke
applikationer.
Next Gen FW Kombinerer forskellige funktion,
kan lave pakke inspektion i
dybden, malware analyse og IPS
mv.
Kan være dyrere og mere
kompleks at implementere og
administrere.
Web App FW Primært til beskyttelse af WEB
applikationer, mod fx SQL
injection, XSS og lign
Kan være målrettet af
avancerede angreb, og kræver
ofte løbende justering af regler
for at være effektiv.
Circuit level Gateway Overvåger transportlager,
anvendes typisk i forbindelse
med VPN
Ingen dybdegående inspektion af
applikationens indhold og
risikerer at tillade visse angreb.
Hybrid FW Kombination af ovenstående Er dyrere og mere kompleks at
implementere og administrere.
4.3.1 Et praktisk eksempel
Mange hjemmenetværk er i realiteten ikke beskyttet bedre end mindre virksomheder, det der også kaldes
SOHO markedet, nok lidt mindre end SMV-markedet. Firewall typen er typisk almindelig pakkefiltrering.
Men der kan være en simpel grad af pakkeinspektion.
Med en internetforbindelse følger ofte en router med indbygget firewall, som oftest har man kun
begrænset indflydelse på hvordan den sættes op – man skal da også være kyndig hvis man ønsker at ændre
i standardkonfigurationen.
I sin router/firewall kan man fx lave en fast routing til en bestemt adresse – fx at alt SMTP-trafik kun går til
en mailserver.
Eksempel fra personligt netværk:
Side 61
Dertil komme så mulighederne for fx at sige at fx FTP-trafik ikke må går ind eller ud af FW. Man kan fx også
blokerer for IP version 6 trafik.
Side 62
Router/firewall trafik eksempel:
IP-adresse filtre
I professionelle firewalls kan der opsættes IP-adresse filtre, dvs. man kan styre at en bestemt IP-adresse
kun må kommunikere med et/flere andre IP-adresser.
Det forudsætter at man anvender statistiske IP-adresser
4.3.2 Intrusion detection
Angreb udefra kaldes ”Intrusion”, det er derfor interessant at have mulighed for at detekterer og bedre
blokerer og derved forebygge at et angreb udefra forvolder skade på virksomhedens infrastruktur. Denne
typer af funktionalitet kan være implementeret på forskellige enheder:
• Firewalls
• Specifikke netværksenheder
• Servere
Side 63
Det kan være den enkelte beskyttelsesenhed der giver en alarm, men det kan også være kombinationer af
hændelser der bevirker at en indtrængning er opdaget, derfor er det vigtig at enderne sender resultater til
et log management system, her kan der så laves scenarier der kan advarer og eventuel blokerer en
indtrængning. Systemer der detekterer kaldes normalt:
```
IPS: Intrusion Prevention System
```
```
IDS: Intrusion Detecting System
```
Flere log management systemer kan have preinstallerede scenarier der kan interface til bestemte IPS/IDS-
systemer-
4.3.3 Sårbarhedsscanning og PenTest
```
Sårbarhedsscanning og penetration testing (PenTest) er to discipliner som skal klarlægge om udstyr eller
```
adgange er sikret som man forventer, men man kan naturligvis kun teste for det som man kender. Det er et
område som både interesserer den virksomhed der leverer IT/OT udstyr, samt større virksomheder som
selv ønsker en uafhængig vurdering af hvor beskyttet de er. Inden man tillader eksterne at udføre fx en
PenTest, så skal man sikre sig at det er en troværdig partner, derfor er det anbefalingen at anvende firmaer
som er akkrediteret til dette formål. Er der ”blot” tale om sen sårbarhedsscanning, så kan man i realiteten
får det udført med software internt i virksomheden, eller købe det som en online udbyder. Uanset hvad
```
skal man have etableret en aftale og der er normalt tale om at der underskrives en NDA (Non Disclosure
```
```
Agreement) der sikre at det firma der fx laver en PenTest ikke anvender informationerne overfor andre.
```
Både PenTest og sårbarhedsscanning kan også bruges for at analyserer om man har et beredskab der vil
```
opdage det, dette er typisk rettet mod større organisationer der fx en SOC selv (Security Operation Center),
```
den enhed der er så laver en test kaldes et ”Red team”, SOC kaldes så ”Blue Team”.
4.4 Netværksarkitektur
Som det er nævnt ovenfor, anvendes DMZ arkitekturen som en måde hvorpå man sikre at man ikke udefra
kan komme ind til selve kernen i virksomheden, ved at kopiere relevante data ud til fx den webserver som
kunderne anvender.
Internt i virksomheden er det også vigtig at adskille fx et administrativt og et produktionsnet. Dette kan ske
på forskellig vis, men ofte er der etableret, ofte to, firewalls mellem de to netværk
Side 64
Firewall mod produktionsnettet kan konfigureres med de samme overvejelser som firewall mod
internettet, men derved har man fx et større vished for at malware ikke spreder sig mellem de to netværk.
Er man en stor virksomhed har man typisk mange firewalls, disse kan været etableret i software og
anvendes i forbindelse med en logisk, i modsætning til en fysisk, opdeling af sit interne netværk. Denne
virtuelle opdeling kaldes typisk VRF-opdeling – virtuel routing på det samme fysiske netværk. VRF realiseres
i den fysiske router. VRF er ikke det sammen som VLAN, men formålet kan være det samme – at sikre en
logisk separering. Subnet, VRF og VLAN er tre forskellige teknologier hvormed man kan adskille trafik, VRF-
teknologien er fremhævet som den sikreste og den der typisk anvendes i større virksomheder hvor der ikke
etableres en fysisk adskillelse af netværk.
4.4.1 WiFi
WiFi, også kendt som 802.11 standarden anvender de to nederste lag af OSI-modellen, 802.11 standarden,
er en familie af standarder hvor de mest kendte er følgende:
Som det fremgår, kan 5Ghz område anvendes for de standarder der er kommet til senest, 5Ghz båndet har
den fordel at der oftest ikke er så meget trafik og dermed forstyrrelser på den enkelte kanal. Til gengæld er
rækkevidden lidt kortere.
Side 65
Set med sikkerhedsbriller er krypteringen i det trådløse net vigtig, her findes der forskellige metoder
I praksis anvendes WEP ikke mere og anbefales ikke da den nemmere kan brydes, fordelen ved de
dynamiske keys er at de skifter ofte og de er beregnet til at skifte så ofte at man ikke kan nå, med
avancerede hjælpemidler, at dekode dem. Når Cuantum Computing bliver en realitet for alvor, ja så bliver
det en anden sag.
Et er kryptering i luften mellem udbyder og klienten, men hvad med udbyderen – udbydes der fx et falsk
SSID?, eller hvad med forbindelsen fra WiFi hotspot til andre netværksområder, De kendte mulighederne
følgende:
• Der opsættes et falsk HotSpot, dem der forbinder sig bliver så aflyttet, også selvom der i ”luften” er
forhandlet en god kryptringsprotokol
• Der aflyttes mellem WiFi HotSpot og til det øvrige netværksudstyr, her sker kommunikationen
ukrypteret, dette kaldes normalt ”Man-n-the-middel attack”, her kan fx aflyttes brugernavne og
kodeord.
• En scanner opsamler store mængder datamængder, bruger så lang tid på at dekode
kommunikation og finde brugernavne og kodeord
• Dårlig konfigureret WiFi HotSpot, fx kan standard admin kodeordet ikke være ændret, eller det er
meget simpelt og sikkert aldrig ændret
Eksempler på hvad man kan gøre
• Brugen af MFA, bevirker at selvom dit brugernavn og kodeord er gættet, ja så kan det
ikke/vanskelig udnyttes da det kræver ”Something you have”.
• Brugen af en passwordmanager kan reducere risici, da det er vanskeligere at gætte fx et 12 tegns
autogenereret kodeord.
• End2End kryptering, brugen af VPN til den virksomhed man ønsker forbindelse til, eller generelt at
anvende en VPN også privat – VPN-forbindelse til et sikkert sted.
Hvad kan man gøre FØR man forbinder sig til WiFi HotSpot
• Start VPN
• Clear browser
Side 66
• Sikre at Malware beskyttelse er opdateret og aktiv
• Stop eventuelle kørende applikationer som du ikke skal anvende
• Sluk for bluetooth
• Sluk for auto-connect.
• Sikre at MFA anvendes ved logon til slut destination
4.4.2 Øvrige netværkskomponenter
Der findes andre netværkskomponenter udover routere og firewalls, som det er beskrevet kan de to
enheder sagtens være i samme fysiske boks
I praksis består et netværk af en række enheder der via decentrale og centrale komponenter er knyttet
sammen til et fladt netværk, eller netværket kan være segmenteret. Til det formål anvendes som oftest
switches, disse kan være administrerbare eller helt passive. De fleste anvender switches der kan
administreres, så man fx kan åbne og lukke for porte centralt – fra en network management system. En
switches kan købes I næsten alle prisklasser, fra nogle få hundrede kroner og op til mange tusinde, bl.a.
afhængig af antal porte og administrationsmuligheder. Som eksempel er her en professionel Cisco
```
switches:
```
Et switches kaldes som oftest en ”Lag 2 switches”, det betyder at den har styr på hvilken MAC adresse der
er knyttet til hvilken Ethernet port. Det har den store fordel at er der to enheder der skal kommunikere på
samme switch, så kan kommunikationen holdes lokalt og ikke sendes ud til hele netværket.
En HUB har typisk den sammen funktion som en switches, men er mindre intelligent og holder ikke styr på
MAC adresser, en HUB er også typisk billigere end en switches, bruges ikke så meget mere i praksis.
En Bridge kan som en switches holde styr på trafikken og anvendes for at sikre opdeling af trafikken, men i
praksis er det switches der anvendes.
En netværksarkitektur kan derfor se således ud:
Side 67
Af andre komponenter kan naturligvis nævnes forskellige server typer, heraf kan nogle have flere
netværkskort og i realiteten opfattes som fx en firewall eller en router, tidligere er det bl.a. nævnt som en
”software firewall”-
Tegningen ovenfor illustrere også at der kan skabes redundans i form af dublering, helt fra ISP niveau og ud
til den enkelte switch.
VPN-server
Anvender man en VPN-klient, skal man også have en VPN server i den anden ende, der er et stort udbud af
VPN-tjenester, de fleste anvendes typisk for at få en given IP-adresse – fx en IP adresse der er i Danmark.
Det er vanskeligt at afgøre om disse VPN-tjenester er ok at anvende som privatperson til almindelige
formål, men flere af dem man betaler for er givetvis ganske ok og kan anvendes i forbindelse med
Side 68
offentlige HotSpot som nævnt tidligere. Er man virksomhed, så skal man have en VPN-server, hvor
brugernes VPN-klienter kan forbinde sig til, der skal konfigureres korrekt og lign. VPN-servere er ofte
implementeret i routere og/eller selvstændig hardware, Har man mod på at opsætte en VPN server privat,
så skal man i første omgang sikre sig at man har en router som man har adgang til og som tillader
opsætning af VPN. OpenVPN er typisk anvendt i disse situationer, der findes en række tutorials der kan
hjælpe med opsætning og konfigurering.
Alternativt kan man selv købe en router der indeholder VPN server funktionalitet og så sikre sig at man har
en ISP router der kan sættes i ”bridge mode”, derved sikre man sig at NAT funktionaliteten i ISP routeren
ikke laver forstyrrelser.
4.5 Log Management
Logning har en stor betydning for at man reaktivt kan finde ud af hvad der er sket, bruges aktivt ved
incidents og når der skal fejlfindes. Logning er også med fremkomsten af GDPR blevet mere almindelig, nu
er det ikke kun noget som en IT-afdeling skal bruge penge på, nu er det også et krav set i en persondata
sammenhæng.
I rigtig mange virksomheder logges der enorme mængder af data uden at de bruges til noget, man skl
derfor gøre sig klart indledningsvis, hvad man har tænkt at bruge loggene til. Dette kan ske i en dialog med
forretningen, kan være lovbestemt eller fordi man som IT-afdeling ønsker at holde styr på noget bestemt.
Det er typisk svært for forretningen af komme op med ideer til scenarier som kunne være interessante at
holde øje med, men det kunne fx være:
• Er der en kundeservice medarbejder der mere en X gange i døgnet har set på en kundes fortrolige
data?
• Er der en salgsperson som downloader store mængder kunde data?
• Hvad laver en opsagt medarbejder de sidste dage?
Hvis der med log management detekteres at et af ovenstående scenarier bliver til virkelighed, ja så skal log
management systemet sende en besked til xyz.
Men logs kan også anvendes meget mere trivielt, fx hole styr på diskforbrug og lign. Ser man på hvad der
står i ISO27001:
Dvs. ganske bredt og som er detaljeret i ISO27002. Overordnet siger ISO27002 om logning:
Side 69
Som udgangspunkt samles der hændelser, også kaldet events, sammen – disse siger som udgangspunkt
intet, det kræver som i mange andre sammenhænge at hændelserne granskes og bliver til information der
så igen måske kan/vil blive til incidents.
Man skal huske at der også kan være tale om fysiske hændelser, fx logs fra dørsystemer, her kunne det fx
være interessant har holde styr på hvem der gik ind af en bestemt dør efter klokken 20 aften?
IP-standarden indeholder noget der kaldes ”Syslog” det er en standardiseret måde at overføre logs til et log
management system på, i nærmest realtid. Modsætningen hertil er at overføre en logfil et antal gange i
døgnet med FTP eller SFTP. Der kan læses mere om Syslog her.
Side 70
Forensics
En disciplin for sig selv, hvor logmanagement er en rigtig vigtig komponent, herunder at man kan bevise at
der ikke er manipuleret med data. Dette er overordentlig vigtig i fx en retssag. Forensics kompetencer er
noget de færreste virksomheder har – her kan man have aftaler med konsulenthuse, der fx. Kan rykke ud til
ens virksomhed ved større hændelser for at indsamle beviser.
Dashboard
Et log management system har typisk et række scenarier som det pr. automatik holder øje med, dertil
kommer at man så selv kan danne scenarier via forskellige mere eller mindre komplicerede metoder. Et log
management system har typisk også et Dashboard hvor man grafisk kan få et overblik over status og hvad
der sker lige her og nu. Som eksempel på et Dashboard er her:
Der findes et utal af eksempler som er gode inspirationskilder, kunsten er så at man ikke får så mange
grafer på skærmen at man ikke får øje på det som man egentlig er interesseret i.
4.6 IoT
”Internet of things”, set med sikkerhedsbriller er der i realiteten ikke noget nyt, det handler om
fortrolighed, integritet og tilgængelighed – de tre grundlæggende begreber som blev gennemgået i modul
1. Men da IoT enheder som oftest er små enheder med et minimalt energiforbrug er det naturligvis ikke så
nemt at beskytte med avanceret software. Mange IoT enhed har ingen eller blot et lille batteri, måske
anvendes ”Energy Harvesting” som metode til at skabe strøm. IoT enheder kan kaldes/styre via Push/Pull
metoden, dvs. enten skubber man en kommando ud og man får et svar/status eller IoT enheden svare selv
fx. Hvert 5 minut. Begrebet dækker overalt alt fra smarte enheder man har i sit hjem, til hele byer – det der
kaldes ”Intelligente byer”, det er nærmest kun fantasien der sætter grænserne.
I 2021 blev der lavet en opgørelse der vist at der var 21.7 milliarder forbundne enheder, heraf blev 11.7
milliarder karakteriseret som IoT enheder. Eksempler på IoT enheder:
Side 71
Indenfor sundhedsområdet er der sket en revolution af IoT enheder og der forventes endnu mere. Men
også i mange andre sektorer forventes der endnu flere enheder. Som det vises nedenfor, forventes en
eksplosion i antal IoT enheder indenfor alle områder. Dette kan bevirke en lang række økonomisk fordele
bl.a. gennem automatisering indenfor:
• Industri
• Offentlig virksomhed
• Private hjem
Data til/fra IoT enheder samles lokalt eller i en cloud løsning, ofte har hver IoT familie sit eget
styringssystem, for private er Philips HUE meget anvendt, her samles enhederne lokalt og styringen sker via
en APP som igen kommunikerer med en cloud service. Ikea har også et stigende antale IoT enheder, så det
breder sig i alle segmenter
Der findes flere og flere fælles kommunikationsstandarder, men stadig er mange helt specifikke, bland de
mest kendt fælles standarder er:
• Zigbee
• Z-Wave
• Matter
• BT
• WiFi
• 4G/5G
Matter ser ud til at vinde mere og mere indpas, standarderne ovenfor tager som oftest højde for de tre
grundbegreber indenfor sikkerhed, CIA. Interessant video her. Løsningen der peges på er PKI, Public Key
Infrastructure, dvs. anvendelse af digital signatur i praksis. Mere herom under afsnittet kryptering
Der sker en enorm vækst af IoT enheder:
Side 72
```
Kilde: Byggebranche
```
Som ved log management systemer, er der også indenfor IoT management systemer en række proprietær
og open source-systemer. Bland de kendte Open Source-systemer er ”Home Assistant” meget populær
blandt private brugere, her kan man samle stort set alle typer af systemers logs, eksempel på integrationer:
Hver enhed kan så have en række sensorer, her et eksempel fra en NAS server:
Side 73
Man kan så lave DashBoads, eksempel:
Side 74
Samt lave et utal af automatiseringer.
IoT enheder indeholder som nævnt en række sikkerhedsudfordringer, her skal nævnes:
• Sikker krypteret kommunikation mellem enhed og ”central” og mellem enhederne selv.
• Autentifikation og Authorization, hvem er det er beder om data og hvilke rettigheder har de, må
man fx lave en software opdatering, også kaldet OTA. Et af de klassiske eksempler er adgang til små
kameraer som man måtte have i hjemmet eller på arbejdspladsen.
• Kan man stole på de softwareopdateringer, der muligvis kommer
• Er det data der ligger i cloud, hvem har så adgang til disse og hvornår
• Ofte er IoT enheder fordelt over et stort område, så der kan være problemer med tilgængeligheden
og de problemer det giver med manglende opdateringer
• Redundans ved fx industrisystemer
Men IoT er et område i eksplosion, her vil bl.a. 5G teknologien skubbe til udviklingen og i den anden ende
vil der komme et utal af meget simple enheder der fx kan give besked når skraldespanden er 75% fuld og
måske få sin energi dertil via skraldespandens låg når der åbnes og lukkes.
Industrirobotter og selvkørende biler er også områder der forventes meget af. Men et af problemenerne er
ofte at en virksomhed, og private, reelt ikke ved hvilke enheder der er på netværket – i praksis kun gener til
de enheder som administreres.
Side 75
Dertil kommer at nogle enheder anvender 4G/5G til kommunikation – virksomheden har derfor som oftest
ikke har et overblik over hvilke enheder der kommunikerer ind/ud af virksomheden og måske heller ikke
hvilke data det handler om.
En af de store udfordringer for IoT er at skaffe energi til alle de decentrale nheder, løses bl.a. gennem
Energy Harvesting, typisk gennem sol eller bevægelse.
4.7 SCADA og OT
SCADA betyder: ”Supervisory control and data acquisition”, typisk et software lag der ligger oven på
operativsystem og som gør det nemt at programmere en maskine eller et system, anvendes meget i
industrien til styring og administration af maskiner, er på sikkerhedsområdet berygtet for at stå åbent på
internet og beskyttet i meget ringe grad.
OT betyder: Operationel Teknologi, i praksis bare et andet ord for SCADA – bare et mere moderne ord som
også dækker PLC’er. Man kan tal helt generelt om OT, som så kan være:
• En fabrik
• I et vandværk
• Vindmøller
• Kraftvarmeværker
• Renseanlæg
• Svømmehal
• Hospitalsenheder
• Centrallager
• Atomkraftværk
• Facility management
Eller man kan tale om det enkelte OT-system, begge dele har betegnelsen ”OT Teknologi”.
SCADA/OT, herefter kaldet OT, har tidligere været typisk ”stand-alone” systemer, men indgår nu i
virksomhedens produktionsnet, men kan ofte være mindre sikret end IT-systemer, bl.a. fordi kulturen har
været at det var selvstændige systemer som kun blev betjent fysisk og ikke via et netværk. Det betyder
derfor at OT-systemer har de samme sikkerhedsudfordringer som IT-systemer. Moderne teknologi har ofte
dele i cloud, det kan for OT-systemer betyde at kontrollen med fx en industrirobot kan ske helt eller delvis
via en cloud service, dette udgør naturligvis nogle yderligere risici – men også fordele.
OT-systemer er oftest medtaget under begrebet ”Edge-Computing”, dvs. systemer der befinder sig tæt på
den fysiske verden.
Side 76
Men hvad er der specielt ved OT? – meget typisk er oppetidskravene meget højere end ved IT. OT er
styrende for produktionen og i mange virksomheder er produktionen 24/7, det betyder at man ikke ”bare”
kan tage systemer ud af drift, som man typisk kan ved IT.
Disse overvejelser skal bygges ind i arkitekturen og stiller også store krav til sikkerhed, fx i forbindelse med
opdateringer i forbindelse med opdagede sårbarheder.
Ser man på virksomheden som en samlet enhed, anvendes ofte denne pyramidemodel:
```
Som ved IT-sikkerhed (bl.a. ISO27001/2) findes der også indenfor OT sikkerhedsstandarder, typisk refereres
```
der til IEC62443, denne anbefaler følgende sikkerhedsarkitektur:
Side 77
Helt klassisk sikkerhedsarkitektur, at de enkelte lag fra pyramidemodellen er adskilt, så man bl.a. kan undgå
at incidents kan sprede sig fra det ene lag til det andet – eller i det mindste gøre hvad man kan for at sikre
lagene. Også her er det naturligvis vigtig at starte med en risikoanalyse, hvad er det for trusler man tænker
man kan blive udsat for og hvilke kan man fx godt leve med.
NIS2 direktivet har også en betydning for OT-teknologi, mange virksomheder vil sikkert tænke at NIS2 det
kun er IT-rettet, men nej det er ikke tilfældet. Alene den overordnede direktivtekst, peger tydeligt også på
OT-teknologi:
Et oplagt spørgsmål er: Dækker virksomhedens sikkerhedspolitik også OT-området? – hvad med
Governance, er det klart hvem der har ansvaret for hvad i relation til OT-sikkerhed?
4.8 Kryptering
```
Som beskrevet under IoT er PKI (Public Key Infrastructure) en af mulighederne for at sikre IoT-enheder mod
```
Cybersikkerhedshændelser. Ordet infrastruktur dækker over at der er en række ting der skal være på plads
Side 78
for at sikre administration af digitale signaturer og sikre kryptering. I praksis anvendes PKI derfor både til at
sikre fortrolighed, integritet og authentication.
Så basis i PKI er digital signatur, ikke for at underkende det apparat der er udenom de basale elementer.
Der skal ikke i disse noter beskrives PKI i detaljer, men det er vigtig at være klar over forskellen mellem:
• Privat digital nøgle
• Offentlig digital nøgle
Denne type kryptering kaldes ”Asymmetric key Encryption”. Løser flere problemer bl.a. at en digital nøgle
har en bestemt levetid, i praksis betyder det at sender og modtager kan opdatere keys uden at det kan
aflyttes og uden at brugerne/systemer har kendskab til hvilken digital nøgle der anvendes lige nu. I den
asymetriske krypterings infrastruktur er der altid en privat og en offentlig nøgle, som navnet antyder er den
offentlige nøgle tilgængelig for alle, hvorimod den private er personlig for system eller person. De to nøgler
er produceret samtidig og er linket sammen på en måde der matematisk har sikre at den private nøgle ikke
kan udledes af den offentlige nøgle. Eksempel:
Da nøglerne hænger sammen, så kan ”Plain Text” krypteres med den offentlige tilgængelige nøgle sikkert,
da ”Cypher Text” kun kan dekrypteres med den private nøgle. De digitale nøglers længde er dog stadig
vigtig og der findes standarder indenfor dette område, fx AES – et kompliceret matematisk område, DES er
en anden standard. I praksis anvendes der nøglelængder helt op til 256 bits, hvilket så i praksis giver 2256
mulige nøgle kombinationer.
Hvis man nu vender det om, så sender krypterer med sin privat nøgle og sender en besked til modtager, så
kan alle med den offentlige nøgle dekode og derved er der ingen fortrolighed forbundet med
kommunikationen, men til gengæld er der garanti for hvem der er afsenderen, hvilket også kan være
ganske vigtig og har stor anvendelse. Kaldes også for ”Non repudiation”, kendes også fra MIT-ID når man fx
skal underskrive et dokument – fx en ansættelsesaftale.
Side 79
Hvad så hvis man først kryptere med sig private nøgle og derefter modtagerens offentlige nøgle, så skal
modtageren først laven en dekryptering med sig egen private nøgle – derefter dekryptere med afsenderes
offentlige nøgle, nu er der så opnået to fordele:
1. ”Plain text” kan læses, fortrolighed og integritet er sikret
2. Modtageren er sikker på at ”Plain Text” er fra afsender
Hvis så nøglerne skiftes hurtigere end en ”man in the middel” kan dekode ”Plain Text”, ja så er
kommunikationen sikret.
Mere simpel anvendelse af kryptering
Kryptering anvender, som beskrevet, altid en digital nøgle, denne anvendes fx til at ændre ”Plaintext” til
”Cyphertext” – som eksempel kan nævnes krypterings af Microsoft Office dokumenter, ZIP filer og hele
harddiske, i disse eksempler er der tale om kryptering med en fast og statisk digital nøgle. Værdien af
denne form for kryptering er derfor stærk afhængig af denne gigitale nøgles længde og kompleksitet – helt
analog med kodeord. Kaldes for ”Symmetric key Encryption”
Som nævnt er nøglerne vigtige i forbindelse med kryptering, men algoritmerne der anvendes er naturligvis
også ganske vigtige, typisk anvendes SHA-1 eller SHA-2, kaldes også for Hashing
For at få en privat og offentlig nøgle som er officiel, skal have udstedt et digitalt certifikat, et sådant får man
via en udsteder – kaldet ”CA” – Certificate Authority, for at få certifikatet skal man godtgøre hvem man er
og hvorfor. Alle kan ansøge en CA og få udstedt et digitalt certifikat og dermed få en privat og en offentlig
nøgle. Vil man kommunikere med en enhed med anvendelsen af PKI, så kan man se hvem der er udsteder
af certifikatet og man kan se hvornår det udløber. Det er nok så vigtigt at holde styr på udløbet, for et
udløbet certifikat er ikke længere gyldig, kan i praksis bl.a. give meddelelsen ”din forbindelse er ikke privat”,
Side 80
eller man kan slet ikke tilgå WEB stedet længere, WEB steder anvender typisk ”SSL” – her er
gyldighedsperioden for certifikater 27 måneder inden de skal genbekræftes. Der findes systemer der
automatisk kan holde styr på en virksomheds officielle og private certifikater.
SSL anvendes til at skabe en sikker forbindelse mellem en WEB server og en WEB browser.
4.9 Cloud
Cloud computing har gennemgået en enorm udvikling og anvendes i dag af stort set alle, både
virksomheder og private, alene at man har en gmail, hotmail konto gør at man er anvender af cloud service
– det at have en smart phone gør at man anvender cloud services.
De fleste firmaer er i den samme situation, følgende tre typer af cloud services er de typiske
```
SaaS (Software as a Service)
```
Adgang til en applikation er SaaS, således noget vi alle anvender i praksis, som oftest er disse services
betinget af at man har tegnet et abonnement, Office365 er et godt eksempel, men der kan også være tale
om gratis services, fx gmail.
```
PaaS (Platform as a Service)
```
Anvendes fx. i udviklings sammenhæng, her kan PaaS levere et komplet udviklingsmiljø, kan fx inkluderer
database services, holde styr på versioner, programmeringssprog mv.
```
IaaS (Infrastructure as a Service)
```
Kan fx. være server, fysiske eller virtuelle, med et bestemt operativsystem, storage eller databaser – dvs.
helt grundlæggende infrastruktur komponenter som man så har valgt at have som en cloud service.
Dertil komme at cloud services ofte opdeles i tre typer:
Public Cloud
Cloud service man deler med andre, men ens data holdes typisk separat.
Privat Cloud
At man har sin hel egen cloud service, både applikation og data er helt sepereret fra andre kunders
Hybrid Cloud
At man har fx en applikation som en cloud service, men data lokalt hos en selv.
De fleste cloud services kan man ikke ændre på, man anvender dem som de er tiltænkt. Men der er cloud
services som kan tilrettes ens behov, fx de processer man har i virksomheden. Som eksempel herpå er det
meget anvendte ServiceNow.
Der er en række helt oplagte fordele ved cloud servces:
• Pris
• Skalerbarhed
• Datasikkerhed
• Mobilitet
• Disaster Recovery
```
• I kontrol (patching, backup, scanning ……)
```
Side 81
Alle større cloud udbydere er da også sikkerheds certificeret på en lang række områder, se fx AWS og
Microsoft Axure. I praksis har disse store cloud service udbydere derfor en lang række sikkerheds
certifikater som ingen almindelige virksomheder vil kunne opnå i praksis:
Så er der grund til at være bekymret for sikkerheden i relation til cloud services?
Der kan være juridiske overvejelser, er det fx lovmæssigt sikret at data skal være i Danmark, dette er
nærmere beskrevet her. Tidligere kaldes det ”Krigsreglen”, nu er det en del af den almindelige
databeskyttelseslovs regler om beskyttelse og op til individuel forhandling med Justitsministeriet.
Udgangspunkt er statens og borgernes sikkerhed, følgende systemer er af Justitsministeriet beslutte skal
blive i Danmark.
• Digital Post
• MitID
• Nemlog-in 3
• DeMars
• Statens Lønløsning
Af andre overvejelser skal nævnes de klassiske ”CIA-overvejelserne” samt tror man på at cloud
```
leverandøren overlever på den lange bane, har man en exit plan, hvor gemmes data (også backup), er der
```
GDPR-udfordringer, hvordan er kommunikationen sikret osv.
Markedet har endnu til gode at se en af de store cloududbydere gå konkurs, hvilket forhåbentlig aldrig sker.
Det danske Center for Cybersikkerhed har lavet en udmærket vejledning, kan findes her. Er også at finde i
fællesmappen
Skal man starte med at anvende cloud services, skal man naturligvis starte med en risikoanalyse, en sådan
risikoanalyse skal sammenholdes med de risici man vil have ved at have systemerne selv. De store
Side 82
cloududbydere er meget opmærksomme på sikkerheden, de kan ikke holde til at blive identificeret med
dårlig sikkerhed, en større hændelse kunne bevirke at kunderne flygter.
Mere om cloud leverandører i modul 6 ”Leverandørstyring”
4.10 Zero-trust
Principperne om zero-trust bygger grundlæggende på at man ikke kan stole på sine perimetre grænser,
brugerne er både lokale og måske globale, applikationer er i cloud og nogle fx produktionsmaskiner styres
og overvåges et eller andet sted i verden. Så hvor er virksomhedens grænser i virkeligheden og hvordan
kontrollerer man disse med FW osv. – man kan konkludere: Denne virkelighed er der i mange
virksomheder.
Det handler derfor om at beskytte hver enkelt asset og sikre sig at autentifikation og autorisation ikke gives
permanent, men løbende skal gengodkendes og valideres. I praksis kan assets ”pakkes ind” i grupper.
Zero-trust princippet:
• Alle kommunikationskanaler skal sikre, fx via kryptering
• Klassifikation af assets
• Anvend kraftig segmentering af netværk, også kaldt mikrosegmentering – ultimativt et segment pr.
asset
• Adgang gives på ”pr session” basis. Dvs. ikke en permanent adgang.
• Stor grad af overvågning
• Sikre former for autentifikation og autorisation samt MFA
NIST har i sit udgivet disse principper publikationen i ”NIST SP.800-207”, findes i fællesarkivet
Side 83
Modul 5: Internetsikkerhed
Basal viden om Cybersikkerhed, inkludere noget om internetsikkerhed og de trusler der er relateret til
anvendelse af internet, men selvom det som oftest opfattes at de største trusler kommer fra internet, så er
forudsætningen for disse truslers indvirkning ofte den menneskelige indvirkning, at man fx klikker på en link
man ikke burde ms.
Dette er også medvirkende til at virksomhedernes awareness aktiviteter er i stærk stigning. Mod danske
SMV’er har Sydbank listet disse klassikere:
• Randsomware
• Faktura fup
• Compliance
I 2023 har PwC undersøgt danske private og offentliges forventninger til udviklingen indenfor cybertrusler,
resultatet siger en del om forventningerne:
Tilsvarende udgiver ENISA en årlig rapport om trusselsbilledet i Europa, kan hentes her.
Hovedkonklusionerne er:
Også her er Randsomware højt på listen, så det må være en risiko enhver virksomhed tager med i sin
overordnede risikoanalyse.
Men for at det kan bevirke et incident, så skal der mere til – den menneskelige faktor, som skrevet ovenfor
så er det som oftest et klik på et forkert link eller lignende det der er udslagsgivent. Vi er nok lidt for
tillidsfulde, for naive vil nogen måske sige, her i Skandinavien.
PwC har derudover en række interessante konklusioner, bl.a:
Side 84
Knap syv ud af ti danske virksomheder skruer op for
budgettet inden for cyber- og informationssikkerhed
over de kommende 12 måneder og ruster sig dermed
mod det aktuelt høje trusselsniveau fra cyberkriminalitet
Det er interessant at der i den grad er fokus på sikkerhed, det ser ud til at det for langt de fleste
virksomhedsejere er gået op for betydningen, tidligere har det været de store virksomheder som var
opmærksomme og som var villige til at øge sikkerhedsbudgetterne, men nu er SMV segmentet også
komme med.
Interessant er det derfor at:
Cybercrime Survey har igen i år bedt dansk erhvervsliv om at vurdere
hændelsesniveauet i deres organisation. Knap 45 % fortæller, at deres
organisation har oplevet mindst én sikkerhedshændelse i løbet af de seneste
```
12 måneder. Niveauet er fortsat højt, men er i år lidt lavere end i 2022 (51 %).
```
Det at der har været et mindre fald siden 2022, må antages at skyldes enden større investeringer,
tilfældigheder eller manglende lyst til at rapporterer.
I forbindelse med NIS2 bliver der et større krav omkring anmeldelse af hændelser antagelig via ”virk.dk”,
det bliver interessant at se på hvilken impact det får for undersøgelser som PwC’s.
IBM har i deres rapport ”X-Force Threat Intelligence Index 2023 konkluderet følgende:
Phishing was the top initial access vector:
Phishing remains the leading infection vector,
identified in 41% of incidents, followed by
exploitation of public-facing applications in 26%.
Infections by malicious macros have fallen out of
favor, likely due to Microsoft’s decision to block
macros by default. Malicious ISO and LNK files use
escalated as the primary tactic to deliver malware
through spam in 2022.
Phishing via service, er et udviklet kit som kan danne mails ud fra nogle parametre, kit kan købes billigt, kaldes også PhaaS
IBM-rapporten findes i fællesmappen.
Det siger noget om den menneskelige faktor og kalder derfor på et meget stort fokus på at sikre at
medarbejderne i virksomheden er veluddannet i emnet. Nogle tydelige og stærke Awareness kampagner.
En anerkendt måde, der kan medvirke til at sikre opmærksomheden på mistænkelige links i mails, er at
teste mails. Send fx en mail ud til medarbejderne der fortæller at de grundet en fantastisk omsætning i
seneste kvartal så er der en ekstra bonus på 1500 Kr., de skal blot oplyse navn, adresse og bankkonto. Så se
hvor mange der reelt afleverer oplysninger og brug dette som illustration i virksomheden for hvor godt
medarbejderne er klædt på. En sådan kampagne giver både indsigt og debat i virksomheden.
Man anvender ofte begrebet ”Den menneskelige firewall”
Side 85
Der findes en række udbydere der kan hjælpe med disse kampagner.
5.1 Trusselsbillede
For den enkelte virksomhed er det vanskeligt at afgøre hvilket trusselsbillede som virksomheden er
eksponeret overfor. For mange virksomheder er det derfor vigtig at søge inspiration fra forskellige kilder,
blandt disse kilder kan være:
Det nationale trusselsbillede
• Sektor trusselsbillede
• Samarbejdspartneres trusselsbillede
• Trusselsbillede fra interesseorganisationerne
• Trusselsbillede fra revisions- og konsulentvirksomheder
Som det fremgår, er der rigeligt med kilder, man skal da også bruge kilder med forsigtighed. Nogle kilder
kan have en interesse i at tegne et trusselsbillede der giver indkomst.
5.1.1 Det nationale trusselsbillede
```
Det nationale trusselsbillede leveres af CFCS (Center for Cybersikkerhed) og er ikke klassificeret, dvs.
```
tilgængelig via CFCS hjemmesiden under ”Cybertruslen”, se fx her. Publikationen findes i Canvas, den
overordnede vurdering for 2023 er følgende:
Truslen fra cyberspionage mod Danmark er MEGET HØJ. Truslen er koncentreret om udenrigs- og
sikkerhedspolitiske forhold såsom Arktis, NATO og EU, selvom også kritisk infrastruktur er udsat for
truslen.
Cyberspionage kan underminere danske interesser, både politisk, økonomisk og sikkerhedsmæssigt. Det
er sandsynligt, at fremmede stater benytter cyberspionage som forberedelse af destruktive cyberangreb.
Truslen fra cyberkriminalitet mod Danmark er fortsat MEGET HØJ. Velorganiserede ransomware-
grupper går efter alle dele af samfundet.
CFCS vurderer, at langt de fleste cyberkriminelle fortsat er økonomisk motiverede, arbejder
opportunistisk og er uafhængige af stater.
Truslen fra cyberaktivisme mod Danmark er HØJ. Det er sandsynligt, at danske virksomheder og
myndigheder vil blive ramt af aktivistiske cyberangreb på kort sigt. Pro-russiske cyberaktivister har et
højt aktivitetsniveau mod NATO-lande, herunder Danmark, og har i stigende grad formaliseret deres
angrebsmodus og forøget deres kapacitet.
Truslen fra destruktive cyberangreb er LAV. Det er mindre sandsynligt, at fremmede stater på
nuværende tidspunkt har til hensigt at udføre destruktive cyberangreb mod Danmark. CFCS vurderer
dog, at hackergrupper tilknyttet fremmede stater forbereder sig for at kunne udføre destruktive angreb
med kort varsel.
Side 86
Danske organisationer, der har aktiviteter i Ukraine eller leverer produkter og tjenester relateret til krigen
i Ukraine, kan være udsat for en højere risiko for at blive ramt af et destruktivt cyberangreb eller
følgevirkningerne af et angreb, der er rettet mod Ukraine.
Truslen fra cyberterror er INGEN. Militante ekstremister har kun begrænset hensigt og ingen kapacitet
til at udføre cyberangreb, der kan sidestilles med konventionel terror.
I rapporten er der yderligere detaljer der begrunder vurderingerne, skal man som virksomhed bruge
trusselsvurderingen aktivt, så skal man ned i det enkelte område og læse baggrunden.
Som eksempel kan man se på Cyberspionage, her er det primært Kina og Rusland der er fremhævet som
aktører indenfor dette område. Herunder at det ikke kun er kriminelle organisationer der er aktive, men
også staternes militære ressourcer der anvendes til spionage. Så er man leverandør til fx Forsvaret, er man
en samfunds kritisk virksomhed, så er det en risiko man bør inddrage
I rapporten er fx følgende fremhævet:
5.1.2 Sektor trusselsbillede
Center for Cybersikkerhed publicerer udover trusselsrapporter mod Danmark, også mere sektorspecifikke
trusselsrapporter, se her. Som eksempel ses der her på energisektoren, trusselsrapporten findes i Canvas.
Disse sektorspecifikke vurderinger er opbygget på samme måde som den nationale. For energisektoren er
følgende fremhævet:
Truslen fra cyberkriminalitet er MEGET HØJ. Den alvorligste trussel fra cyberkriminalitet kommer fra
ransomware-angreb, der løbende rammer virksomheder og underleverandører i sektoren. Presset på
virksomheder fra ransomware-angreb øges, hvis der er tvivl om, hvorvidt et angreb også kan ramme den
```
operative teknologi (OT).
```
Truslen fra cyberspionage er MEGET HØJ. Den vedvarende trussel udgår især fra Rusland og Kina og
fører løbende til cyberangreb mod danske mål. Energisektoren er et eftertragtet mål, både af civile og
militære årsager. CFCS vurderer, at Danmarks fortsatte førerposition i den grønne omstilling også vil
kunne drive truslen.
Truslen fra cyberaktivisme er HØJ. Truslen udgår særligt fra pro-russiske hackere, der har øget deres
aktivitetsniveau efter Ruslands invasion af Ukraine, og løbende rammer mål i Vesten – også i Danmark.
Truslen fra destruktive cyberangreb er LAV. Selvom stater, herunder Rusland, har kapaciteten til at
udføre destruktive cyberangreb mod Danmark, har de for nuværende ikke intentionen. Krigen i Ukraine
Side 87
har vist, at destruktive cyberangreb er blevet en del af moderne krigsførelse, og at energisektoren er et
prioriteret mål i en konfliktsituation.
Truslen fra cyberterror er INGEN.
Igen skal man ned under det enkelte punkt for at finde baggrunden for vurderingen. Energisektoren har
egen CERT som også laver en trusselsvurdering, et eksempel herpå findes i Canvas.
EnergiCERT anvender ”TLP protokollen”, en global måde at klassificere information på – dvs. en måde at
fortælle at en given information kun på ses/læses af en bestemt gruppe. TLP er beskrevet flere steder, bl.a.
```
som:
```
Trusselsbillede offentliggøres flere gange om året og er tilgængelig via hjemmesiden:
Side 88
Netop denne sektor var udsat for et større angreb som kunne være overordentlig kritisk.
Hændelsesrapporten opsummerer følgende:
Side 89
Angrebet skete i første omgang via en kritisk sårbarhed i en Zyxel ruter som CERT viste at man brugte i
mange medlemsvirksomheder som router/FW mod OT-systemer. Den 11. maj blev 11
medlemsvirksomheders FW overtaget og havde dermed adgang til kritisk infrastruktur. Incident skal ikke
beskrives yderligere her, men det er interessant læsning.
Konklusionen blev denne:
Side 90Side 91
5.2 Malware
Malware en fælles betegnelse, der dækker over ”ondsindet kode”.
Fjendtlig, ondsindet software/malware søger at invadere, beskadige eller deaktivere computere,
computersystemer, netværk, tablets og mobile enheder, ofte ved at tage delvis kontrol over en enheds
drift. Ligesom den menneskelige influenza forstyrrer den normal funktion.
Motiverne bag malware varierer. Malware kan handle om at tjene penge, sabotere en virksomheds evne til
at få arbejde udført, at lave en politisk udtalelse eller bare prale. Selvom malware ikke kan beskadige den
```
fysiske hardware i systemer eller netværksudstyr (med få undtagelse), kan malware stjæle, kryptere eller
```
slette en virksomheds data, ændre eller kapere computerfunktioner og spionere på din computeraktivitet
uden din viden eller tilladelse.
5.2.1 Malware typer
Der findes en række forskellige oversigter over Malware typer og deres funktioner, fx:
Forskellige typer Malware
Virus
Virus er en af de mest almindelige typer af malware til dato. Det er et program, der inficerer
en computer, lammer enheden for selv at replikker på systemet. Da vira er selvreplikkerende,
når de er installeret og kørt, kan de automatisk spredes fra en enhed til en anden på det
samme netværk uden menneskelig indgriben. Tidligere kaldet man det en orm når vira var
selvreplikkerende.
Trojan
En trojaner er en form for malware, der downloades fra internettet eller installeres af andre
ondsindede. Et eksempel på et bemærkelsesværdigt trojansk malwareangreb er Zeus Trojan,
der blev opdaget i 2007. Denne type malwareangreb stjal ikke kun klassificerede data, men
duplikerede også softwaren ved at implementere botnets for at fortsætte med at inficere
flere enheder og systemer.
Botnet
Botnets er grupper af enheder, der er inficeret med malware til at udføre en bestemt opgave.
Disse typer malware-bots kan bruges af ondsindede årsager, herunder som afsendelse af
spam-e-mails, phishing, smishing, lancering af DDoS-angreb eller distribution af malware.
Rootkit Rootkits er en slags malware skabt for at skjule sin tilstedeværelse i et computersystem. Detkan bruges til at få uautoriseret adgang til et system eller netværk.
Spyware Spyware er en type malware, der spionerer på en brugers computeraktivitet. Denne typemalware kan overvåge Et eksempel på spyware er en keylogger.
Adware Adware er en type software, der viser uønskede reklamer på din computer. Det kandistribueres via e-mail-vedhæftede filer, downloads og inficerede websteder.
Randsomware
Ransomware er malware, der krypterer et målrettet offers filer og låser adgangen til deres
computersystem. Denne type malware kræver en løsesum for at modtage en
dekrypteringsnøgle eller en anden adgangsmetode til at låse systemet op for at få adgang til
det igen. Ransomware-angreb har til formål at afpresse penge fra enkeltpersoner,
virksomheder og organisationer ved at holde information og systemer som gidsler.
```
Kilde: https://www.comptia.org/blog/7-most-common-types-of-malware
```
Side 92
Der er yderligere detaljer om hvert enkelt punkt at finde i fællesmappen til dette kursus, men generelt er
det et område hvor der løbende kommer nye ord til, dvs. nye typer. Fx Smishing, som i virkeligheden bare
er phishing via SMS.
Backdoors, er også en kendt sårbarhed, behøver ikke at være egentlig malware, men kan vær udviklerne
der har gemt at slette kode som blev anvendt i udvikling og test af softwaren.
5.2.2 Malware indgange
Som nævnt kommer malware ind i en virksomhed typisk via:
• Medarbejderne der klikker på noget bestemt
• Dårlig opdaterede eller konfigurerede systemer
• Installation af opdateringer med malware
Da kommunikation i en virksomhed som oftest indebærer internet aktivitet, er der en reel risiko for at
malware kommer ind på en eller anden måde.
5.2.3 Malware beskyttelse
Det er en større industri der lever af at sælge systemer til Malwarebeskyttelse og de fleste private personer
er da også klar over at det er noget man skal have installeret på ens private udstyr. Basalt set så udnytter
malware sårbarheder, eller skaber dem selv når først de er installeret.
Da Malware kan komme ind i virksomheden via forskellige kanaler, så kan man ikke bare installerer noget
SW og så dermed sige at alt er ok. Malware beskyttelse, ofte kaldet AntiVirus beskyttelse, testes af mange
forskellige i markedet, men kan man stole på disse tests?
Et produkt kan være bedre den ene dag, fordi andre produkter ikke er blevet opdateret endnu. Søger man
på bedst opdaterede AntiVirus beskyttelse, så får man forskellige resultater frem alt efter hvilken side man
ser på. Men typisk er disse at finde i top-10 listen:
Andre test kan vise andre resultater, bl.a. Microsofts ”Defender” som i nogle test klare sig glimrende og i
andre tests falder igennem.
Når man modtager nyt software, fx en opdatering, ja så bør den også testes for malware inden den
installeres. Det betyder at man skal have et sikret miljø som forhindre at eventuel malware kan sprede sig
til andre systemer i virksomheden. Der findes forskellige former for sikrede miljøer:
Stand-alone udstyr: Man har på simpel vis et testmiljø der er ”galvanisk adskilt” fra alt andet
Sandbox miljø: Et Sandbox miljø er logisk adskilt fra resten af virksomheden, kan fx være en midlertidig
virtuel maskine
Side 93
Hvad skal man foretrække af disse to typer? – det er der ikke en klar definition på. Så brug den mulighed
der er mest nærliggende, men er det så en garanti for at fx en opdatering ikke indeholder malware. Nej det
er det ikke, en software opdatering kan fx indeholde muligheden for selv at hente software et sted fra. Det
betyder så også at der er brug for systemer der tester kommunikation. Men generelt kan man ikke være
100% sikker på noget.
WEB filter
Mange virksomheder har et WEB filter, kan være indbygget i Firewallen, men er typisk etableret på et
selvstændigt miljø, al internettrafik går så forbi dette filer inden den sendes/modtages af den enkelte
medarbejder eller system. WEB-browseren kan også indeholde mere simple versioner af WEB filtre.
Formålet er at scanne al trafik, baseret på opsatte regler
```
Malwarebeskyttelse: Phishing og andre ondsindede websteder kan bruges til at levere malware og andet
```
ondsindet indhold til brugernes computere. Webfiltrering gør det muligt for en virksomhed at blokere
adgangen til websteder, der udgør en trussel mod virksomhedens og brugernes sikkerhed. Helt analogt
med det vi kender fra spam filtre i mail sammenhænge.
```
Datasikkerhed: Phishing-websteder er almindeligvis beregnet til at stjæle brugeroplysninger og andre
```
følsomme data. Ved at blokere adgangen til disse sider begrænser en organisation risikoen for, at sådanne
data vil blive lækket eller brudt.
Regulatorisk overholdelse: Virksomheder er ansvarlige for at overholde et voksende antal
databeskyttelsesforskrifter, som påbyder, at de beskytter visse typer data mod uautoriseret adgang. Med
webfiltrering kan en organisation administrere adgang til websteder, der sandsynligvis vil forsøge at stjæle
```
beskyttede data, og dem, der kan blive brugt bevidst eller utilsigtet til at lække data (såsom sociale medier
```
```
eller personlig cloud-lagring).
```
Håndhævelse af politik: Webfiltrering gør det muligt for en organisation at håndhæve
virksomhedspolitikker for webbrug. Alle typer webfiltrering kan bruges til at blokere upassende brug af
virksomhedens ressourcer, såsom at besøge websteder med eksplicit indhold.
```
Statistik: Indeholder gode muligheder for at se hvad brugerne anvender internetkommunikation til, fx i
```
hvilken udstrækning anvendes Facebook eller andre lign. medier – og hvornår.
Konfiguration
Som nævnt kan malware komme ind hvis ens systemer ikke er beskyttet tilstrækkeligt, de fleste systemer
```
(hardware og software) er beskyttet som de fleste brugere kan leve med via standard ”hardening”, men
```
man kan ikke stole på at det er tilstrækkeligt i ens specifikke situation. Der findes leverandør specifikke
hardening dokumenter som er udarbejdet af diverse sikkerhedsfirmaer eller uafhængige organisationer.
Bland disse er CIS nok den mest kendte. Hardening dokumenter kaldes her Benchmarks.
Hardening dokumenter er typisk opdelte i disse kategorier:
• Application hardening
• Operating system hardening
• Server hardening
• Endpoint hardening
Side 94
• Database hardening
• Network hardening
Desværre er det forholdsvist dyrt at have et abonnement på CIS, så ofte må man forholde sig kritisk til
leverandørernes hardening dokumenter eller søge andre kilder.
Zero-Day
Tiden fra der opdages en sårbarhed, til den bliver kendt er kritisk og kaldes ”Zero-Day”. Denne periode kan
udnyttes af dem der hacker. Leverandøren vil ofte være vidende om sårbarheder og have kendskab til disse
før de kommer med en patch, det er en balance som mange leverandører har et blandet forhold til. Man
kan som virksomhed lave en aftale med nogle leverandører om håndtering af denne periode, fx ved at de
anviser mitigerings forslag indtil en patch er klar. Men det er bestem ikke alle leverandører der tilbyder
dette og det er også kun større virksomheder der får tilbuddet. Mere om dette under leverandørstyring.
Det er almindeligt at leverandørerne siger: Vi har fundet en sårbarhed og vi har for øvrigt også en patch
5.2.4 Sociale medier
De sociale medier udgør et stigende problem, en del malware kan komme ind via disse veje. De sociale
medier anvendes da også i stigende grad og mon ikke de fleste brugere har fået underlige henvendelser og
tilbud. De 3 største risici er:
• Download af malware
```
• Cyberbulling (mobning)
```
• Data tyveri
• Identitets tyveri
• Skade omdømme
Man kan ikke længere lave en skarp opdeling mellem arbejde og privatliv, mange virksomheder har derfor
også regler for anvendelsen af sociale medier i forbindelse med arbejde.
Virksomheder kan teknisk eller administrativ begrænse brugen af fx Facebook og lign systemer, men stort
set ingen virksomheder ønsker et totalforbud. Alle virksomheder har dog et legitimt krav omkring loyalitet
som ikke kun gælder for sociale medier.
En politik for anvendelse af sociale medier kaldes også for en SoMe politik og kan typisk indeholde disse
```
overskrifter:
```
• Præcisering af loyalitetspligten
• Reducer risikoen for medarbejdernes handlinger, så virksomheden ikke bliver erstatningsansvarlig,
fx i forhold til markedsføringsloven
• Forventningsafstemning omkring promovering af virksomheden
• Reducer risiko for offentliggørelse af forretningshemmeligheder
• Forebygge chikane og mobning
• Regulering af medarbejdernes forbrug af sociale medier
• Vejledning til den enkelte medarbejder
Mange skoler har en skarp formuleret politik.
Side 95
5.3 IoC
IoC betyder Indicator of Compromise
Under en cybersikkerhedshændelse er IoC spor og beviser på et databrud. Disse digitale data stumper kan
ikke blot afsløre, at et angreb har fundet sted, men ofte, hvilke værktøjer der blev brugt i angrebet, og
hvem der står bag dem.
IoC’er kan fx være signaturer i et malware beskyttelsessystem, men kan også være en IP-adresse som man
ved står bag hackere mv.
IoC’er er således noget der udveksles mellem de organisationer der ønsker at beskytte, og lever af, at
beskytte virksomheder og privatpersoner.
```
En anden art kaldes en IoA (Indicator of Attack), IoA anvendes til at afgøre om et angreb er under udførsel.
```
Generelt er det interessant at se på om der foregår noget unormalt og mange SIEM systemer har netop
denne funktionalitet, det er også disse systemer der kan fodres med IoC/IoA’er.
5.4 DLP
DLP betyder Data Leakage Prevention, og er typisk et system der holder styr på trafikken ind/ud af en
virksomhed, blandt det der ofte ses efter er:
• Transport af specifikke data fx CPR-numre
• Transport af store filer
• Transport til bestemt områder
Men generelt kan der opsættes regler i disse systemer, hvilket gør det muligt for virksomheder at begrænse
transport af fortroligt materiale, eller fx at holde styr på om man overholder GDPR forordningen. Nogle
DLP-systemer kan også scanne hele filsystemer for bestemte mønstre, igen kan CPR-numre anvendes som
et eksempel. Der kan læses mere om DLP-systemer hos de forskellige leverandører, samt her.
Der findes tre typer af DLP-systemer:
• Netværks DLP
• Endpoint DLP
• Cloud DLP
Som eksempel på Cloud DLP kan nævnes Microsofts DLP-system i deres SharePoint løsning, her kan man
konfigurere både det at scanne hele SharePoint instansen og løbende overvåge filtransporten.
AI vil også kraftigt påvirke disse løsninger i fremtiden, til bl.a. at holde styr på unormal trafik.
5.5 DDOS og botnet
DDOS betyder ”Distributed Denial of Service Attack”, I praksis at en hjemmeside eller anden dataadgang
ikke bliver tilgængelig pga. stor belastning. Denne angrebstype er meget almindelig og udføres af
Side 96
professionelle, man kan lave en SLA-aftale med en udbyder af denne service – så skal man blot fortælle
hvem man ønsker at blokerer og så betale med sit kreditkort. Nogle af disse DDOS angreb kan være meget
store og ødelægge det for andre også, hvis internet forbindelserne er indrettet af ISP’en i fx øer. Der findes
```
forskellige angrebsflader i OSI-modellen, men meget typisk er det lag 3 der bliver angrebet (ICMP, fx ping).
```
En anden ofte anvendt angrebsmetode, er at anvende IP spoofing i kombination med fx DNS, dvs. man
beder en DNS server om at give alle oplysninger på en bestemt IP-adresse, og har man så som angriber
anvende dette adresse i sit request, ja så bliver den store DNS record sendt til den IP-adresse man angriber.
Tilsvarende kan andre protokoller som fx NTP anvendes, men det forudsætter at IP-adresse spoofing er
tilladt.
Skal man lave et DDOS-angreb, ja så skal man have mange enheder til at sende et request til den enhed
man ønsker angrebet, dette gøres nemmest ved at anvende et botnet. Det tager tid for en kriminel at
opbygge et botnet. Et botnet består af et stor antal enheder der kan kontrolleres af en kriminel, disse
enheder er blevet inficeret med en form for malware som kan styres centralt fra. Den kriminelle har så
hvad der kaldes en ”Command and Control server” der kan dirigere alle enheder i et botnet at angribe en
bestemt adresse. Men enheder menes alle typer af IP forbundne enheder der er modtagelige for malware,
vil typisk være Windows eller MAC computere, men kan også være IoT enheder.
So angivet på figuren kan botnets også anvendes til at udsende helt almindelig spam mails, for derved at
undgå de forskellige mailudbyders begrænsninger, fx t man kun kan sende 500 mails ud i timen fra den
samme konto.
Hvordan kan man så forebygge at man bliver medlem af et botnet, det kan man først og fremmest ved at
sikre sig at enhederne man administrere er opdaterede.
DDOS-angreb kan forebygges bl.a. ved forskellige teknikker, ofte anvendes det der kaldes en ”Scrubber” en
enhed som trafik kan sendes igennem hvis der detekteredes at der er et DDOS-angreb i gang. Men i første
omgang skal man kunne detektere om der er et angreb i gang, dette sker som oftest ved at man se om det
trafikmønster der er i gang er atypisk.
Side 97
5.6 Klassifikation af sårbarheder
Hvor alvorlig er en sårbarhed? – det kan være meget subjektivt at afgøre, men der findes et standardiseret
```
system kaldet CVSS (Common Vulnerability Scoring System) som kan klassificere sårbarheder. CVSS blev
```
først annonceret i 2003 af ”National Infrastructure Advisory Council” og betegnes som en industri standard.
I praksis er FIRST udpeget som den organisation som varetager og vedligeholder CVSS systemet
CVSS-systemet anvendes globalt og har udviklet sig i specifikke versioner. Seneste udgave er version 4.
Skalaen går fra 0 til 10, hvor 10 er det mest alvorlige. Sårbarhedsscannere anvender CVSS systemet til at
score sårbarheder og er en stor hjælp i prioritering af arbejdet med fx at patch sine systemer. Flere
virksomheder har fx en politik om at bliver en sårbarhed kendt som betegnes som ”Critical” eller ”High” så
skal der patches straks.
Den metode der anvendes for at finde en specifik CVSS score for en given sårbarhed er ganske detaljeret,
netop for at tage det subjektive ud af ligningen, FIRST har en kalkulator til dette formål, denne kan ses her.
Detaljer om sårbarheder er naturligt ok opgivet med fortrolighed, men kan godt fortælle at der er fundet
en sårbarhed i Unix version x.y, men en CVSS score på 5.6 – det er der ikke i sig selv fortrolighed omkring,
men kan også fortælle at der er en patch eller sårbarheden kan mitigeres ved at gøre noget bestemt.
Offentlige tilgængelige oversigter over sårbarheder kan findes her. Disse kaldes CVE Security Vulnerability
Database. Man kan i denne database finde en del oplysninger om sårbarheder, hvoraf nogle er ganske
```
alvorlige:
```
Side 98
Det er altid interessant at søge egne systemer frem i denne database. Firmaer der laver
sårbarhedsscanninger giver som oftest input sammen med leverandørerne til denne database.
5.6 Hvem passer på Danmark
```
Som udgangspunkt er opgaven hjemmehørende hos Forsvarets Efterretningstjeneste (FE), det er nemlig her
```
```
Center for Cybersikkerhed (CFCS) er organiseret – indtil videre, der kan komme ændringer hertil i
```
forbindelse med en oprettelse af ”Ministerie for Samfundssikkerhed og Beredskab”.
CFCS udgiver en række pjecer og er til rådighed i et vist omfang for offentlige og private institutioner og
virksomheder, men dog uden at konkurrerer med alle de sikkerhedsfirmaer der er i markedet. CFCS’s
primære fokus er at passe på de samfundskritiske funktioner og derigennem Danmark.
Det kan naturligvis undre at CFCS er placeret i FE, FE tager sig sum udgangspunkt af det der er fra den
danske grænse og ud og PET tager sig af det interne i Danmark, forklaringen er at en sikkerhed er
grænseoverskridende og derfor er samarbejdet med udenlandske tjenester essentiel. Det er dog også
fremført flere steder at en af grundene er at sikre budgettet til området.
Både som offentlig eller privat virksomhed er CFCS vejledninger værd at læse og få vejledning fra. Det er
fode vejledninger der direkte kan anvendes. Man kan tilmelde sig en mailingliste, dette kan kun anbefales –
så bliver man opdateret når der sker noget nyt.
Side 99
Ovenfor kan man læse hvad FE og CFCS primære opgaver er, samt et eksempel på hvad det overordnede
indhold af en trusselsrapport.
5.6.1 National strategi for cyber og informationssikkerhed
Den Danske regering udgang i 2014 den første version af strategien, her blev der bl.a. udpeget enkelte
samfundskritiske sektorer som der var et særligt fokus på. Dette medførte bl.a. at der for første gang skete
en regulering af fx telesektoren på sikkerhedsområdet, dvs. der blev udarbejdet en lov og efterfølgende en
bekendtgørelse der direkte adresserede teleområdet. CFCS udarbejdede lov og bekendtgørelser og det blev
også CFCS der havde tilsynsopgaven med overholdelsen – en opgave de stadig varetager. De
bekendtgørelse der må komme ud af NIS2 loven, vil sandsynligvis skulle udarbejdes af det enkelt
ressortministerie hvor så også tilsynsopgaven forventes placeret.
Den seneste strategi dækker 2022 til 2024, og kan findes her. Ansvaret for udarbejdelsen er lagt i
Digitaliseringsstyrelsen. Hovedpunkterne fra deres hjemmeside er følgende:
Side 100
Hvad kommer der så ud af en strategi?
Digitaliseringsstyrelsen sætter initiativer i gang og har midlerne hertil. De samfundskritiske sektorer
pålægges at indarbejde den overordnede strategi i deres delstrategier del-strategier, som eksempel kan
den seneste for telesektoren hentes her. Disse strategier er normalt offentlige tilgængelige. For
telesektoren er det CFCS der løbende følger op på status.
5.6.2 NOST
Den Nationale operative stab, kaldet NOST i daglig tale, på deres hjemmeside skriver de slev følgende:
I tilfælde hvor Danmark rammes eller påvirkes af større kriser og hændelser, som fx ekstremt vejr, brand,
eksplosioner, strømafbrydelser, ulykker eller angreb, træder Den nationale operative stab – i daglig tale
NOST – sammen for at styre og koordinere den operative indsats på tværs af myndighederne.
Staben ledes af Rigspolitiet og består ud over Rigspolitiet af Politiets Efterretningstjeneste, Forsvarets
Efterretningstjeneste, Forsvarskommandoen, Beredskabsstyrelsen, Udenrigsministeriet, Styrelsen for
Side 101
Forsyningssikkerhed, Sundhedsstyrelsen og Trafikstyrelsen. Andre myndigheder kan indkaldes efter behov i
forhold til hændelsens karakter.
Er det så interessant for virksomhederne? – ja det er det for specielt de samfundskritiske sektorer kan nemt
blive inddraget, dette skete bl.a. i forbindelse med Corona krisen. Her blev en række private virksomheder
bedt om at medvirke til sikring af Danmark.
5.6.3 Cyberværnepligt
Cyberværnepligt er en uddannelse, den basale soldat uddannelse suppleret med nogle måneder specifik
rettet mod IT og sikkerhed. Det er ikke et specielt værn, men et supplement. Man får løn under
uddannelsen og der er en optagelses test man skal gennemgå. Der er mere information her.
Det er et krav at man kan sikkerhedsgodkendes til ”Hemmelig”, men eller er der ikke specielle krav udover
bestået folkeskole, basal viden om PC/MAC og netværk.
5.7 Hvem passer på virksomhederne
Som udgangspunkt er det virksomhedernes eget ansvar, men virksomhederne understøttes bl.a. gennem:
1. Lovgivning, fx NIS2 og bekendtgørelser
2. Vejledninger og delvis support fra Brancheorganisationer bl.a. CFCS
3. Købe konsulentbistand fra diverse Sikkerhedsfirmaer.
Virksomhederne har derfor en række håndtag de kan trække på, men først og fremmest skal
virksomhederne selv være klar over hvilke risici de reelt står overfor, deres afhængighed af fx
produktionsapparat, omdømme og lign. Rigtig mange virksomheder har ikke dette overblik, ingen har
sikkert det fulde overblik – men en grad af overblik er nødvendig, om ikke andet så for at efterleve
gældende lovgivning.
Specielt SMV-segmentet har sine udfordringer, bl.a. fordi de ikke selv har kompetencerne og ledelsen
tænker ”det er vist ikke noget der rammer os” – men set i lyset af fx den undersøgelse som PwC har lavet
over hvad virksomheder reelt er udsat for, se tidligere i dette afsnit, er det åbenlyst at virksomhederne må
have et skærpet fokus på området. De fleste virksomheder få det oftest først efter de er blevet ramt,
hvilket kan være til stor frustration for sikkerhedsfolk.
I 2024 har Digitaliseringsstyrelsen oprette en varslingstjeneste, her kan bl.a. SMV segmentet få varsler om
sikkerhedshændelser og forhold.
5.8 Hvordan sikre den enkelte borger sig
”En borger” er et meget blandet begreb, for en typisk borger findes naturligvis ikke, men alligevel er der i
de nationale strategier afsat midler der skal hjælpe den enkelte borger. Hjælpen består primært i konkrete
vejledninger til hvad man skal foretage sig hvis man oplever en hændelse samt en udmærket APP. Fokus er
derfor hvad man kan gære når skaden er sket.
Samlet set er det nok desværre de færreste borgere der er bekendt med mulighederne, eksempler:
Side 102
I praksis findes disse vejledninger via www.sikkerdigital.dk. På hjemmesiden er der yderligere et
telefonnummer, kaldet Cyberhotline her kan man ringe til hvis man er gået fast. Hvor mange der benytter
sig af dette, er ikke at finde på deres hjemmeside.
Side 103
På APP siden kan ”Digital selvforsvar” kun anbefales.
Men et er hvad man skal gøre når man har været udsat for en hændelse, noget andet er hvad man skal/kan
gøre proaktivt for at undgå dette. Det er der også vejledning til på sikkerdigital.dk
Hvad er det i praksis man anbefaler familie, venner og kollegaer at være opmærksom på?
Eksempler kunne være:
```
• Bruge gode, ikke genbrugte, kodeord (MFA) – pasordshusker?
```
• Klik ikke på links du ikke kender eller har undersøgt
• Afgiv aldrig dine oplysninger til steder du ikke kender
• Hold dine systemer opdateret – malwarebeskyttelse+
• Hvis noget er for godt til at være sandt, så er det ikke sandt
• Vær forsigtig med opkald og SMS
• Køb ikke udstyr der er for billigt, opdateringer?
• Hold dig fra mystiske handelsplatforme
• Backup af data – hvad er vigtig for mig?
• Del med omtanke, pas på reklamer og konkurrencer
• Hvis noget er gratis, så er du selv betalingen
Digitaliseringsstyrelsen har sammen med ”Ældre Sagen” udarbejdet en folder, kan ses og hentes her.
Modul 6: Leverandørstyring
Styring af en virksomheds leverandører har en stigende betydning og for de virksomheder der skal være
NIS2 compliant får det en ekstra stor betydning, det er ikke længere nok at tage højde for virksomhedens
egne risici, nu skal man også tage sine leverandørers risici med ind i sin egen risikostyring. Det giver god
mening, men er et ekstra lag. Baggrunden har fx været at en sourcing partner typisk har fuld adgang til en
virksomheds IT-systemer kan være blevet hacket, dermed får en 3 part adgang, hvilket naturligt nok udgør
en risiko den enkelte virksomhed kan have vanskelig ved at kontrollere.
Side 104
6.1 Leverandørtyper
Nu er det jo ikke uden betydning hvad det er der købes, en lang række produkter indeholder ikke ”Cyber
risici” og kontrakter skal som følge heraf ikke indeholde cyber specifikke detaljer eller krav.
Der findes forskellige opdelinger- men denne kan eventuelt anvendes:
De sikkerhedsmæssige krav stiger alt efter hvad der købes, flere krav handler om outsourcing, dvs. hvis en
virksomhed overlader håndteringen, fx IT-drift, til en ekstern part. Man kan desværre ikke outsource
ansvaret, man kan kun outsource opgaver.
Køber en virksomhed ”Ikke tekniske produkter”, følger der som ofte ikke Cyber sikkerhedskrav med, men
der kan stadig, og vil være der en række leverance og kvalitetskrav.
6.2 Leverandør og NIS2 krav
NIS2 er beskrevet mere detaljeret i modul 3. Det nye ved NIS2 er at virksomheden skal medtage sine
sikkerhedskrav i relation til de leverandører man har, helt fra risikoanalyse – dvs. virksomhedens
risikoanalyse skal indeholde dele af sine leverandørers risici. Hvorfor så det?
Der har været adskillelige eksempler på at en leverandør er blevet hacket og det så har medført at de
produkter og services der leveres, har indeholdt fx malware. MÆRSK sagen er et af de mere kendte
eksempler på dette.
NIS2 artikel 21 er blandt de mere konkrete artikler i direktivet
Medlemsstaterne sikrer, at væsentlige og vigtige enheder træffer passende og forholdsmæssige tekniske,
operationelle og organisatoriske foranstaltninger for at styre risiciene for sikkerheden i net- og
informationssystemer, som disse enheder anvender til deres operationer eller til at levere deres tjenester, og
for at forhindre hændelser eller minimere deres indvirkning på modtagere af deres tjenester og på andre
tjenester.
Side 105
Artikel 21, stk 3 lettere oversat:
Når enhederne overvejer, hvilke foranstaltninger, der er nødvendige til at sikre forsyningskædesikkerheden,
skal de tage hensyn til de sårbarheder, der er specifikke for hver direkte leverandør1 og tjenesteudbyder, og
den generelle kvalitet af deres leverandørers og tjenesteudbyderes produkter og cybersikkerhedspraksis,
herunder deres sikre udviklingsprocedurer.
I denne overvejelse er enhederne også forpligtede til at tage hensyn til resultaterne af ”de koordinerede
sikkerhedsrisikovurderinger af kritiske forsyningskæder”.
Den fulde tekst findes i arkivet under Modul 3.
6.3 Leverandørprocessen
Den danske CFCS har udgivet en guide til leverandørstyring, i denne opdeles processen med
indkøb/outsourcing i 5 aktiviteter:
1. Planlægning
2. Kravstildeles
3. Leverandørvalg
4. Aftalen
5. Styring
6. Afslutning
Dokumentet fokuserer meget på outsourcing, men tænker man på begrebet i sin bredeste forstand, kan
det bruges helt generelt i relation til leverandører – der er måske så ikke noget der er relevant hvis man fx
blot køber noget som ikke relatere sig til cyber trusler.
Meget afhænger af hvor stor virksomheden er, en større virksomhed har en ”Procurement proces” som er
obligatorisk at følge, små og mindre virksomheder har oftest fundet et produkt fra en leverandør som der
så købes og installeres.
Fordelen ved at følge en struktureret proces vil typisk være at man har identificeret krav og interessenter
før man beslutter sig til hvilken produkttype man ønsker sig, samt derefter få tilbud fra flere og dermed
sandsynligvis en bedre pris. Hvis man er leverandør, så er man basalt også interesseret i at kunden får det
rigtige produkt og bliver tilfreds med det.
I CFCS-dokumentet peges der på følgende i outsourcing sammenhæng:
Side 106
én RACI kan også bruges i denne sammenhæng fx:
Overordnet indeholder CFCS følgende overskrifter pr fase:
Side 107
6.3.1 Planlægning
Hvad er det i praksis man søger, er det anskaffelse af en ny service, outsourcing eller lign., er der alternative
forhold der bør overvejes og har man interessenterne med – ja hvem er de i praksis.
Identifikation af interessenter og risikoanalyse er den primære aktivitet i denne fase. Det er også
interessant at få defineret hvem der er den primære interessant – hvem der det der står med kontrakten
og skal sikre overholdelsen indtil aftalen afsluttes?
Side 108
6.3.2 Kravstilleslse
Er oplagt et kerneområde, hvilke krav interessenterne har til købet, er typisk afgørende for valget af
leverandøren. De forskellige interessenter vil have forskellige krav, disse skal samles og vurderes, er det fx
økonomi, brugervenlighed eller sikkerhed der skal vægte højest?
Undgå̊ generelle og ukonkrete krav såsom ”Leverandøren skal foretage backup af systemet”. Stil klare og
præcise krav, der er tilpas specifikke, f.eks. ved at konkretisere omfanget og frekvensen af backuppen samt
antallet af opbevarede sikkerhedskopier hhv. online og offline.
Hvad kan man i praksis komme igennem med af krav, skal man fx at leverandøren er ISO27001 certificeret
og hvad du hvis den bedste leverandør ikke er det? – hvad med SOA, kan man kræve at få den udleveret?
Skal man kræve at man kan komme og lave en uafhængig audit? – ikke mange virksomheder vil have
kunder gående rundt og spørge medarbejderne ud om processer.
Skal man kræve bestemte sikkerheds og kvalitets certifikater?
Generelt om krav så skal de være SMART:
Man kan stille potentielle leverandører en række overordnede spørgsmål fx:
• Har virksomheden en sikkerhedspolitik og er den tilgængelig for kunder
• Har virksomheden en sikkerhedsstrategi og vil den vær tilgængelig for kunder
• Hvilke compliancekrav skal virksomheden efterleve
• Er der specielle sikkerhedsforhold som virksomheden ønsker at oplyse
• Har virksomheden nogle sikkerhedscertifikater
• Hvordan kontrollerer virksomheden underleverandører
• Hvordan håndterer virksomheden awareness
• Har virksomheden en sikkerheds governance struktur og er den tilgængelig for kunder
• Har virksomheden BCM-planer og testes disse
• Vil virksomheden dele risikoanalyser/billeder
Dertil kan der så spørges mere specifikt indenfor områder som:
• Datacentre
• Fysisk sikkerhed
• Udvikling
• Sikkerheds infrastruktur
Men igen afhænger det af hvad der skal købes.
Side 109
6.3.3 Leverandørvalg
Ikke alle krav vægter lige højt, et af kravene fra fx en finansafdeling kan være at det maksimal må koste et
bestemt beløb, på sikkerhedsfronten kan der være krav om ISO-certificering. Andre interessenter kan
kræve at bestemte compliancekrav overholdes osv. Man skal inden der sker et endeligt valg have bestemt
sig hvilke krav der er ultimative og hvilke der er mere optionelle.
Sikker Digital har udgivet et par vejledninger, kaldet:
• Leverandørdialog spørgeskema
• Leverandørdialog vejledning
Disse to dokumenter findes i fællesarkivet.
Er der flere leverandører der har budt på opgaven, skal de behandles lige og fair, nogle af de parametre der
kan være afgørende, kan fx være:
• Leverandørens evne til at leve op til de stillede sikkerhedskrav.
• Leverandørens geografiske placering.
• Leverandørens accept af eventuelle overgangsforhold, hvis opgaven tidligere har været outsourcet
eller varetaget af en anden leverandør.
• Leverandørens villighed til at samarbejde og til at lade sig efterse/revidere.
• Leverandørens accept af ophørsbestemmelser, herunder forpligtelsen til at opretholde cyber- og
informationssikkerheden i hele ophørsperioden.
• Leverandørens økonomiske forhold og ejerforhold.
• Leverandørens brug af underleverandører, hvordan sikres at krav videreformidles?
• Leverandørens integritet og eventuelle konstaterede tilfælde af væsentlig misligholdelse af tidligere
offentlige kontrakter.
• Størrelses- og afhængighedsforholdet mellem kunde og leverandør.
• Risikoen for leverandørlåsning pga. omkostningerne ved senere at skifte leverandør, når kunden
først er blevet afhængig af leverandørens ydelser.
6.3.4 Aftalen
Hvad der skal indgå detaljeret i den konkrete aftale, er udenfor scope af disse noter. Men
Under leverandørvalg starter typisk udformningen af kontrakten, en kontrakt kan være helt ny eller blot en
udbygning af en eksisterende. Kontaktudformningen, afhængig af leverandørkategori, kan være udarbejdet
sammen med en ekstern part.
Ved større outsourcing aftaler kan det anbefales at anvende en ekstern part der har erfaring med
udarbejdelse af den type kontrakter.
Side 110
6.3.5 Styring
Den i virksomheden er er ansvarlig for kontrakten, har ansvaret for at sikre at kontrakten overholdes
gennem hele kontraktperioden. Det kan også ske ændringer som ligeledes skal varetages i
kontraktperioden, fx nye krav, udvidelse af aftale mv.
Den løbende opfølgning af kontrakt kan fx ske via disse aktiviteter:
```
• Statusmøder mellem kunde og leverandør (faste møder eller ad hoc).
```
```
• Skriftlig rapportering til kunden (fast afrapportering eller ved anmodning).
```
```
• Tilsyn hos leverandøren (enten varslet eller uanmeldt besøg).
```
• Intern audit/gennemgang eller egenkontrol foretaget af leverandøren.
• Ekstern audit/gennemgang foretaget af kunden eller en uvildig tredjepart.
• It-revision/audit via certificerede revisorer.
• Beredskabsøvelser med kunden som deltager eller observatør.
```
• Sikkerhedstekniske undersøgelser (også kaldet penetrationstests).
```
Men meget afhænger af hvor stor virksomheden er og hvad der købes.
6.3.6 Afslutning
Det er ikke unormalt at denne del af en aftale ikke overvejes grundigt når aftalen udarbejdes, igen er det
meget afhængigt af hvad aftalen handler om, men følgende områder kan overvejes – og skal så i praksis
være med allerede ved kontraktindgåelsen:
• Leverandørens forpligtelser og fortsatte servicemål i ophørsperioden, hvis aftalen frivilligt opsiges
eller ophører som følge af tvister mellem parterne.
• Kundens krav til cyber- og informationssikkerhed i kunde-leverandørforholdet, mens opgaven
overdrages til en anden leverandør eller overtages af kunden.
```
• En komplet liste over kundens aktiver (inklusive backup) opbevaret hos leverandøren, der skal
```
leveres tilbage til kunden, overdrages til en ny leverandør eller bortskaffes.
• Procedurer, der sikrer, at kundens aktiver leveres tilbage til kunden, overdrages til en anden
leverandør eller bortskaffes, som beskrevet i aftalen.
• Parternes fortsatte tavshedspligt efter aftalens ophør.
• Leverandørens forpligtelse til at bidrage til en smidig overgang og videreførelse af driften, hvis
opgaven skal i genudbud, overdrages til en ny leverandør eller hjemtages af kunden, herunder krav
til leverandørens udlevering af dokumentation, overførsel af viden og samarbejde i
overgangsperioden.
Side 111
6.4 Leverandøradgang
Nogle leverandører skal have fysisk eller logisk adgang til virksomhedens IT eller OT-miljø, det kan være
under normale driftsforhold, som fx ved outsourcing aftaler – men det kan også være i forbindelse med
supportopgaver hvis virksomheden selv drifter.
Ved fysisk adgang bør virksomheden have en politik for om leverandøren må færdes frit eller der kun må
være ledsaget adgang.
Ved logisk adgang skal der være en politik/procedure for håndtering af VPN, skal en sådan fx altid stå åben,
hvad må den give adgang til, hvad logges osv. Eller kræver virksomheden af support kun sker gennem en
medarbejder, fx ved at dele en skærm over Tems eller Zoom. Så er det medarbejderen der er garant for
sikkerheden.
Men også på dette område gælder helt almindelige sikkerhedsprincipper omkring CIA, ”Kneed to know”
principper, brugeradministration og brugerrevidering samt netværksdesign, så leverandørens VPN kommer
ind fx via et DMZ.
Modul 7: Konsulentrollen og Implementering
7.1 Konsulentrollen
De fleste virksomheder anvender på tidspunkter eksterne ressourcer, kaldet konsulenter. Det er en oplagt
måde at tilføre viden til virksomheden som man ikke selv har. Nogle virksomheder anvender store
mængder af konsulenter til konkrete opgaver, enkelte konsulenter har være konsulent i virksomheden så
mange år at man glemmer det er en ekstern ressource – og ikke tager højde for at viden kan forsvinde fra
den ene dag til den anden.
Harvard Business Review indeholder en glimrende artikel omkring anvendelsen af konsulenter, den kan
læses her. Den øverste del af artiklen siger dette:
Each year management consultants in the United States receive more than $2 billion
for their services.1 Much of this money pays for impractical data and poorly
implemented recommendations.2 To reduce this waste, clients need a better
understanding of what consulting assignments can accomplish. They need to ask
more from such advisers, who in turn must learn to satisfy expanded
expectations.
Som det fremgår, er det ikke kun positive aspekter i at anvende konsulenter, netop det at en ekstern
konsulent har manglende kendskab til virksomhedens kultur og dynamik bevirker ofte at en
implementering reelt ikke lykkedes og at pengene kan være spildt. Til gengæld vil det ofte være sådan at en
ledelse ofte er mere lydhør overfor en ekstern konsulent, bl.a. fordi man forventer at det er en specialist –
hvilket også ofte er afspejlet i prisen.
Side 112
Som intern konsulent burde man derfor have bedre muligheder, der er da også mange virksomheder som
anvender eksterne konsulenter til at understøtte interne ressourcer med specialistviden. En løsning der kan
medvirke til en mere sikker implementering.
I artiklen fra Harvard Business Review er der en udmærket illustration af hvilke ydelser eksterne
konsulenter typisk yder til virksomheder:
I artiklen beskrives de enkelte trin.
Anbefalingen er at man som virksomhed gør sig det klart hvad man vil bruge den eksterne konsulent til og
ikke lader sig overbevise om ekstra ydelser medmindre disse er meget velovervejet. Der er eksempler på at
virksomheder ansætter eksterne konsulenter til at styre eksterne konsulenter fra et andet firma, det er
sjældent en god ide!.
I afsnit 1.6 var der en kort gennemgang af emnet ”Assurance program”, dette kunne være et godt eksempel
at tage udgangspunkt i – et sådant program vil også ”Hvedebro Maskinfabrik” skulle have etableret,
Side 113
interessant er det derfor at overveje i hvilket udstrækning der er brug for eksterne konsulenter og hvad de
kunne tænkes at bidrage med?
Er det en god ide at anvende en ekstern konsulent som projektleder, fx i forbindelse med implementering
af et Assurance Program?
I den situation er det afgørende at man har kendskab til virksomheden, at man kender kulturen. Man kan
anvende en ekstern projektleder som overordnet koordinering, men de specifikke opgaver bør i videst
muligt omfang håndteres internt, helt specifikt implementering.
En ekstern projektleder vil ofte have vanskelig ved at bedømme hvad det kræver internt at komme i mål
med fx et specifikt projekt, her er det afgørende at der er en intern at sparre med så projektet bliver opdelt
i nogle faser, der hver især giver værdi og giver et synligt resultat.
7.2 Hvad er god sikkerhed?
Hvad er god sikkerhed, og hvem afgør om det er ”godt nok”, i en virksomhed kan det være
finansafdelingen, eller den administrerende direktør. Dvs. i praksis er det i mange tilfælde økonomien der
sætter baren for hvad der er ”godt nok”. Set med sikkerhedsbriller er det ikke det bedste valg, vi vil som
sikkerhedsansvarlige som oftest anvende en risikoanalyse og så, sammen med ledelsen, estimere hvad
reduceret risici på forskellige områder koster og kræver af initiativer.
Som sikkerhedsansvarlig vil man ønske at have en norm at læne sig op af, normen kan være en
sikkerhedsstandard, fx at virksomheden bliver certificeret efter fx ISO27001, men der er også andre
muligheder.
Det offentlige Danmark, er pålagt 20 tekniske minimumskrav som kan bruges som rettesnor, de tekniske
minimumskrav er beskrevet her, og findes i fællesmappen. Der er tale om tekniske krav, ikke krav til
processer -men de tekniske krav er en god rettesnor for hvad de danske myndigheder har defineret som
minimumskrav. Som følge heraf er de gode at måle sig op af. Disse krav justeres løbende, afhængig af det
trusselsbillede vi i Danmark står overfor. Trusselsbilledet er beskrevet i modul 5.
Og hvad hvis man så ikke efterlever alle 20? – så er man for det første klar over at man ikke er på ”best
practice” niveau, dernæst ved ham hvad man kan/bør/skal stræbe efter, eller man ikke ser det
trusselsbillede for virksomheden – eller man til sidst bare accepterer disse risici. Der er ikke nogen tvivl om
at myndighederne gerne ser ”samfundskritikinfrastruktur” efterleve disse 20 minimumskrav, men reelt har
myndighederne ikke lovhjemmel til at force det i den private sektor. I den sammenhæng anvendes
bekendtgørelse som det er sket med NIS1 og som sker med NIS2 – dermed dækkes lang flere
virksomheder..
7.2.1 Hvad kan konsulenten gøre i praksis
En konsulent opfinder som udgangspunkt ikke noget nyt, en konsulent anvender allerede kendt standarder
og vejledninger. Ofte har konsulenthusene en fast metode der anvendes når en ny virksomhed bliver
kunde. Som nævnt vil en konsulent f.eks. se på de 20 minimumskrav som er nævnt ovenfor, eller andre
tilsvarende krav for specifikke sektorer. Energisektoren har 25 krav som kan være interessante at se på, de
er ikke specifikke for sektoren – men ganske generelle. De findes i EnergiCERT håndbogen som findes i
fællesarkivet. De 25 anbefalinger:
Side 114Side 115
Hvordan kan man så som konsulent anvende disse struktureret? - der skal være en form for skala, man kan
kalde det en modenhedsskala, man kan fint anvende en af de modenhedsskaler der har være gennemgået i
Side 116
tidligere moduler, fx NIST:
Af andre interessante parametre der er relevante for vurdering kan nævnes CIS hvad de kalder ”Security
Controls”:
Side 117
ØVELSE: Hvordan ses disse prioriteringer? – vil de kunne anvendes på Hvedebro Maskinfabrik?
Så en ny konsulent i en virksomhed vil typisk sikre sig at der også er arbejde efter den første indledende
fase, så selvom udgangspunktet burde være en risikoanalyse, så er det nærliggende at tage udgangspunkt i
de krav der er nævnt ovenfor. Dvs. ale en vurdering af hvor virksomheden er på hvert enkelt punkt, få
virksomheden til at tage stilling til hvor de gerne vil være og så komme med et forslag til at løse den
udfordring der ligger i at nå målet.
Så en ny konsulent kan f.eks. arbejde i disse tre steps:
4. Præsenter et trusselsbillede, kan være det nationale, branche specifik eller anden viden for
ledelsen. Er der fx lovgivning der skal overholdes osv.
5. Lave en assessment og en gap-analyse, eventuelt suppleret med en penetration test
6. Udarbejde et løsningsforslag og en plan, herunder hvad det vil kræve af ressourcer – dvs.
også hvor konsulenten så ser sig selv bedst anvendt.
En forudsætning for ovenstående er at konsulenten kender virksomhedens ambitionsniveau på
sikkerhedsområdet, assessment delen er også en form for modenhedsanalyse, den vil afdække hvor
virksomheden er i praksis og er et godt udgangspunkt for en debat med ledelsen om hvor de ser
virksomheden bevæge sig hen.
Datatilsynets katalog over ”Foranstaltninger” findes her. Vejledninger fra Datatilsynet her.
Side 118
Men der er en række andre muligheder, på SikkrDigital.dk, er der 7 gode råd til virksomheder – disse kan
findes her. Der findes samme sted en udmærket quiz.
7.3 Sikkerhedsprocesser
Hvilke sikkerhedsprocesser er de mest vigtige for en virksomhed, ja det afhænger af flere faktorer, bl.a.
trusselsbillede, risikoanalyse og typen af virksomheden. Men der er bred konsensus om at følgende
processer er vigtige, i ikke prioriteret rækkefølge:
Proces Beskrivelse Hvorfor
Brugeradministration Sikre at brugere har adgang til det der er
nødvendig, og kun, for udførelse af deres
arbejdsopgaver. Sikre at brugere slettes
når bruger forlader virksomheden, sikre at
det er nemt at lave en oversigt over hvem
der har adgang til hvad. Sikre funktion
adskillelse
Både internt og overfor
virksomhedens revision, skal der
være styr på adgange. Vigtig også
ved incidents
Sikkerhedsopdatering Generel opdatering af infrastruktur, dvs.
patching af operativsystemer,
applikationer, netværkskomponenter,
client udstyr, mobiltelefoner osv.
En af de store risici for
indtrængning af malware er
manglende opdatering af udstyr
– kendte sårbarheder skal
håndteres, dette sker typisk via
patching af systemerne.
Incident Management En proces der beskriver hvordan
incidents, herunder forskellige typer, skal
håndteres. I praksis er det ofte på et
generelt plan ”hvem gør hvad hvornår”
Når der sker et incident, er tiden
ofte en vigtig faktor. Det er
derfor vigtig af have gjort sig
nogle overvejelser om hvordan
disse skal håndteres.
Change Management I forbindelse med ændringer på fx servere
og applikationer, skal der udarbejdes en
plan for hvordan det skal ske og hvis det
giver fejl, hvordan kommer man så tilbage
Der er ofte i forbindelse med
ændringer af systemer der sker
nedbrud
Sikkerhed Risk
Management
En proces der skal sikre at sikkerheds risk
identificeres, og håndteres i praksis.
Processen skal også dokumentere hvilket
acceptabelt risikoniveau virksomheden
kan leve med.
Et vigtigt værktøj for
sikkerhedsafdelingen, være med
til at prioritere hvad der er
vigtigst. Dokumentere hvem der i
virksomheden er ansvarlig for
risici.
Log Management Både i forbindelse med GDPR og i
forbindelse med hændelser er det vigtig
at have styr på hvem der har haft adgang,
måske ændret, data. Yderligere hvem der
fx har udført specifikke kommandoer med
administrationsrettigheder.
Helt essentielt når der er
hændelser, skal også bruges i en
eventuel bevisførelse. Kan
automatiseres
Beredskab Sikre at man er forberedt på hvad man
kan gøre når der kommer et angreb,
fokuser på hvad en risikoanalyse viser og
hvad der er mest værdifuldt.
Det er ikke et spørgsmål om man
får en sikkerhedshændelse, det
er kun et spørgsmål om hvornår.
Side 119
Awareness At sikre sig at brugere/medarbejdere har
en basal forståelse for sikkerhed og sikre
at de ved hvad de skal gøre hvis de fx
opdager en hændelse
Brugere/Medarbejdere er ofte
kalden ”The Human FW”, så
derfor er det vigtigt at de ved
hvad de skal gøre i bestemte
situationer og har en basal viden
om sikkerhed.
Firewall vedligehold Løbende opdatering af FW, kan være en
del af Change Management processen.
Sikre at man løbende har den
nødvendige beskyttelse mod
udefra kommende hændelser.
Backup/restore Proces for løbende backup af system og
periodisk test af om backup kan anvendes
```
(restore test)
```
Så man kan komme hurtig i liften
efter en hændelse, Backup bør
helt eller delvis være eksternt
7.3.1 ITIL
Alle virksomheder har processer for f.eks. de processer der er listet ovenfor, man behøver ikke starte forfra
med at tænke processer. ITIL er et procesframework som er opbygget over lang tid, i dag findes det i
version 4. Der findes en del kurser i ITIL og ITIL er generel og meget anvendt i mange virksomheder.
ITIL er udviklet af IBM og for alvor taget i brug og godkendt af den britiske regering helt tilbage i 1980’erne
og kaldes i dag en ”best practice” globalt indenfor proces flow, med fokus på IT i ordets bredeste
betydning. I England var man meget opsat på at bruge de standardiserede proces flow indenfor den
offentlige sektor, men det bredte sig også hurtigt til den private sektor.
ITIL historien:
Mange ITSM systemer har implementeret ITIL processer” out of the box”.
ITIL V3 proces overblik:
Side 120
For at få proces flow i praktisk form skal man deltage på kurser og/eller købe bøgerne.
ITIL indeholder over 25 processer, bland de mest anvendte er:
• Incident Management
• Service Management
• Release Management
• Change Management
• Problem Management
7.4 Implementering
Implementering, fx af et ”Assurance program” er ofte en overset disciplin, det er ikke ualmindeligt at man
forestiller sig at når software er udviklet og installeret, når en sikkerhedspolitik er udarbejdet og godkendt,
når et projekt er afsluttet – ja så er man færdig. Men først her starter ”bøvlet”
Side 121
Implementering kaldes også ”Change Management”, hvor man normalt ser det som en teknisk disciplin, så
er det på det organisatoriske niveau en ændring af mennesker, måske deres måde at arbejde på?
De fleste mennesker er helt villige til at ændre måden at arbejde på hvis der følger en fornuftig forklaring
med og man kan se det er en god ide. Formår man dette fx i et ”Assurance program”, ja så er ”risikoen” for
succes stor. Noget af det værste er at diktere ændringer uden begrundelse.
Regel #1 er derfor:
Involver dem du har tænkt dig at forandre så tidlig som muligt
Det er ikke altid en mulighed, men for det meste er det muligt tidlig at fortælle at noget er på vej, anvende
den viden som allerede er til rådighed og derved få en implementering, der starter lang tid før noget skal
ændres i praksis. Styrelsen for Arbejdsmarked og Rekruttering illustrerer det således:
Dette er uafhængigt af hvad det handler om. Der er både forsket og skrevet meget om ”Organizational
Change Management” se fx her eller her.
I afsnit 3.5 af disse noter, var der en kort gennemgang af Awareness, aktiviteter på dette område kan
udmærket bruges til at begrunde og anskueliggør behovet for en forandring, man taler ofte om muligheden
for at have en ”brændende platform” – hermed menes at det bliver kommunikeret på en måde så ”alle”
kan se der er et påtrængende behov for en forandring.
7.4.1 Implementering af Governance
Implementering af en ny sikkerhedspolitik og governance struktur, er også change management.
Her starter processen med ledelsen, det er i ledelsen at initiativerne på dette område skal initieres. Men
det udelukker naturligvis ikke at resten af organisationen skal informeres så tidligt det er muligt.
Ændringer af sikkerhedspolitikker, må antages at være begrundet i et ændret risikobillede eller ny
lovgivning, det er sådan set også det samme som hvis man reelt ingen sikkerhedspolitik har. Som det er
nævnt i kapitel 2, så skal sikkerhedspolitikker tilpasses det modenhedsniveau som virksomheden har – det
kan god konflikte lidt med at virksomheden måske også skal efterleve en regulering: der skal derfor findes
Side 122
en balance, som dels gør det muligt reelt at komme igennem med en implementering og som samtidig
efterlever de standarder som er nødvendige for at sikre compliance.
Men det starter med ledelsen. Medmindre initiativet til ændrede sikkerhedspolitikker kommer fra ledelsen
selv, så skal ledelsen overbevises om at det er nødvendigt, det er op til sikkerhedsorganisationen, en
ekstern konsulent eller måske bestyrelsen at sikre dette. Som oftest vil det være sikkerhedsorganisationen
der må konstatere at virksomheden befinder sig i et andet trusselsniveau end tidligere og at det
nødvendiggør ændrede politikker. Men sikkerhedsorganisationen skal sikre at ledelsen har forstået det
ændrede trusselsniveau og har accepteret nødvendigheden af ændringer. Når det er sikret, er det tid for
information til resten af virksomheden efter aftale med ledelsen.
7.4.2 Personlighedstyper
Der vil også i en projektorganisation være et behov for at få de rigtige persontyper til at stå for
implementeringen og koordinerer disse aktiviteter. De personer der har indkøbt eller udviklet er ikke
nødvendigvis gode til at sikre en fornuftig implementering. En implementering kræver fokus på processer
og mennesker.
Der findes et utal af modeller der illustrerer personlighedstyper fx DISC modellen:
Side 123
Så mon ikke den oplagte projektleder til implementering er en ”Gul” i DISC modellen. Der kan læses mere
om denne personlighedstype her.
ØVELSE: Hvordan skulle en ”Assurance Program” for Hvedebro Maskinfabrik organiseres? Dvs:
▪ Skal der anvendes eksterne konsulenter, hvis ja til hvad?
▪ Hvordan sikres en fornuftig implementering af et program?
Der er skrevet mange bøger og artikler om implementering, netop fordi det er et meget vanskeligt område
og noget som man aldrig bliver helt færdig med at forstå. Som beskrevet ovenfor er der en del psykologi i at
forandre mennesker og organisationer.
Helt essentielt er det ofte at den enkelte kan se sig selv i forandringen, forstår hvorfor og hvordan det
hænger sammen med virksomhedens strategi. Dette sammen med en løbende orientering om fremdrift er
et godt fundament for at sikre en effektiv implementering.
Side 124
8 Afslutning
Disse noter indeholder en gennemgang af de vigtigste principper indenfor Cybersikkerhed,
Informationssikkerhed eller hvad der nu er mest relevant at kalde det.
Noterne er derfor generelle, dog er afsnit om NIS2 skrevet om nogle gange, da lovgivningen omkring NS2
har være udsat flere gange, men nu er den vedtaget – pr. 1. juli 2025. NIS2 får en stor betydning for
sikkerhedsarbejdet i en lang række danske virksomheder, hvilket er også hele ideen fra EU: At styrke
Cybersikkerhed generelt i hele unionen.
Noternes formål er ikke at gå i dybden med alle områderne, dertil er emnet for stort. Noterne indeholder
en række henvisninger som kan bruges hvis der er specifikke emner der ønskes detaljeret. Noterne forsøger
at have en praktisk tilgang til sikkerhedsarbejdet, forsøger at undgå en teoretisk indfaldsvinkel.
Slutteligt er det forfatterens forhåbning at disse noter kan være inspirationskilde til yderligere fordybelse
og at de efter undervisningen vil kunne anvendes til opslag i en specifik arbejdssituation.
Sikkerhedsområdet står på ingen måde stille, det er et område i udvikling – men de basale begreber består
og ændres ikke. Det forventes at AI vil have en stadig stigende impact også på sikkerhedsarbejdet,
eksempelvis i opdagelse af sikkerhedsbrud men også i det daglige arbejde for medarbejdere i en
sikkerhedsafdeling.
Kurt Sejr Hansen
kurt@sejr-hansen.dk