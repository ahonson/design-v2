---
---
Tema enligt designprinciper (kmom06)
=========================

Detta innehåll är skrivet i markdown och du hittar innehållet i filen `content/rapport/08_designprinciper.md`.

Temat som beskrivs här kan nås via följande [länk](rapport/designprinciper?style=kmom06-designprinciper).

Balans
-----------------------

Webbplatsens huvudsakliga innehåll (inklusive navbaren och footern) är centrerat vilket ger en tilltalande känsla av symmetri. Det centrerade innehållet som har en fast bredd på 1100px är på sätt och vis inramat med hjälp av headern och footern som båda är satta till ```width: 100%;```. Detta bidrar ytterligare till att besökaren upplever webbplatsen som balanserad.

Perspektiv
-----------------------

Navbarens menyval har tilldelats en skugga (text-shadow), vilket kan upplevas som att menyvalen är något upphöjda. Sidebarens länkar har däremot försetts med ```box-shadow: 9px 3px;```. I och med att skuggan i x-led är tre gånger så stor som skuggan i y-led guidas användarens blick till själva innehållet som man kommer åt om man klickar på länkarna.

Enhetlighet och harmoni
-----------------------

I och med att bodyelementet har en opacity på 0.9 och att barnelement inte kan ha högre opacitet än sina föräldrar genomsyras hela webbplatsen av bakgrundens mönster och till viss del dess färgval. Den gröna grundtonen passar väl till lövet i övre vänstra hörnet (dbwebbs logotyp) och är ytterligare framhävd med hjälp av den gröna skuggan som navbarens menyval har.

Flashbilden som jag har i mina övriga teman (moln och himmel) passar inte färgmässigt till det aktuella temats färgschema. Därför har jag ersatt den med en annan bild på gröna träd i en skog. Detta har jag gjort genom att sätta flashbildens url till ```content: url("../../htdocs/image/green.jpg?width=1100&height=150&crop-to-fit&area=0,0,30,0");``` via CSS. Om jag hade bytt ut bilden i ramverket skulle jag ha förstört vissa av mina tidigare teman.

Rörelse
-----------------------

Webbplatsen visar upp flera rörliga inslag. När man scrollar neråt på webbplatsen har man en känsla av att bakgrunden förskjuts åt höger. I själva verket rör det sig om två stycken bakgrunder: html-elementets bakgrund står stilla (är fixed), medan bodyelementets bakgrund följer med när man scrollar och har en opacity på 0.9. De båda bakgrundernas diagonaler lutar i motsatt riktning, vilket också ger en känsla av rörelse.

CSS-koden till bakgrunderna är tagna från den [här](https://www.gradientmagic.com/browse) sidan, men jag anpassade proportionerna i dem för att tona ner rörelserna som annars skulle ha varit alltför distraherande.

Variation
-----------------------

Under kmom06 började jag att experimentera med animeringar. Jag satte bakgrundsfärgen till breadcrumb till #111 som sakta men säkert går över till den grönaktiga färgen #474 som sedan skiftar tillbaka till ursprungsläget. Detta repeteras i oändlighet och har attributen ```alternate``` och ```ease-in-out``` för att undvika abrupta förändringar.

Referenser
-----------------------

Den teoretiska bakgrunden till rapporten är hämtad främst från följande [artikel](https://www.canva.com/learn/design-elements-principles/).

Övrigt
-----------------------

Rapporten har skrivits av mig, Aron Tési (arts19).
