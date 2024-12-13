# AI-seminarium

## AI och datalogiskt tänkande

### 01 

Vi fick ett mer utförligt svar från chatgpt, tydliga instruktioner med kodförslag medans aizo lämnar mer utrymme för tolkning. Chatgpt går mer på djupet och bryter ned varje enskild punkt i detalj medans aizos svar uppmuntrar för mer eget tänkande. Det här beror väl mycket på att Aizo inte är byggd för att förse frågor med direkta svar, utan är tänkt som en vägledare som leder studenten i rätt riktning. Medans chatgpt är lösningsorienterad, vilket gör att vi får ganska stora skillnader vid prompts som denna.

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

Vi testade båda versionerna och fick liknande resultat i konsolen. Här är vad som framkom under testerna:
Båda versionerna loggade varje enskilt kast i konsolen.
För varje kast kunde vi se vilket tal som genererades och om det var lyckat (matchade målet i stegen) eller ej.
Båda versionerna markerade tydligt när ett steg i stegen blev avklarat.
När spelet var slut, summerade båda versionerna antalet kast som behövdes för att klara hela stegen (1–6).
Resultaten varierade, men låg ofta inom ett rimligt intervall för slumpmässiga kast.
Totalt antal kast och spelets logik överensstämde mellan båda versionerna. Den största variationen kom från slumpen i tärningskasten, vilket förväntas i ett sådant spel.

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

Stora skillnader i hur chatGPT svarar på frågan (dock efter att jag startat en helt ny chatt) - efter att jag beskrivit för chatGPT vem jag är och hur jag vill att den ska agera så svarar den på ett väldigt pedagogiskt sätt, med lättförståeliga liknelser och skillnader i ett konkret programmeringsexempel. Det blir mer som att jag sitter med en lärare som vill att jag ska förstå snarare än någon som bara ger mig rätt svar utan någon som helst kontext eller intresse i att jag ska lära mig hur det faktiskt fungerar.

### 08

Stor skillnad! Med anpassning så fungerar ChatGPT mer som en lärare som förklarar varje steg, kommenterar koden så att man ska förstå vad varje rad gör, och kommer med exempel från "riktiga livet". När jag tog bort anpassningarna så fick jag bara koden rakt upp och ner, utan förklaring. Helt värdelöst!

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

Nikki tyckte att Github labs code brushes som städar upp ser otroligt nice ut. Emund tycker att det ser väldigt nice ut att copilot skriver bredvid och alltid ger förslag på färdig kod som man kan välja att implementera själv. Robin tycker att der ser väldigt effektivt ut och att man kan bli riktigt produktiv när man använder det på rätt sätt.

## AI i yrkeslivet

### 14

Robin är inte så orolig utan ser det mer som att det blir en global grej, eftersom AI kan ta många jobb i många olika branscher. Emund är inte heller särskilt orolig, men fundersam på hur svårt det blir att få sitt första jobb.

Nikki ser AI som ett verktyg, inte som en ersättare. Precis som en miniräknare inte ersatte mattelärare så kommer AI vara en hjälpande hand snarare än en ersättare. Det behövs fortfarande människor för att både träna och dubbelkolla, och det behövs fortfarande mänsklig problemlösning.

### 15

Nikki upplever att maskininlärningen ofta är utdaterad, och i o m att utvecklingen i branschen går väldigt snabbt så kan det vara svårt för verktygen att hålla sig relevanta. På temat säkerhet, så tänker nog inte AI:n alltid på hur sårbar koden möjligen är. Samtidigt kan den sakna kontext för hela projektet vilket kan göra att det ibland blir lite galet.

Emund är tveksam till hallucinationerna som AI:n gör, det kan ofta resultera i ett felaktigt resultat så det gäller att veta vad man gör så man kan rätta till koden själv.

Robin instämmer, och understryker hur viktigt det är att hela tiden fortsätta utveckla sitt eget kunnande och inte bli bekväm med att bara sitta och låta ett verktyg spotta ut AI-genererad kod, främst av anledningarna som nämns ovan. 

## AI Generellt

### 16

#### Tabnine

Tabnine är en AI-driven kodkomplettering som använder maskininlärning för att ge relevanta kodförslag i realtid. Den stöder en mängd programmeringsspråk och kan integreras med populära IDE:er som Visual Studio Code, IntelliJ IDEA och Sublime Text. Tabnine fungerar både lokalt och i molnet, vilket ger användaren flexibilitet kring sekretess och dataskydd. Verktyget är särskilt användbart för att snabba upp utveckling och för att föreslå kod baserat på projektets kontext.

#### Kite

Kite är ett AI-verktyg som fokuserar på att förbättra utvecklares produktivitet genom avancerad kodkomplettering. Det stöder språk som Python, JavaScript och Go och fungerar med flera populära textredigerare som Atom, PyCharm och VS Code. Kite erbjuder även funktioner som dokumentation i realtid och föreslår kodblock baserat på tidigare mönster i projektet. Verktyget har blivit uppskattat för sin enkelhet, även om dess stöd för vissa språk är mer begränsat jämfört med konkurrenter.

#### AWS CodeWhisperer

AWS CodeWhisperer är ett AI-verktyg från Amazon som hjälper utvecklare genom att generera kodförslag och automatisera repetitiva uppgifter. Det är djupt integrerat med AWS-ekosystemet och är särskilt kraftfullt för molnbaserade applikationer, med stöd för språk som Python, Java och JavaScript. CodeWhisperer är utformat för att förbättra utvecklingshastigheten och säkerheten genom att erbjuda förslag som följer bästa praxis och säkerhetsstandarder. Dess integration med molntjänster gör det till ett bra val för företag som använder AWS.

### 17

Github co-pilot samt github co-pilot labs. Av det vi sett av dessa verktyg än så länge så är vi övertygade om att både co-pilot och labs kan vara till stor hjälp i vårt framtida arbetsliv när det gäller att både effektivisera samt städa upp vårt arbete och vår kod i framtiden. 

Som studerande tänker vi att det kan användas som en extra hjälplärare som dessutom har tillgång till vår kod. Att kunna be den förklara koncept och ha direkt hjälp att tillgå utan att behöva hoppa fram och tillbaka är värdefullt som student.
