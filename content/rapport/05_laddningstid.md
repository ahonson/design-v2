---
---
Laddningstid (kmom05)
=========================

Detta innehåll är skrivet i markdown och du hittar innehållet i filen `content/rapport/05_laddningstid.md`.

Syftet med denna uppsats är att mäta och analysera laddningstiden hos tre webbplatser med liknande struktur och innehåll samt att dra slutsatser gällande vilka åtgärder som kan vidtas för att minska de uppmätta värdena och på så sätt förbättra webbplatsernas UX.

Urval
-----------------------
Public Service har till uppdrag att informera allmänheten om aktuella händelser, att underhålla, att utbilda mm. Detta innebär att stora mängder av data ska levereras till användarna med rimliga laddningstider. Jag har valt att analysera tre statliga nyhetskanaler med jämförbar struktur: Storbritanniens [BBC](https://www.bbc.com/), Norges [NRK](https://www.nrk.no/) och Danmarks [DR](https://www.dr.dk/). Förutom hemsidorna analyseras även undersidorna där användaren kan nå nyheter och radiokanaler. Anledningen till att jag inte tog med svensk public service i urvalet är att dess struktur är annorlunda: motsvarande information är placerad på två separata sajter ([SR](https://sverigesradio.se/) och [SVT](https://www.svt.se/)) och nås inte från en enda webbplats.

Metod
-----------------------

Jag samlade in de relevanta uppgifterna om de utvalda webbplatsernas prestation med hjälp av webbläsarens inbyggda DevTools (Chrome 79 för Windows 10) och med hjälp av onlineverktyget [Page Speed Insights](https://developers.google.com/speed/pagespeed/insights/) (PSI). Från DevTools hämtades information gällande laddningstider, antalet begäran och filstorlek medan PSI-värdena och förbättringsförslagen hämtades från PSI.

Förutom hemsidan analyserades två undersidor (nyheter, radio) för varje webbplats i urvalet. Eftersom varje sidladdning ger (eller kan ge) olika resultat bestämde jag mig för att beräkna fem sidladdningars medelvärde för varje sida och att endast ta med de genomsnittliga värdena i [bilagan](https://docs.google.com/spreadsheets/d/1tXWC8Cfl3cJemy4D-QO_k8orKxADwSxS0VZjqy8yKPE/edit?folder=0AGIscMfz0fNxUk9PVA#gid=0). Undersökningen genomfördes både för desktop och för mobil.

Resultat
-----------------------

De uppmätta värdenas medelvärden sammanfattas i detta [Excel ark](https://docs.google.com/spreadsheets/d/1tXWC8Cfl3cJemy4D-QO_k8orKxADwSxS0VZjqy8yKPE/edit?folder=0AGIscMfz0fNxUk9PVA#gid=0), medan förbättringsförslagen finns att läsa i [denna flik](https://docs.google.com/spreadsheets/d/1tXWC8Cfl3cJemy4D-QO_k8orKxADwSxS0VZjqy8yKPE/edit#gid=73654095) av samma ark.

### Storbritanniens [BBC](https://www.bbc.com/)

![BBC:s hemsida](image/rapport/05_laddningstid/bbc.png)

PSI-värdena för BBC:s sajter hamnade mellan 34 och 83 på mobil och mellan 72 och 99 på desktop. DOMContent laddades inom en sekund, medan de blockerande resurserna laddades inom två sekunder för samtliga sidor (både på mobil och desktop).

Det som skulle kunna bidra mest till att minska laddningstiden på desktop är att eliminera blockerande resurser (som CSS / JS-filer) genom att tillämpa dem som inline CSS / JS. Den mest effektiva optimeringsåtgärden för mobiler skulle vara att senarelägga laddningen av icke-synliga bilder.

Den överförda datamängden är alltid begränsad till högst 2 MB, vilket gör att webbplatsen utmärker sig med snabba laddningstider och bra PSI-värden trots att antalet begäran ligger på mer än 100.

### Norges [NRK](https://www.nrk.no/)

![NRK:s hemsida](image/rapport/05_laddningstid/nrk.png)

PSI-värdena för NRK:s sajter hamnade mellan 28 och 70 på mobil och mellan 78 och 99 på desktop. När det gäller desktop fick NRK alltså något bättre resultat än BBC och betydligt bättre än DR. På BBC:s och NRK:s nyhetsflik såg PSI ingen förbättringsmöjlighet (PSI kom endast med diagnostiska kommentarer som inte påverkar laddningstiden avsevärt.)

För mobilen fick NRK samma feedback som BBC gällande blockerande resurser men utöver detta ska även bildhanteringen förbättras på nyhetsfliken. Förslagsvis skulle man kunna optimera bildstorleken och tillhandahålla bilderna i ett annat format (next-gen).

Den överförda datamängden skilde sig inte markant mellan desktop och mobil. Emellertid var det senare mera begränsat för nyhetsfliken vars mobila laddningstid uppmättes att ligga på mer än två sekunder.

### Danmarks [DR](https://www.dr.dk/)

![DR:s hemsida](image/rapport/05_laddningstid/dr.png)

PSI-värdena för DR:s sajter hamnade mellan 10 och 37 på mobil och mellan 63 och 76 på desktop. Därmed har DR det klart sämsta resultatet bland webbplatserna i urvalet för både desktop och mobil. I och med att DR fick nästan lika många anmärkningar (26) som BBC och NRK tillsammans (27) är listan på potentiella förbättringar ganska lång. Det som bör lyftas fram som viktigast är åtgärder rörande bildhantering. Hälften av DR:s samtliga förbättringsförslag gäller just denna kategori.

Det skulle också löna sig att ta bort blockerande resurser och onödig CSS på den mobila varianten, särskilt på nyhetsfliken som fick ett all titme low resultat på två poäng. Där skulle man också kunna tänka sig prioritera laddningen av viktiga begäran (pre-load key requests) samt minifiera JavaScript och komprimera texten (enable text compression).

Det låga resultatet kan till viss del skyllas på den genomförda datamängden som verkar onödigt stor (21.3 MB) jämfört med BBC (4.6 MB) och NRK (7.4 MB), men också på antalet filer som laddas av webbläsaren. Siffran rör sig kring 300 när det gäller radiofliken.

Analys
-----------------------

Det ska understrykas att samtliga webbplatser klarade sig överlägset bättre på desktop än på mobilen. NRK kan utses som vinnare när det gäller desktop medan BBC verkar betydligt bättre än de andra två webbplatserna på mobila enheter. Allt som allt kan man säga att BBC har något högre PSI-betyg än NRK, medan DR är sämst i klassen.

I vissa fall varierar PSI:s betyg extremt mycket: jag analyserade en och samma webbplats två gånger inom en minut och fick se att det ena värdet låg på 20 och det andra på 53. Resultaten som presenteras i rapporten ska alltså inte accepteras utan vidare utan ska tas med en nypa salt om de verkar extremt låga (som DR:s resultat på 2 poäng för mobila enheter).

Men oavsett detta visar PSI:s förbättringsförslag klart och tydligt att man ska se till att inte överföra mer data i början än nödvändigt. Detta kan uppnås genom att minifiera och komprimera filer samt att välja rätt filstorlek och filformat för bilderna. Andra viktiga aspekter att beakta är att prioritera rätt vilka filer som ska laddas först, att undvika alltför stora DOM-träd och att tänka på hur cache kan effektiviseras.

Förutom BBC:s radioflik gäller det för samtliga sidor att resurserna strömmar in hela tiden och att sidan aldrig laddas färdigt. I [bilagan](https://docs.google.com/spreadsheets/d/1tXWC8Cfl3cJemy4D-QO_k8orKxADwSxS0VZjqy8yKPE/edit#gid=0) markerade jag detta genom att skriva "över 10 minuter". Detta väcker också vissa frågetecken.

Personligen anser jag att sidor som tar mer än en eller två sekunder att börja rita upp innehållet upplevs som sega och om man ska vänta mer än tre-fyra sekunder på att få se bilderna känns det som störande. Dessa krav uppfylls av alla tre webbplatser som jag har analyserat. Jag är dock medveten om att många andra människor har lägre gränsvärden än jag.

Jag tycker att vissa åtgärder som kan bidra till att minska laddningstiden gör att man som programmerare skjuter sig i foten i längden. Detta gäller rådet om att använda sig av inline CSS och JavaScript och att inte använda sig av third-party code. Det finns ju en anledning till att man har valt att ta med exempelvis Google Analytics på sin webbplats. Det är inte heller alltid möjligt att undvika alltför stora DOM-träd: meningen med webbplatserna som har analyserats i rapporten är ju att de ska presentera så mycket information som möjligt. Man kan inte både äta kakan och ha den kvar.

Referenser
-----------------------

Förutom verktygen som nämns i Metod ovan användes inga externa källor.

Övrigt
-----------------------

Rapporten har skrivits av mig, Aron Tési (arts19).
