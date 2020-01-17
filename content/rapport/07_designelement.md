---
---
Tema med designelement (kmom06)
=========================

Detta innehåll är skrivet i markdown och du hittar innehållet i filen `content/rapport/07_designelement.md`.

Temat som beskrivs här kan nås via följande [länk](rapport/designelement?style=kmom06-designelement).

Gradients
-----------------------

I detta kmom började jag att experimentera med hur olika bakgrundsmönster kan skapas med hjälp av CSS. Efter att ha studerat vissa exempel på den [här](https://freefrontend.com/css-background-patterns/) sidan prövade jag mig fram till ett vågrätt sicksacksmönster som nu ingår i footerns bakgrund. Mönstret är framtaget med hjälp av två stycken linear-gradients med en lutning på 25 respektive -25 grader.

Linjer
-----------------------

Förutom linjerna i footerns bakgrund använder jag streck för att markera länkar i brödtexten men inte i listor. Jag har också experimenterat med ```transform: rotate(1deg);``` som gör att sidebarens (och bylinens) innehåll lutar lätt åt vänster på vänster sida och åt höger på höger sida. Jag tycker att denna effekt bidrar till att guida användarens blick i rätt riktning (nämligen till innehållet i mitten). Dessutom är området inner-wrap-main avgränsat med nästintill osynliga vertikala linjer på bägge sidorna.

Typografi
-----------------------

Efter att ha lyssnat på ett [program](https://sverigesradio.se/avsnitt/102597) i SR:s serie om typsnitt blev jag nyfiken på Comic Sans och valde det för brödtexten i temat. Rubrikerna sattes till ett annat sans-serif typsnitt: Impact. Nu har jag läst på lite grann och fått veta att Comic Sans väcker starka känslor hos en hel del människor (mest hos designfolk) och anses vara ett typsnitt som är olämpligt i en rad sammanhang och som ofta missbrukas. Jag tycker däremot inte att det ger ett dåligt intryck på webbplatsen eller att det sticker ut på något negativt sätt.

Texturer, mönster
-----------------------

Headerns och sidebarernas samt bodyelementets svart- respektive vitaktiga bakgrunder utgörs av texturer som är lånade från [den här sidan](https://www.toptal.com/designers/subtlepatterns/). Mönstren är tillräckligt subtila för att inte dra alltför mycket uppmärksamhet till sig själva men samtidigt så ger de en lite annorlunda känsla till webbplatsen. Footerns bakgrundsmönster tog jag fram själv med hjälp av CSS.

Färger, kontrast
-----------------------

Färgschemat som används i temat har vissa likheter med mitt mörka tema i kmom04. Här har dock bodyelementet en vitaktig bakgrund med mörk text. Bakgrundsfärgerna är inte enhetliga färger utan är finkorninga texturer. Vid hovring får länkarna i navbaren och sidebarerna en svart bakgrund. Jag såg också till att html-elementets bakgrund inte syns på de sidorna där innehållet inte tar upp hela sidan genom att sätta footerns box-shadoww till ```box-shadow: 0 50vh 0 50vh #123``` som är samma färg som footern har i övrigt.

Bakgrundsfärgerna och texternas färger har tillräckligt bra kontrast på hela webbplatsen, men samtidigt har jag sett till att inte maximera kontrasten för det kan ha oönskade effekter.

Referenser
-----------------------

Den teoretiska bakgrunden till rapporten är hämtad främst från följande [artikel](https://www.canva.com/learn/design-elements-principles/).

Övrigt
-----------------------

Rapporten har skrivits av mig, Aron Tési (arts19).
