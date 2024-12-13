# AI-seminarium

## AI och datalogiskt tänkande

### 01 

Mer utförligt svar från chatgpt, tydliga instruktioner med kodförslag medans aizo lämnar mer utrymme för tolkning. Chatgpt går mer på djupet och bryter ned varje enskild punkt i detalj medans aizos svar uppmuntrar för mer eget tänkande.

### 02

Chatgpt genererar en mer generisk pseudokod som är lättare för en nybörjare att förstå, medans aizo förutsätter ett visst kunnande och genererar en pseudokod som är lite mer avancerad. Även i beskrivningen använder chatgpt mer nybörjarvänliga beskrivningar samtidigt som aizo använder begrepp som while-loop.

Starta spelet
    Definiera STEGE som en lista av mål: [1, 2, 3, 4, 5, 6]
    Sätt NUVARANDE_INDEX till 0 (börja med första steget)
    Sätt ANTAL_KAST till 0 (räkna antal kast)

    Upprepa så länge NUVARANDE_INDEX < längden på STEGE:
        Slumpa ett tal mellan 1 och 6 (TÄRNINGSKAST)
        Öka ANTAL_KAST med 1
        
        Om TÄRNINGSKAST är lika med STEGE[NUVARANDE_INDEX]:
            Öka NUVARANDE_INDEX med 1 (gå till nästa steg i stegen)

    När loopen avslutas:
        Skriv ut ANTAL_KAST som antalet kast som krävdes för att nå stegen

Avsluta spelet

Svaret från chatGPT

### 03

Testade båda och fick liknande resultat i konsollen. Båda loggade varje kast och om det var lyckat eller ej. De loggades även ut hur många kast totalt det resulterade i när spelet var slut.

## AI som studiekamrat

### 04

AI-verktyg kommer såklart överlag att fortsätta utvecklas och öka sin förmåga att lösa även mer komplexa problem i takt med att det matas in ny och mer utmanande data. Men för att hänvisa till torsdagens seminarium så ligger nog problemen snarare hos människan, att det krävs en förståelse för vad som byggs och vilka problem som bör lösas på vilket sätt. Med det sagt så är det svårt att på egen hand säga var begränsningarna går för dessa verktyg i dagsläget, men när vi frågar dom så får vi dessa svar.

Enligt chatgpt är dess begränsningar att:
- Jag kan inte interagera med externa API:er eller system i realtid utan hjälp av din lokala miljö.
- För mycket specialiserade eller domänspecifika problem kan det ta tid att sätta upp en lösning om jag behöver ytterligare kontext.
- Väldigt stora projekt (som ett helt system) är svåra att bygga på en gång, men jag kan ge dig en plan, startkoden och vägledning.

Samtidigt kan chatgpt jobba i betydligt fler språk så som exempelvis Python, Java, C++, C#, PHP etc medans aizos huvudfokus är HTML, CSS och Javascript. 

När vi frågade aizo vilka begränsningar den har, så svarar den först att den helst inte löser hela problemet, utan älskar att guida oss genom processen och ställa frågor som hjälper en att tänka själv, medans dess begränsningar är mer avancerade eller specifika områden utanför HTML, CSS och Javascript som till exempel maskininlärning eller vissa backend-teknologier.

### 05

Aizo kallar det för CSS-egenskap medan ChatGPT kallar det för CSS-regel. 

I övrigt så är ChatGPT mer utförlig i sina svar där den förklarar både hur man justerar positivt och negativt och har även en sammanfattning på slutet, medan Aizo ställer en motfråga. I övrigt är det väldigt lika i språkbruket.

### 06

Jag fick aldrig exakt samma kod tillbaka, utan det var små förändringar även om den största majoriteten var likadan. Jag upplever att den ibland justerar sin egen ändring, som att den inte riktigt vet själv vad som är rätt. 

Gällande .promise() och att den är utdaterad så tror jag det beror på att inlärningsmodellen är äldre och att den har lärt sig mycket på "gammal" kod vilket gör att den också föreslår "gammal" kod.

### 07

Stora skillnader i hur chatGPT svarar på frågan (dock efter att jag startat en helt ny chatt) - efter att jag beskrivit för chatGPT vem jag är och hur jag vill att den ska agera så svarar den på ett väldigt pedagogiskt sätt, med lättförståeliga liknelser och skillnader i ett konkret programmeringsexempel. 

### 08

### 09

Vi tycker att det är OK att använda AI för att:

- Få hjälp att lära sig koncept som är svåra att förstå<br>
Exempel: Vad är skillnaden mellan var, let och const?
- Få inspiration eller idéer<br>
Exempel: Hur kan jag strukturera denna komponent för återanvändbarhet?
- Felsökning<br>
Exempel: Varför får jag "undefined is not a function"?
- Automatisering av repetiva uppgifter<br>
Exempel: få hjälp att fylla i en json-fil med data
- Komplement till egen kodning<br>
Exempel: Kan du optimera den här funktionen så att den kör snabbare/använder mindre kod?

Vi tycker **INTE** det är OK att använda AI för att:

- Fuska, givetvis<br>
- Att undvika att lära sig<br>
Exempel: Att hoppa över att läsa en dokumentation för att istället få ett snabbt svar av AI
- Att ta AI-svaren utan att dubbelkolla<br>
Exempel: AI gör ofta fel, förstår du inte koden så kan du heller inte förstå vad felet är.

Sammanfattningsvis tycker vi att det är OK att se AI som en lärare eller mentor som förklarar hur något fungerar utan att ge lösningar. Vi tycker dock det är viktigt att inte lita blint på de svar vi får från AI.

### 10

Vi ser flera risker med att använda AI, men de tre största är:

- Begränsad förståelse för lösningen <br>
Om vi använder AI för att generera kod utan att förstå den så lär vi oss inte *hur* den fungerar eller *varför* den fungerar
- Lär oss inte att problemlösa <br>
Om vi använder AI för att lösa våra problem så riskerar vi att inte lära oss att problemlösa, utan istället att bara prompta en AI.
- Felaktig eller ineffektiv kod <br>
AI kan generera felaktig, utdaterad eller ineffektiv kod. Det krävs att vi kan och förstår för att vi ska kunna ta emot hjälp på ett bra sätt.

## AI som kodkompis

### 11

En klar styrka är att vi tillåts att effektivisera vårt arbete, dock är det såklart förutsatt att vi faktiskt vet vad vi pysslar med. Praktiskt att ha allt "in house", istället för att behöva hoppa fram och tillbaka mellan program vilket kan störa fokus. 

Risken är även här att vi använder för mycket "färdig" kod, och elementet av att tänka sig själv fram till en lösning riskerar att försvinna. Är nog en bra idé att till en början som student stänga av "auto complete" funktionen så att vi inte behöver oroa oss för att överanvända det.

### 12

Förutsatt att vi förstår och bottnar i det vi gör, så är det ett effektivt sätt att skynda på arbetsprocessen. Vill understryka här dock att det är bättre att använda verktyget för lite än för mycket, så att vi inte riskerar att fastna i en loop där vi inte behöver tänka så mycket själva innan vi faktiskt lärt oss grundligt.

### 13

## AI i yrkeslivet

### 14

### 15

## AI Generellt

### 16

### 17
