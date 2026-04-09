# Bilag – AI-politik og AI-audit (Hvedebro)

Dette bilag operationaliserer AI-delen i IT-sikkerhedspolitikken.

## 1. Formål
At sikre, at brug af AI skaber værdi uden at kompromittere fortrolighed, integritet, tilgængelighed, compliance eller IP-beskyttelse.

## 2. Omfang
Gælder for alle AI-værktøjer, herunder:
- Generativ AI (tekst, kode, billede)
- Copilots i Office/udviklingsværktøjer
- AI i leverandørprodukter (fx OT-overvågning)

## 3. Grundregler
1. **Kun godkendte AI-værktøjer** må bruges i arbejdstid.
2. **Forbudt input:** CAD/IP, kundedata, persondata, kontrakter, sikkerhedshændelser og andre klassificerede data i uautoriserede AI-tjenester.
3. AI-output skal kvalitetssikres af en medarbejder før brug i beslutninger, kundesvar eller tekniske ændringer.
4. AI må ikke bruges til at omgå sikkerhedskontroller, adgangsstyring eller compliancekrav.

## 4. AI-risikoklasser
- **Lav:** Idégenerering uden fortrolige data
- **Middel:** Intern produktivitet med anonymiserede data
- **Høj:** Output påvirker drift, kundekommunikation, sikkerhed eller compliance
- **Kritisk:** AI i OT, beslutningsstøtte til sikkerhed, eller behandling af følsomme data

Høj/kritisk AI-brug kræver formel risikovurdering og ledelsesgodkendelse.

## 5. AI-audit (kvartalsvis)
### Minimumskontrol
- Opdateret register over anvendte AI-værktøjer
- Datakilder, datatyper og dataflow dokumenteret
- Leverandørvurdering (sikkerhed, datalagring, underdatabehandlere)
- Adgangsrettigheder og logning verificeret
- Kontrollér at forbudte datatyper ikke anvendes
- Kontrol af hallucinations-/kvalitetsrisiko i kritiske processer

### KPI’er
- Andel AI-værktøjer med godkendt risikovurdering
- Antal AI-relaterede policybrud
- Andel medarbejdere med AI-awareness gennemført
- Andel høj/kritisk AI-use-cases med dokumenteret human review

## 6. Roller
- **Informationssikkerhedsansvarlig:** ejer AI-governance og auditprogram
- **Data-/systemejere:** godkender AI-use-cases i eget område
- **IT:** teknisk kontrol, logging og adgangsstyring
- **HR/Ledelse:** træning og håndtering af policybrud

## 7. Hurtig implementering (90 dage)
1. Udgiv AI-regler i kort version (1 side til alle medarbejdere)
2. Etabler AI-register (værktøj, formål, data, ejer, risikoklasse)
3. Spær uautoriserede AI-tjenester hvor muligt
4. Gennemfør målrettet awareness (ledelse, udvikling, kundeservice, økonomi)
5. Kør første AI-audit og rapportér resultater til direktionen
