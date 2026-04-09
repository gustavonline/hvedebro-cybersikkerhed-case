

## Cybersikkerhed

## Modul 4: Teknik

Hvad skal vi igennem
•Basal IP viden
•Firewall og netværkskomponenter
•Netværksarkitektur
•Log Managemenet
•IoT
•SCADA og OT
•WiFi
•Kryptering
•Cloud
•Zero -Trust
## Reference: Information Noterne

Basal IP viden - historien
•Historien – ARPANET (1960)
•Første e-mail i 1971  (min første i 1989)
•Web 1.0 i 1989 (Tim Berners Lee)
•Web 2.0 i 1999  (det sociale internet)
•OpenSource bevægelsen .....
•Web 3.0 i 2014 ”The Semantic Web” – AI
•rfc – hvor standarder dannes
## Reference: Information Noterne

Basal IP viden - teknik
## Reference: Information Noterne
IP adresse: 0.0.0.0 til 255.255.255.255
MAC adressen: 48 bit = 2
## 48
muligheder
Dynamisk og statiske IP adresser
NAT: ”Network Address Translation”
Iplocation.net giver dette resultat:

xxxxxxxxxxxxxxxxxxx
Reference: Information Secuity Management Principles, Third edition – Chapter:6 og noterne
”192.168.0.0/24”, dette betyder at 24 bit (3
oktetter) er netværksadressen og de sidste 8 bit
er så host adresser.
Adresserummet 192.168.0.0 til 192.168.0.255,
tidligere blev dette kaldet en klasse C adresse,
men det anvendes ikke så ofte mere.
Oktet = en byte = 8 bit

Basal IP viden – teknik - port nummer
•Port 0 til 1023: Veldefinerede porte, defineret og godkendt af IANA (Intrnet Assigned
## Numbers Authority)
•Port 1024 til 49151: Kan bruges af udviklere og kan registreres
•Port 49152 til 65536: Bruges af klientprogrammer, en session tildeles et port
nummer
•Eksempler på port nummer allokeret til bestemte protokoller:
•Port 80: HTTP
•Port 25: SMTP
•Port 123: NTP
•Port 161: SNMP
## Reference: Information Noterne

Basal IP viden – teknik - teknologier
## •NAT
## •DHCP
## •BGP
## •UDP/TCP
## Reference: Information Noterne

IP kommandoer på eget udstyr – prøv det!
•Ipconfig /all – find, hostname, IP adressen, subnetmask, MAC adresse, og default gateway
•Netstat – se hvilke forbindelser der er aktive, portnummer?
•Tracert www.dr.dk – hvor mange step er der til www.dr.dk
•Ping www.dr.dk – hvor lang er forsinkelsen til www.dr.dk
•Difo.dk – varetager den danske del af internettet
•punktum.dk – administration af DK domæner
## Reference: Noterne
## MAC?:
ipconfig getsummary en0
pconfig /all – find  -> ipconfig getsummary en0
Netstat->lsof -nP -iTCP -sTCP:LISTEN
Tracert www.dr.dk-> traceroute www.dr.dk

Øvelse – IP basic
•Find en offentlig tilgængelig service, hvad er den officiel IP adresse og hvor i verden er den – er
der anden interessant info at finde?
## Reference: Noterne

Netværks komponenter

Basal IP viden – teknik - Firewall
•Hvorfor anvende en Firewall
•Regulere hvilken type af trafik der må komme hvorfra og hvortil
•Liste IP-adresser der må kommunikere
•Sikre at trafik på den ene net ikke flyder over i det andet net
## Reference: Information Noterne

Basal IP viden – teknik - DMZ
## Reference: Information Noterne

Konfiguration FW – (hjemmenetværk)
## Reference: Information Noterne
Typisk er der mange konfigurationsmuligheder
ofte har ISP bestemt

Konfiguration hjemmenetværk - trafikeksempel
## Reference: Information Noterne
IPS: Intrusion Prevention System
IDS: Intrusion Detecting System

Sårbarhedsscanning og Pentest
•Sårbarhedsscanning (Intern og ekstern)
•Afslører typisk manglende patching eller forkert konfiguration
•RedTeam – BlueTeam
•Automatisk
•WhiteHat
•Fysisk
•Social
•Awareness – fx. illustration af e-mail, phishing angreb
## Reference: Noterne
Begge teams kan være interne

Netværksarkitektur og komponenter
## Reference: Noterne

Firewall typer
TypeAnvendelseBegrænsninger
PakkefiltreringDen mest anvendte, er installeret som
standard i næsten alle routere
Ikke i stand til at inspicere indholdet af pakkerne (dvs. ingen dybdegående
analyse af applikationstransaktioner eller data), hvilket gør den sårbar over
for visse angreb som f.eks. IP-spoofing
Stateful Inspection FWKaldes også en dynamisk FW. Tillader fx kun
pakker der er en del af en eksisterende
session
Mere kompleks og ressourcekrævende end pakkefiltrering, men stadig ikke
i stand til at analysere indholdet af applikationstransaktioner.
Proxy FWEt mellemled mellem bruger og ressourcer
som der ønskes adgang til. Mulighed for
mere dyberegående inspektion
Kan introducere forsinkelse og er mere ressourcekrævende. Kan kun
arbejde med specifikke applikationer.
Next Gen FWKombinerer forskellige funktion, kan lave
pakke inspektion i dybden, malware analyse
og IPS mv.
Kan være dyrere og mere kompleks at implementere og administrere.
Web App FWPrimært til beskyttelse af WEB applikationer,
mod fx SQL injection, XSS og lign
Kan være målrettet af avancerede angreb, og kræver ofte løbende justering
af regler for at være effektiv.
Circuit level GatewayOvervåger transportlager, anvendes typisk i
forbindelse med VPN
Ingen dybdegående inspektion af applikationens indhold og risikerer at
tillade visse angreb.
Hybrid FWKombination af ovenståendeEr dyrere og mere kompleks at implementere og administrere.
## Reference: Noterne

WiFi standarder og debat
## Reference: Noterne
Er det risikofrit at anvende WiFi?
Hvad med på et hotel?

WiFi risici ved anvendelse af offentlige HotSpot
•Der opsættes et falsk HotSpot, dem der forbinder sig bliver så aflyttet, også selvom der i ”luften”
er forhandlet en god kryptringsprotokol
•Der aflyttes mellem WiFi HotSpot og til det øvrige netværksudstyr, her sker kommunikationen
ukrypteret, dette kaldes normalt ”Man-in-the-middel attack”, her kan fx aflyttes brugernavne og
kodeord.
•En scanner opsamler store mængder datamængder, bruger så lang tid på at dekode
kommunikation og finde brugernavne og kodeord
•Dårlig konfigureret WiFi HotSpot, fx kan standard admin kodeordet ikke være ændret, eller det er
meget simpelt og sikkert aldrig ændret
## Reference: Noterne

Reducer risici ved anvendelse af offentlige HotSpot
•Brugen af MFA, bevirker at selvom dit brugernavn og kodeord er gættet, ja så kan det
ikke/vanskelig udnyttes da det kræver ”Something you have”.
•Brugen af en passwordmanager kan reducere risici, da det er vanskeligere at gætte fx et 12 tegns
autogenereret kodeord.
•End2End kryptering, brugen af VPN til den virksomhed man ønsker forbindelse til, eller generelt
at anvende en VPN også privat – VPN-forbindelse til et sikkert sted.
## Reference: Noterne
Erfaringer med anvendelse af HotSpots?

Øvrige netværkskomponenter
•Mest anvendt er en ”lag2 switch” – kan være administrerbar.
•VPN server
## Reference: Noterne

## Øvelse – Hvedebro Maskinfabrik
•Hvad bør/kan Hvedebro Maskinfabrik tage stilling til omkring et nyt
netværksdesign, formuler nogle verbale forslag
## Reference: Noterne

## Logning

## Logning
•Hvorfor logning?
•Hvad skal logges?
•Lovgivning?
## •ISO27002: (8.15)
•Definerede scenarier
•Tillid?
•Hvem afgør hvad der skal
logges? (oppefra/nedenfra)
•Syslog
•Events=hændelse
## Reference: Noterne

Logning – mulige scenarier
•Log Management systemets egne scenarier = den nemme løsning
•Virksomhedens risici
•De mest værdifulde assets
Business eksempler:
•Er der en kundeservice medarbejder der mere en X gange i døgnet har set på en
kundes fortrolige data?
•Er der en salgsperson som downloader store mængder kunde data?
•Hvad laver en opsagt medarbejder de sidste dage?
•Er der medarbejdere der downloader store mængder af data?
## Reference: Noterne

DashBoard eksempel:
## Reference: Noterne

Logning - debat
•Hvordan kommer man frem til hvad der er relevant at logge?
•Hvad giver god mening som minimum at logge?
## Reference: Noterne

Internet of things, Scada og OT

Hvad er IoT – er der noget nyt set med sikkerhedsbriller?
## Reference: Noterne
## Protokoller:
•Zigbee
•Z-Wave
•Matter
## •BT
•WiFi
## •4G/5G

IoT anvendelse
## Reference: Noterne

IoT og sikkerhedsudfordringer
•Sikker krypteret kommunikation mellem enhed og ”central” og mellem enhederne selv (MESH).
•Autentifikation og Authorization, hvem er det er beder om data og hvilke rettigheder har de, må
man fx lave en software opdatering, også kaldet OTA. Et af de klassiske eksempler er adgang til
små kameraer som man måtte have i hjemmet eller på arbejdspladsen.
•Kan man stole på de softwareopdateringer, der muligvis kommer – OTA, bliver enheder
opdateret?
•Er det data der ligger i cloud, hvem har så adgang til disse og hvornår
•Ofte er IoT enheder fordelt over et stort område, så der kan være problemer med
tilgængeligheden og de problemer det giver med manglende opdateringer
•Redundans ved fx industrisystemer
•Power – energy harvesting
## Reference: Noterne

Demo af Home Assistant
•Link
## Reference: Noterne

SCADA og OT
•Typiske udfordringer på sikkerhedsområdet er:
•Gammel teknologi der gøres tilgængelig via IP
•Manglende viden om Cybersikkerhed – manglende opdateringer
•Udgået teknologi, der findes ingen patches
•Man ved ikke helt hvad man reelt har, hvad indeholder maskinen
•Hvad gør man?
•Sikre adgang til OT enheder
•Asset Management, få styr på hvad man har hvor
•Sårbarhedsscanning, patch management – opdateringer!
•Netværks segmentering
•Backup
## Reference: Noterne

OT – Operational Technology
•En fabrik
•I et vandværk
•Vindmøller
•Kraftvarmeværker
•Renseanlæg
•Svømmehal
•Hospitalsenheder
•Centrallager
•Atomkraftværk
•Facility management
## Reference: Noterne

OT – Operational Technology
## Reference: Noterne
## Edge Computing
OT Standard: IEC62443

IEC62442 – hvad indeholder denne standard?
## Reference: Noterne
Generelle principper og rammer
•IEC 62443-1-x: Definerer overordnede principper for cybersikkerhed i industrielle systemer og beskriver rammerne for implementering af
sikkerhedsforanstaltninger.
Sikkerhedsprocesser og styring
•IEC 62443-2-x: Omhandler styring og implementering af sikkerhedsprocesser, herunder hvordan organisationer kan etablere og opretholde
sikkerhedsprogrammer for industrielle systemer.
System- og netværksinfrastruktur
•IEC 62443-3-x: Fokus på at designe og implementere cybersikkerhed for selve systemet og netværksinfrastrukturen, som styrer industrielle applikationer.
## Komponentbeskyttelse
•IEC 62443-4-x: Behandler cybersikkerheden for de enkelte komponenter i industrielle systemer, såsom hardware, software og enheder. Den adresserer
sikkerhedsforanstaltninger på lavere niveau, som sikrer integriteten af både hardware og software i systemet.
Sikkerhedskrav til leverandører
•Standarden stiller krav til leverandører af industrielle systemer om at implementere cybersikkerhedsfunktioner, der kan beskytte deres produkter mod
kendte trusler.

OT – Operational Technology - designprincipper
## Reference: Noterne
Risikostyring: Identificere og vurdere risici tidligt i udviklingsprocessen og implementere passende
modforanstaltninger.
Sikkerhedsstandarder og bedste praksis: Følge etablerede sikkerhedsstandarder og -principper,
som for eksempel "least privilege", "defense in depth", og OWASP, ISO27001/2, IEC62443 .....
Trusselmodellering: Analysere potentielle trusler og sårbarheder, og tage skridt til at mitigere dem
før systemet tages i brug.
Sikkerhedsfeedback: Inkorporere feedback fra sikkerhedstestning og overvågning gennem hele
udviklingscyklussen for at forbedre systemet kontinuerligt.
Opdatering og patching: Designe systemet, så det nemt kan opdateres og patches kan
implementeres hurtigt for at forhindre udnyttelse af kendte sårbarheder.

## Kryptering

## PKI
•Public Key infrastructure, nøgler fås via ”Certificate Authority”
•Private Key Infrastructure
•Private nøgler
•Offentlige nøgler
•Uafviselighed (non repudiation)
## Reference: Noterne
Certifikat (har en bestemt gyldighed)

Symmetrisk vs Asymmetrisk kryptering
•Symmetrisk: Samme nøgle til kryptering og dekryptering
•Asymmetrisk: To nøgler, en offentlig og en privat nøgle
•Nøglelængder:
•Symmetrisk – typisk 128 til 256 bit
•Asymmetrisk – op til 512 bit
•Krypterings standarder bl.a.:
•Advanced Encryption Standard (AES)
•RSA (Opfindernes efternavne)
## Reference: Noterne

Anvendelse af nøgler
## Reference: Noterne
Fortrolighed, integritet og uafviselighed:
1.Krypter med egen private nøgle
2.Krypter med modtagers offentlige
nøgle
3.Send
4.Modtager dekryptere med egen
privat nøgle
5.Modtager dekrypter med senders
offentlige nøgle
## Uafviselighed:
1.Krypter med egen private nøgle
2.Send
3.Alle med offentlig nøgle kan
dekrypterer
## Kryptering
1.Krypter med modtageres offentlige
nøgle
## 2.send
3.Modtager er den eneste der kan
dekryptere med sin private nøgle

Hvordan virker https?
1.Hello – klient –server kommunikation. Klienten starter, der svares tilbage med
ServerHello – bl.a. SSL versionen og andre basale data.
2.Certifikat udveksling, Server sender offentlig nøgle til klient og anden
information, domain, owner, status mv. Klienten kan nu spørge CA om certifikat
er valid.
3.Nøgle udveksling – der udveksles den symmetriske nøgle som anvendes både til
kryptering og dekryptering. Hvis begge parter er ok så:
4.Kommunikationen starter.
## Reference: Noterne

## Øvelse
1.Åben en browser, gå til mitid.dk
2.Undersøg om det bliver en sikker forbindelse
3.Find status på signatur og hvem der har udsted det, hvornår udløber det?
4.Hvem ejer certifikatudstederen?
5.Find den offentlige nøgle
## Reference: Noterne

## Cloud

Cloud computing historie
•1996 – Compaq lavede en business plan for det vi i dag kender som cloud
computing
•2000 – Amazon udvider eget datacenter og starter introduktionen af AWS
•2007 - Google kommer med, introducerer Google Docs
•2010 - Microsoft introducerer Microsoft Azure
Men ideen stammer tilbage fra 1960’erne, her afleverede man jobs til et datacenter,
som så blev kørt efter aftale.
## Reference: Noterne

Cloud teknologi
SaaS (Software as a Service)
Adgang til en applikation er SaaS, således noget vi alle anvender i praksis, som oftest er disse services
betinget af at man har tegnet et abonnement, Office365 er et godt eksempel, men der kan også være
tale om gratis services, fx gmail.
PaaS (Platform as a Service)
Anvendes fx. i udviklings sammenhæng, her kan PaaS levere et komplet udviklingsmiljø, kan fx
inkluderer database services, holde styr på versioner, programmeringssprog mv.
IaaS (Infrastructure as a Service)
Kan fx. være server, fysiske eller virtuelle, med et bestemt operativsystem, storage eller databaser –
dvs. helt grundlæggende infrastruktur komponenter som man så har valgt at have som en cloud
service.
## Reference: Noterne

Cloud computing drivers
•Omkostninger
•Lokations uafhængighed
•Vedligehold
•Skalerbarhed
•Tilgængelighed
•Sikkerhed
## •DR
## Reference: Noterne

Cloud og sikkerhed
## Reference: Noterne

Skal man være bekymret for cloud?
•Kan en af de store udbydere gå konkurs?
•Hvem tænker på at man måske skal flytte til en ny udbyder?
## Reference: Noterne

Overvejelser - debat
•Er cloud noget for Hvedebro Maskinfabrik?
•Hvis til hvilket formål?
•Hvilke risici er der ved anvendelse af en cloud leverandør til x,y,z i forhold til at
have det selv?
## Reference: Noterne

## Zero Trust

## Zero-trust
•En virksomhed har ingen perimetrigrænse
•Principper – bl.a. arkitekturprincipper
•Alle kommunikationskanaler skal sikre, fx via kryptering
•Klassifikation af assets
•Anvend kraftig segmentering af netværk, også kaldt mikrosegmentering – ultimativt et
segment pr. asset
•Adgang gives på ”pr session” basis. Dvs. ikke en permanent adgang.
•Stor grad af overvågning
•Sikre former for autentifikation og autorisation samt MFA
•Bruges det?
## Reference: Noterne

IT-arkitekt og Cybersikkerhed

Overordnede principper
Som IT-arkitekt er det vigtigt at tage et helhedsorienteret ansvar for
cybersikkerheden i alle aspekter af systemdesignet. Dette kræver en systematisk
tilgang, der involverer både tekniske foranstaltninger (kryptering, adgangskontrol,
netværkssikkerhed) og organisatoriske processer (incident response, compliance).
Arkitekten skal også være opmærksom på den konstante udvikling af nye trusler og
sikre, at systemet er fleksibelt nok til at håndtere fremtidige sikkerhedsudfordringer
Reference: Information Secuity Management Principles, Third edition – Chapter:3

Det helhedsorienterede
•Trusselsmodellering og risikoanalyse
•Security By Design
•Datasikkerhed
•Adgangskontrol og Autentifikation
•Netværkssikkerhed
•Sårbarhedsstyring og Patch Managenet
•Intrusion detection og prevention
•DevSecOps
•Incident responce og gendannelse af data/app/system
•Compliance
Reference: Information Secuity Management Principles, Third edition – Chapter:3

## Feedback

## Feedback
•Hvordan opleves dette modul?
•For meget eller for lidt information?
•Var detaljeringsniveauet passende?
•Praktisk/teoretisk, var det ok?
•Var øvelserne ok?
•Andet?
Reference: Information Secuity Management Principles, Third edition – Chapter:3