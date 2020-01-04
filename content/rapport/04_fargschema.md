---
---
Färgval (kmom04)
=========================

Detta innehåll är skrivet i markdown och du hittar innehållet i filen `content/rapport/04_fargschema.md`.

Syftet med denna uppsats är att dokumentera och analysera tre webbplatser utifrån vilka färger de använder och vilken känsla de förmedlar.

Urval
-----------------------

Jag har länge spelat schack på klubbnivå så jag har bestämt mig för att analysera tre schacksajter som presenterar världens främsta spelare. Världsmästaren [Magnus Carlsen](https://magnuscarlsen.com/en/), världsfemman [Ian Nepomniachtchi](http://nepochess.com/en/home-en/) och världssjuan [Maxime Vachier-Lagrave](http://www.mvlchess.com/en/) är alla födda år 1990. Jag har alltså valt att jämföra webbplatser som presenterar och marknadsför schackelitens aktuella stjärnor: jämnåriga unga män med i stort sett samma bakgrund och intresse.

Metod
-----------------------

Jag har strävat efter att dokumentera webbplatsernas färgschema (primära färger, stöd- och accentfärger) och till viss mån deras typografi. Jag använde mig av Eye Dropper (en extension till Google Chrome) för att komma åt färgkoderna och DevTools (F12) för att identifiera typsnitt, fontstorlek mm. Först beskrivs de tre webbplatserna var för sig (se Resultat nedan) och sedan jämförs de med varandra (Analys).

Resultat
-----------------------

### Magnus Carlsens [webbplats](https://magnuscarlsen.com/en/)

![Magnus Carlsen](image/rapport/04_fargschema/magnus.png)

Webbplatsen präglas av ett akromatiskt färgschema i och med att bakgrunden är satt till svart och olika varianter av mörkgrå samtidigt som texten är mestadels vit. Regionen under den första navbaren har en gradient som bakgrund som går från #444 till #222.

Sparsamma inslag av en ljusgråaktig accentfärg livar upp det akromatiska färgschemats monotoni. Accentfärgen används endast inom navigationen som består av två navbarer. Den översta har grön text mot en svartaktig bakgrund som växlar till svart text och vit bakgrund när man hovrar över LI-elementen. Accentfärgen återfinns även som den aktiva länkens bakgrund samt i den nedersta navbarens text när användaren hovrar.

Om man bortser från bilderna är webbplatsens färgval alltså begränsat till följande färger:

<table style="border-spacing: 4px; border-collapse: separate;">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #000">
        <td style="height: 50px; width: 50px; background-color: #111">
        <td style="height: 50px; width: 50px; background-color: #222">
        <td style="height: 50px; width: 50px; background-color: #444">
        <td style="height: 50px; width: 50px; background-color: #4d4d4d">
        <td style="height: 50px; width: 50px; background-color: #32d1a7">
        <td style="height: 50px; width: 50px; background-color: #00d9a3">
        <td style="height: 50px; width: 50px; background-color: #fff">
    </tr>
</table>

När det gäller typografi är typsnittet satt till `font-family: "Cera pro bold", sans-serif;` på rubriker och rubrikliknande paragrafer (såsom Carlsens namn till vänster om välkomstbilden). På resten av sidan används "Cera pro".

### Ian Nepomniachtchis [webbplats](http://nepochess.com/en/home-en/)

![Ian Nepomniachtchi](image/rapport/04_fargschema/ian.png)

Webbplatsen präglas av ett akromatiskt färgschema utan accentfärger så färganvändandet är mycket sparsamt. Navbaren har vit text mot en mörk bakgrund (#1f1d1d) som är något ljusare (#666) för den aktiva länken. Webbplatsen har en helt vit bakgrundsfärg medan nyhetsinslagens bakgrund är satt till #fafafa (dock mörkgråaktig vid hovring). Om man scrollar ner till footern ser man en mörk bakgrund (#272727) med grå text (#9b9b9b), en alldeles låg kontrast tyckte jag. Enligt [Contrast Checker](https://webaim.org/resources/contrastchecker/) har dessa två färger en constrast ratio på 5.37 vilket räcker för normal och stor fontstorlek, men inte för den pyttelilla texten i footern.

Det framgår från DevTools att body-elementet har nästan identisk color (#222) och background (#2a2a2a), vilket verkar konstigt. Dessa färger syns dock aldrig. Källkoden har en för mig ovanlig struktur och ovanliga lösningar på vissa håll.

Om man bortser från flaggorna i navbaren och från bilderna (som byts ju ut med jämna mellanrum) finns endast följande färger med:

<table style="border-spacing: 4px; border-collapse: separate;">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #1f1d1d">
        <td style="height: 50px; width: 50px; background-color: #272727">
        <td style="height: 50px; width: 50px; background-color: #666">
        <td style="height: 50px; width: 50px; background-color: #9b9b9b">
        <td style="height: 50px; width: 50px; background-color: #fff">
    </tr>
</table>

När det gäller typografi är typsnittet satt till Oswald på navbaren, men även Nepomniachtchis namn är markerat med detta typsnitt på välkomstbilden. På resten av sidan är font-family satt till Lato (med "Open Sans" och sans-serif som fallback).

### Maxime Vachier-Lagraves [webbplats](http://www.mvlchess.com/en/)

![Maxime Vachier-Lagrave](image/rapport/04_fargschema/maxime.png)

Om man scrollar ner från välkomstbilden ovan till kontaktformuläret ser det ut så här.

![Maxime Vachier-Lagrave](image/rapport/04_fargschema/maxime_2.png)

Färgschemat som präglar Maximes webbplats är närmast monokromatiskt med orangeaktiga accentfärger. De orange accentfärgerna (en mörk och en ljusare variant) återfinns i kontaktformulärets H2-element och i epostadressen. Dessutom blir navbarens LI-element också orange när man hovrar över dem. Det bör tilläggas att kontrasten mellan accentfärgen och bakgrundsfärgen har ett värde på endast 2.72 och är följaktligen alldeles får låg.

Det finns inget vitt (och inget svart heller) på sidan, utan texterna (både i navbaren och i kontaktformuläret) har färgen #e3ddce. Varannan länk i navbaren leder till regioner med #e3dcce och varannan med #221810 bakgrund, medan själva navbaren sticker ut med den mörka färgen #120f0c.

Om man bortser från flaggorna i navbaren och från välkomstbilden finns endast följande färger med:

<table style="border-spacing: 4px; border-collapse: separate;">
    <tr>
        <td style="height: 50px; width: 50px; background-color: #120f0c">
        <td style="height: 50px; width: 50px; background-color: #221810">
        <td style="height: 50px; width: 50px; background-color: #222">
        <td style="height: 50px; width: 50px; background-color: #a24100">
        <td style="height: 50px; width: 50px; background-color: #f46900">
        <td style="height: 50px; width: 50px; background-color: #e3ddce">
    </tr>
</table>

När det gäller typografi är typsnittet satt till `font-family: "Libre Franklin", Helvetica, Arial, sans-serif;` på BODY-elementet och till  `font-family: Abel, Helvetica, Arial, sans-serif;` på paragrafer och rubriker.

Analys
-----------------------

I enighet med den vedertagna uppfattningen att sans-serif är trevligare att läsa på skärm finns inga som helst spår av seriftypsnitt på de tre webbplatserna.
Magnus Carlsens webbplats är den enda i urvalet som försöker att sticka ut genom att använda ett relativt okänt typsnitt som kostar [$55](https://www.myfonts.com/fonts/typemates/cera/), medan de andra två nöjer sig med gratis typsnitt från Google Fonts.

När det gäller färgval kan man konstatera att de tre webbplatserna skiljer sig markant från varandra utseendemässigt. Detta framgår tydligt av följande tabell som sammanfattar de viktigaste strukturella skillnaderna. I fortsättningen hänvisar jag till respektive webbplats med förkortningarna i tabellens översta rad.

|                | Carlsen (MCA)  | Nepomniachtchi (IAN) | Vachier-Lagrave (MVL) |
| :------------- | :------------- | :-------------       | :-------------        |
| **Färgschema** | Akromatiskt    | Akromatiskt          | Monokromatiskt        |
| **Accentfärg** | Kall (grön)    | Ingen                | Varm (orange)         |
| **Ton**        | Mörk           | Ljus                 | Blandad               |

Alla tre webbplatser ser till att undvika alltför stora kontraster. De använder aldrig #000 mot #fff eller tvärtom utan en aning ljusare respektive mörkare toner.
När det gäller att avgöra om urvalets webbplatser präglas av ett ändamålsenligt färgval och typografi kan man utgå ifrån att världens främsta schackspelare gärna vill förmedla kompetens, självsäkerhet, styrka, stabilitet och elegans. MCA:s mörka ton som är kombinerad med ett unikt typsnitt kan alltså anses vara passande.

Även om den svarta färgen ofta sägs signalera egenskaperna ovan ska det inte glömmas att styrka lika gärna kan uttryckas med vitt inom schackvärldens färgsymbolik. Statistiskt sett har spelaren med de vita pjäserna en upp till 10 % större [chans](https://en.wikipedia.org/wiki/First-move_advantage_in_chess#Winning_percentages) att vinna än motståndaren. Med hänsyn till detta kan även IAN:s luftiga, ljusa stil anses vara ändamålsenlig.

Accentfärgen kan till och med syfta på ens spelstil. Världsmästaren Magnus Carlsen beskrivs ibland som en känslokall positionell spelare, så det är kanske ingen slump att MCA har en kall accentfärg. Å andra sidan använder MVL en varm accentfärg vilket inte är någon tillfällighet: Maxime Vachier-Lagrave har en aggressiv, attackerande stil med vass taktik och känslosamma kombinationer.

Slutligen vill jag framhålla att MCA verkar klart överlägsen i urvalsgruppen både med tanke på typografi och färgval. Både MVL och IAN har undermålig kontrast på vissa ställen och har en fontstorlek som är i mitt tycke svårläst ibland. MCA förmedlar en mera dynamisk känsla. Jag anser att grundtanken med MVL:s design pekar i rätt riktning: bristerna verkar lätta att åtgärda. Däremot kräver IAN en omfattande omarbetning om den ska matcha MCA:s nivå.

Referenser
-----------------------

Den teoretiska bakgrunden som rapporten bygger på är hämtad ur [kapitel 2](https://learning.oreilly.com/library/view/the-principles-of/9780980576894/ch02.html) i kursboken *The Principles of Beautiful Web Design*. Under arbetets gång använde jag mig också av färghjulet på [Color Scheme Designer](https://colorschemedesigner.com/csd-3.5/).

Övrigt
-----------------------

Rapporten har skrivits av mig, Aron Tési (arts19).
