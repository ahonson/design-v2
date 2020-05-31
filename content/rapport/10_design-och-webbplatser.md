---
---
Design och webbplatser (kmom10)
=========================

Detta innehåll är skrivet i markdown och du hittar innehållet i filen `content/rapport/10_design-och-webbplatser.md`.

Syftet med denna uppsats är att kartlägga vilka designprinciper som tillämpas på webbplatser som presenterar världens främsta operasångare.

Urval
-----------------------

De mest berömda operasångarna i modern tid är förmodligen de tre män som blev kända på 1990-talet som de tre tenorerna. Artisterna Plácido Domingo, José Carreras och Luciano Pavarotti har sina rötter i Sydeuropa, kommer från samma kulturkrets och är i stort sett lika gamla. Det kan vara intressant att se vilka likheter deras webbplatser uppvisar.

Metod
-----------------------

Webbplatserna som ingår i urvalet undersöktes var för sig utifrån de designprinciper som finns beskrivna i [Visual literacy](https://dbwebb.se/article/vl.pdf).

* Balans och perspektiv
* Harmoni och enhetlighet
* Rörelse och variation

Undersökningarna återfinns under rubriken Resultat varefter följer en jämförelse av de tre webbplatserna (se Analys nedan). I och med att webbplatserna består av flera sidor kan endast en bråkdel presenteras här. I vad som följer nedan läggs tonvikten på det som finns på förstasidan.

Resultat
-----------------------

### Plácido Domingos [webbplats](https://www.placidodomingo.com/)

![Plácido Domingos](image/rapport/10_webbplatsdesign/domingo.png)

#### Balans och perspektiv

Headern som spänner över hela bredden och som har samma vita bokstäver och samma innehåll på webbplatsens samtliga sidor rymmer Domingos namn (sidans logotyp) och hans motto till vänster samt navbarens länkar till höger. I mitten ser man för det mesta Domingos porträtt (varje sida pryds dock med sin egen bakgrundsbild). Fontstorleken på Domingos namn och på mottot är 42 respektive 18 pixlar, medan navbarens länkar 24 pixlar stora. Om man nu tänker på porträttet som på mittpunkten på en gungbräda får man en känsla av balans genom intrycket att orden till vänster och orden till höger väger lika tungt.

Webbplatsens övriga sidor har ingen margin runt innehållet, medan förstasidans har det vilket lånar ett annat perspektiv till välkomstsidan. På första sidan täcker en div med klassen `slideText` över en del (men inte den nedersta delen) av bakgrundsbilden som om den flöt in från vänster. Det är ett annat exempel på hur elementen kan ordnas i förhållande till varandra.

#### Harmoni och enhetlighet

Webbplatsens navbar och rubriker har adobe-caslon-pro som typsnitt medan brödtexten är satt till open sans med webbläsarens inbyggda serif respektive sans-serif som fallback. Förutom typografin bidrar även formvalet till att sidan förmedlar ett enhetligt intryck. Förstasidan präglas av kvadratiska former då blocken under välkomstbilden är inramade med smala, ljusgråa och raka linjer.

En annan aspekt att tänka på är hur färgpaletten används för att göra sidan mera harmonisk och enhetlig. Bakgrundsbildens grönaktiga ton samt den gula accentfärgen återfinns i reklamen för Rolex längst ner på sidan. På så sätt kan man uppnå att reklamen inte sticker ut som ett störande främmande element utan är skickligt införlivad med resten av sidan.

#### Rörelse och variation

Reklamen längst ner till höger föreställer en levande urtavla vars kontinuerliga rörelse utstrålar en sorts elegans och lugn. Det kan också lyftas fram att samtliga bilder på artisten präglas av en sorts asymmetri som signalerar att han ständigt är i rörelse. Till och med webbplatsens motto: "If I rest, I rust." tyder på detta.

Webbplatsens övriga sidor uppvisar mycket mer variation än den harmoniska förstasidan och avviker följaktligen markant från den.

### Luciano Pavarottis [webbplats](https://www.pavarottiofficial.com/)

![Luciano Pavarotti](image/rapport/10_webbplatsdesign/pavarotti.png)

#### Balans och perspektiv

Flashbilden (som finns under headern men har trots detta det missvisande klassnamnet: `header-image`) är en svartvit bild som spänner över hela bredden och framställer Pavarotti under ett framträdande. Artisten syns mitt på bilden. Sidinnehållet som följer under bilden är centrerat på samma sätt. Detta skulle kunna vara en bra början till att uppnå balans men sidan uppvisar också ett antal störande element som låter oss ana att designkonceptet var betydligt mindre genomtänkt än vad fallet var på Domingos webbplats.

Man skulle kunna förvänta sig att bilden längst upp till vänster (en siluett med artistens namn) fungerar som en länk som leder besökaren tillbaka till förstasidan, men den visar sig sakna funktionalitet. Från en designsynpunkt framstår den som ett dominant element utan någon motpart som skulle kunna skapa balans. När det gäller texten och länkarna runt flashbilden har jag inte lyckats med att upptäcka vilken designprincip som styr deras upplägg. De verkar ha placerats lite på måfå.

Skrollar man ner till stycket "More music" ser man tre stycken udda placerade album. De som skapade sidan kunde gärna ha lagt till ytterligare ett album för att göra sidan lite mer symmetrisk eller de kunde ha satt `text-align` till justerat, men det gjorde de inte vilket gör att besökaren får en lite udda känsla av obehag.

#### Harmoni och enhetlighet

När det gäller typografi är sidan enhetlig för den använder ett och samma typsnitt genomgående. Som jag nämnde ovan tycker jag att det är lite olyckligt att brödtexten inte är justerad.

Förutom en röd accentfärg (som återfinns i rubriker och vissa länkar) är sidan mestadels svartvit. Jag finner det störande att samtliga externa länkar till höger ovanpå flashbilden är röda inklusive Facebooks, Apples, Spotifys och Twitters logotyper som man normalt sett borde ha andra färger. Samma röda färg (#ff4226) används som bakgrundsfärg för stycket "More music" där albumen presenteras. Albumens färgpaletter och denna skrikande röda färg passar tyvärr väldigt illa till varandra.

Sidan präglas alltså av en viss grad av enhetlighet, men det olyckliga färgvalet och det illa genomtänkta konceptet när det gäller layout och typografi gör att det inte finns någon nämnvärd harmoni på webbplatsen. Detta gäller samtliga sidor.

#### Rörelse och variation

De flesta bilder som framställer Pavarotti (t o m siluetten) visar hur han vinkar och gestikulerar ofta med en näsduk i ena handen medan han framträder. Man kan också lägga märke till att R:t i artistens namn längst upp tilll vänster har ett lite längre streck som på så sätt sträcker sig delvis under nästa bokstav.

Förutom dessa inslag har sidan ingenting nämnvärt att erbjuda som skulle ha med rörelse och variation att göra. Den har varken runda linjer eller diagonala streck.

### José Carreras [webbplats](https://josepcarreras-tenor.blogspot.com/)

![Jose Carreras](image/rapport/10_webbplatsdesign/carreras.png)

#### Balans och perspektiv

Sidan är upplagd på följande sätt. Längst till vänster finns en sidebar som innehåller länkar till (och information om) bl a Carreras leukemifond. På mindre eneheter försvinner sidebaren och kan accessas via hamburgarmenyn. Det är lite oväntat att hamburgarmenyn döljer en sidebar och inte navbarens menyval.

Om man bortser från sidebaren ser man att välkomstbilden spänner över hela bredden. Längre ner följer innehållet i en tvåkolumnslayout som dock omvandlas till en enda kolumn på enheter vars bredd är mindre än 1250 pixlar. Detta förmedlar en känsla av balans.

När det gäller perspektiv kan det nämnas att artistens namn (som ser ut som en rubrik men är i själva verket en bild) längst upp är försett med `text-shadow` och ser följaktligen ut som om det var upphöjt lite grann.

#### Harmoni och enhetlighet

På webbplatsen används två typsnitt genomgående, båda från Google Fonts: EB Garamond för rubrikerna och Lora för brödtexten. Färgpaletten är ett annat verktyg som bidrar till att sidan kan upplevas som enhetlig. Rött och svart är de enda färgerna som används mot en genomgående vit bakgrund. Det är märkvärdigt att den röda färgen inte används som ren accentfärg utan markerar både (aktiva) länkar och rubriker. Färgvalet är mera lyckat än på Pavarottis sida. Delvis beror detta på att Carreras sida använder en mörkare variant som inte är så intensiv och att färgen används med måtta.

#### Rörelse och variation

På webbplatsen finns inga spår av medvetna designbeslut gällande rörelse och variation. Det finns varken animationer eller övergångar. Inget element förändrar sitt utseende då man hovrar över det. Emellertid går det att hitta ett förmodligen oavsiktligt sicksackmönster då man skrollar förbi förstasidans välkomstbild till den regionen där innehållet presenteras i två kolumner. De äldre blogginläggens bildmaterial råkar ha varierande höjd och formar på så sätt ett sicksackmönster. Detta kan dock försvinna om nya inlägg publiceras med annorlunda proportioner.

Analys
-----------------------

Vårt ursprungliga antagande om att webbplatserna som har ingått i urvalet kan uppvisa vissa likheter har visat sig sakna underlag. De tre tenorernas webbplatser skiljer sig avsevärt från varandra både innehålls- och kvalitetsmässigt. Plácido Domingos webbplats är den enda som håller måttet och som präglas och genomsyras av professionella designbeslut. Pavarottis officiella webbplats känns aningen daterad med olyckligt färgval och typografi. Enligt detta [verktyg](https://www.duplichecker.com/domain-age-checker.php) är det just Pavarottis webbplats som underhålls mest sällan.

Det hade kanske varit mera rättvist att analysera [Pavarottistiftelsens](https://www.lucianopavarottifoundation.com/) webbplats i stället för hans officella sajt för denna andra webbplats spelar i en helt annan liga när det gäller grafiska koncept och design. Det kan dock tilläggas att Pavarotti gick bort år 2007 så webbplatsens brister har ingenting med honom personligen att göra.

Webbplatsen som presenterar José Carreras är ingen webbplats i egentlig mening utan endast en blogg som är skapad med hjälp av verktyget [Blogger](https://www.blogger.com/). Bloggen har inga som helst kopplingar till honom personligen utan underhålls av en ivrig beundrare till honom. Även om bloggar som sådana har sina begränsningar tycker jag att Carreras blogg överträffar Pavarottis webbplats i många hänseenden. Det kan också nämnas att Carreras har en webbplats för sin [leukemifond](https://www.carrerasresearch.org/en/). Han tycker nog att det är mera angeläget att marknadsföra den än sin egen person.

Sammanfattningsvis kan jag säga att undersökningen har lett till andra slutsatser än jag förväntade mig i början av arbetet. Det var intressant att se hur pass olika urvalets tre webbplatser föreföll sig vara. I tidigare rapporter analyserade jag mest webbplatser som är knutna till webbyråer och ungdomar och som alltså har betydligt trendigare lösningar än de som beskrivits ovan i denna rapport.

Referenser
-----------------------

Jag använde mig av [Eye Dropper](https://chrome.google.com/webstore/detail/eye-dropper/hmdcmlfkchdmnmnmheododdhjedfccka?hl=en) för Chrome för att komma åt de hexadecimala färgkoderna. Dessutom identifierade jag typsnitt, fontstorlek mm med hjälp av DevTools (F12).

Under arbetets gång hittade jag vägledning och inspiration i kurslitteraturens läsanvisningar som hör till kmom06.

Övrigt
-----------------------

Rapporten har skrivits av mig, Aron Tési för kmom10 i Designkursen (ht19).

2020-05-27
