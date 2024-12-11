# Computational Thinking - Air Bean Group Project
**Fantastic Scientists**

Länk till vår FigJam hittas [här](https://www.figma.com/board/u1q68FuFGJBPCwfCQcJlxe/Computational-Thinking---Group-Project?node-id=0-1&node-type=canvas&t=PhDZA7ApaRL6y3W7-0).

## Decomposition

Vi har delat upp applikationen utefter i fyra olika kategorier: **Produkter**, **Kundhantering**, **Kassa** och **Leverans**. Varje kategori innehåller sina egna specifika funktioner och processer som bidrar till att skapa en sammanhängande och användarvänlig tjänst.

**Produkter** inkluderar hanteringen av produktdetaljer såsom namn, pris och beskrivning, vilka lagras i en dedikerad databastabell. Vi gör ett antagande att systemet erbjuder rekommendationer och möjligheten att visa de senaste beställningarna, baserat på användarens beteende och preferenser. Även dessa data hanteras via en separat databastabell.

**Kundhantering** täcker flera aspekter av användarens interaktion med applikationen. Det inkluderar autentisering och lösenordshantering vid inloggning, tillsammans med en registreringsprocess som validerar användarinformation och sparar den i databasen. Dessutom erbjuds kundservice i form av en informationssida, en chattfunktion som vi gör ett antagande att det finns och övriga kontaktalternativ. Kundprofiler gör det möjligt för användare att hantera sina konton, inklusive redigering av inställningar, så som betalningssätt, leveransadress och kontoinformation. En viktig funktion i denna kategori är också tillgången till orderhistorik.

**Kassa** är optimerad för att göra betalningsprocessen enkel och säker. Den hanterar varukorgen, olika betalningsalternativ och möjligheten att använda rabattkoder. Sparade betalningsmetoder lagras i en skyddad databastabell, vilket säkerställer hög säkerhet och snabb åtkomst vid framtida beställningar. Själva betalningssystemet måste också skötas på ett säkert sätt.

**Leverans** fokuserar på att informera användaren om leveransen. Efter en beställning genereras en orderbekräftelse som inkluderar ett unikt ordernummer och en uppskattad leveranstid. Användaren får även möjlighet att följa leveransen via realtidsuppdateringar (återigen, ett antagande från vår sida), vilket förbättrar transparens och tillfredsställelse. Viktiga data som ordernummer och leveransinformation lagras i dedikerade databastabeller för korrekt hantering och spårning.

## Pattern recognition
Här blickade vi ut över vår decomposition för att försöka hitta alla möjliga typer av gemensamma nämnare. Vi hade till en början lite problem med att skilja på vad som borde finnas under pattern recognition och vad som borde vara under abstraction. Det vi så småningom landade i var att abstraction handlar om att förenkla och dölja oväsentliga detaljer, medan pattern recognition helt enkelt handlar om att identifiera mönster och skapa lösningar som kan återanvändas. Som exempelvis hamburgemenyn eller varukorgen. Men även sånt som användarbeteende, vilket kan vara användbart i en sån här typ av app då det exempelvis kan vara bra för kunden att kunna lagra sin betalningsinformation, adress, samt att få en anpassad meny där exempelvis "Du beställde senast" eller "Du kanske också gillar" återfinns överst på menyn.

Summan av vårt resonemang här var att vi vill göra det så enkelt för våra framtida jag som möjligt, så när vi i det inledande skedet bryter ner helheten i mindre beståndsdelar så fortsätter vi processen med hjälp av pattern recognition genom att hitta olika områden av problem som kan lösas på ett gemensamt sätt.

## Abstraction

Applikationen är utformad för att leverera en enkel och effektiv upplevelse för användaren, med fokus på de mest grundläggande och viktiga funktionerna. Användaren ska kunna se en tydligt presenterad lista över tillgängliga drycker, vilket möjliggör en snabb och smidig navigering. Därefter kan användaren välja en eller flera drycker för att lägga till i sin beställning. För att göra processen så bekväm som möjligt ges användaren möjlighet att genomföra sin order direkt, utan att behöva gå igenom krångliga steg. Efter beställningen ska användaren enkelt kunna följa sin orderstatus, från att beställningen är mottagen till dess att leveransen är på väg. Slutligen ska användaren kunna ta emot sin beställning via en smidig leveransprocess.

Utöver dessa kärnfunktioner erbjuds användaren ytterligare möjligheter för en mer personaliserad upplevelse. Genom att skapa ett konto och logga in kan användaren spara sin information och därmed förenkla framtida beställningar. En inloggad användare får dessutom tillgång till en historik över tidigare beställningar, vilket ger ökad transparens och enkel åtkomst till sina favoritval. Dessa tilläggsfunktioner är valfria och påverkar inte möjligheten att använda tjänsten som gäst.

## Algorithm design
När det till sist var dags att göra vår algorithm design så valde vi att bryta ned det till ett flöde för varje menyalternativ, även då uppgiften egentligen var att beskriva flödet från att användaren landar på sidan till att beställningen är lagd.

Vi landar först på splashsidan, tar oss därifrån till menyn, och beroende på vilka val vi gör därefter så har vi beskrivit de olika utfallen, fram tills dess att en order blir lagd.

Det intressanta här var att få zooma ut lite och få en helhetsbild över hur processen faktiskt ser ut. Men överlag inga konstigheter utan i o m förarbetet vi gjort som ledde fram till vår algorithm design så flöt den här delen av uppgiften på smidigt.

### Initial startup av applikation

Användaren startar applikationen och hamnar på en "splashsida", bilder i Figma med "AIR BEAN" och grön bakgrund. Efter det så hamnar användaren på menysidan, där den har följande val:

- Hamburgermeny
- Varukorg
- Lista på drycker

### Hamburgermenyn

Använder sig kunden av hamburgermenyn så finns det fyra val:

- Meny (där vi är just nu)
- Vårt kaffe
- Min profil
- Orderstatus

### Meny

Listan på drycker innehåller detaljer om drycken (namn och ingredienser), pris och en knapp för att lägga till. När användaren trycker på lägga till så hamnar det i varukorgen. I varukorgen sedan så kan användaren se varor, för att sedan bekräfta beställningen. Här gör vi ett rimligt antagande att kunden behöver fylla i namn, adress och betalsätt. När användaren har bekräftat beställningen så lagras den i en databas tillsammans med ett unikt ordernummer och en bekräftelse visas med ordernumret och uppskattad leveranstid.

### Vårt kaffe

Information om Air Bean från bolagets VD och grundare. Detta är en strikt informationssida så det finns inga flöden eller antaganden att göra. Kunden kan använda hamburgermenyn för att navigera till en annan sida.
 
### Min profil

Trycker kunden på Min profil i menyn så gör vi ett rimligt antagande baserat på skissen att kunden hamnar på en inloggningssida. Det finns en länk under inloggningsformuläret ifall kunden vill skapa ett konto. Om kunden försöker logga in så behöver formuläret valideras och autentiseras mot databasen. Om båda dessa lyckas så hamnar kunden på sin profilsida och kan se bland annat orderhistorik. Vi gör ett antagande att kunden även kan göra andra inställningar här, som ändra lösenord, välja ett förvalt betalsätt och leveransadress med mera. Om kunden vill skapa ett nytt konto så hamnar den på en ny sida där den kan registera sina uppgifter. Även här behöver formuläret valideras och autentiseras, här behöver också en extra kontroll göras så att användarnamnet/epostadressen inte redan är i bruk. Om det är OK så lagras uppgifterna i databasen och kunden skickas tillbaka till inloggningssidan.

### Orderstatus

Här gör vi ett antagande att orderstatus visar en pågående beställning, så kunden bör då skickas till samma sida som den hamnar på efter en bekräftad beställning, som visar ordernummer och uppskattad leveranstid.
