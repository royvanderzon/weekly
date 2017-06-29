### Weekly
- [02-07 Steven](#weekly_1)
- [02-14 Justus](#weekly_2)
- [02-28 Peter Paul Koch](#weekly_3)
- [03-14 Titus Wormer](#weekly_4)
- [03-28 Jasper](#weekly_5)
- [04-14 Bram](#weekly_6)
- [04-14 Peter Peerdeman](#weekly_7)
- [04-28 Niels](#weekly_8)
- [05-16 Nick de Bruijn](#weekly_9)
- [05-23 Guido Bouman](#weekly_10)
- [05-31 Leonie Watson](#weekly_11)

### Artikelen
- [Artikel 1](#article_1)
- [Artikel 2](#article_2)
- [Artikel 3](#article_3)
- [Artikel 4](#article_4)
- [Artikel 5](#article_5)

# Weekly

<a name="weekly_1"></a>
## 02-07 Steven -> Catawiki
Steven Hay vertelde over het bedrijf Catawiki. Steven had meerdere bedrijven, hield van Lo Fi sketching, graphic design, design en usability.
Hij is een enorme voorstander van de web richtlijnen die het makkelijker maken voor blinden en andere webgebruikers die met omwegen het web bezoeken.
Ook is hij tegen het gebruik van dark patterns. Hij liet interessante voorbeelden zien hierover.

<a name="weekly_2"></a>
## 02-14 Justus -> Docent HvA (gemist)

<a name="weekly_3"></a>
## 02-28 -> Peter Paul Koch
Peter Paul Koch is een interessante man die echt terug naar de basis van het web is gegaan. Alles moet werken op alle apparaten waar dan ook. Zo is hij dagelijks bezig met het testen van websites. Ook doet Peter een aantal bijzondere uitspraken (waar ik het grotendeels eens mee ben) waardoor veel ophef is ontstaan.
1 – Websites worden te veel als native apps gemaakt
2 – Te veel features
3 – Teveel libs/tools/frameworks
4 - De website is geen platform

<a name="weekly_4"></a>
## 03-14 Titus Wormer -> Docent HvA (over github)
Het is belangrijk dat je altijd de eigenaar van gekopieerd werk crediteert (als je de code mag gebruiken). Ook heeft Titus een stukje geschiedenis laten zien van open source en over de bedenker van GitHub.
Aan het eind van de Weekly Nerd heeft Titus een mini stukje live demo gegeven omdat er niet veel tijd meer over was.
“Free, not as in free beer”

<a name="weekly_5"></a>
## 03-28 Jasper (Voorhoede)
Optimalisatie van websites. Laten zien hoeveel winst je kan maken met het optimaliseren van websites. Maar ook hoeveel meer conversie je kan halen. Dit is altijd een bijzonder goed werkend verkooppraatje voor nieuwe klanten.

Ook vertelde Jasper over een nieuwe beweging waarin je makkelijker PwA’s kan maken. Dit doordat veel native functionaliteit van mobiele devices beschikbaar wordt gemaakt in de verschillende browsers.

<a name="weekly_6"></a>
## 04-14 Bram -> Accessibility
Bram is blind en nam daarom zijn hond mee naar de Weekly Nerd. Hij is in het eerste gedeelte van de Weekly Nerd door een aantal websites heen gegaan om te laten zien hoe dit nou precies in zijn werk ging. Ook kon hij er wel gevatte opmerkingen over maken. De HvA website zit bijvoorbeeld goed in elkaar maar toch zijn er een hoop dingen onduidelijk voor bijvoorbeeld slechtzienden.
De kern van het verhaal is dat je altijd moet zorgen dat iedere website altijd goed te gebruiken is voor mensen die het web op een andere manier bezoeken.

<a name="weekly_7"></a>
## 04-14 Peter Peerdeman -> Lifely
Peter kende we al van Lifely. Hij liet startdashboard.nl zien, het is een applicatie in Meteor. Deze applicatie bevat een intranet met realtime features. Het wordt vanuit een eigen server gedraaid wat zorgt voor privacy. Het is niet ge-connect met facebook of Whatsapp.
-	Distributed data protocol
-	Connection
-	Managing data
-	Remote Procedure Calls
-	Error

<a name="weekly_8"></a>
## 04-28 Niels -> IoT specialist
Niels is de oprichter van HTML5test.com en heeft ook meerdere projecten gestart zoals Solonhub. Niels is afkomstig uit Groningen! Niels heeft de techniek bedacht “klik aan klik uit”. Het is een simpele manier om IoT te developen door middel van een draggable interface. Ook maakt hij gebruik van Z-wave. Dat zorgt ervoor om een mash netwerk te creëren. (Wifi hotspot aanzicht)

<a name="weekly_9"></a>
## 05-16 Nick de Bruijn -> CEO Lifely
Nick is de CEO van Lifely. Hij is op zijn 12e begonnen met ondernemen. Hij begon met het verkopen van Pokemon kaarten online over de hele wereld! Nick vertelde dat de mainfocus van het bedrijf gaat naar de backend van het bedrijf. Hij is op dit moment bezig met veel verschillende projecten. Een ervan is die over de integratie van vluchtelingen in Nederland.
-	Wees uniek
-	Leer van je fouten
-	Doe maar een ding tegelijk
-	Je moet je producten kunnen verkopen

<a name="weekly_10"></a>
## 05-23 Guido Bouman -> Q42
Guido is een interaction engineer bij Q42. Q42 heeft vestigingen in Nederland en Amerika. Ze maken websites, webapplicaties, native apps en IoT. Dit doen ze in verschillende programmeertalen. Hij heeft verteld over hoe ze zijn koffie zet apparaat hebben aangeloten op het netwerk. Dit hebben ze doormiddel van een Raspberry pie! Ze konden uiteindelijk uitlezen wat de zero state was en wat er veranderd was. Zo konden ze zien wat voor verschillende koffie er gedronken wordt. Dit laten ze realtime zien op de website.

<a name="weekly_11"></a>
## 05-31 Leonie Watson -> Accessibility developer (blind)
Leonie wilde een aantal dingen vertellen over screen readers:
-Voor wie screen readers zijn! (Bijvoorbeeld ook voor slecht ziende)
-Wanneer screenreaders gebruikt worden
-Waar ze gebruikt worden
-Waarom je er moet voor ontwikkelen

# Artikelen

<a name="article_1"></a>
## Hoe zet je een schaalbare proctieomgeving op voor NodeJS en MYSQL?

Hoe zet je een productie omgeving op die je echt kan gebruiken om je applicatie bezoek baar te maken voor gebruikers? In dit artikel lees je over hoe je dit het beste kan opzetten. We gaan het voornamelijk hebben over NodeJS, Mysql, Nginx, security, OpenVPN, Ubuntu en Esxi.

Om te beginnen heb je een aantal ingrediënten nodig:
-VPS met VPN of een hobby server
-Esxi
-Ubuntu
-NodeJS & NPM
-Mysql server
-Nginx
-OpenVPN op je computer

Wat zijn al deze dingen?

VPS & VPN (Virtual private server & virtual private network) of hobby server
Dit is gewoon een computer waarop jouw applicatie en database draaien. Het is belangrijk dat dit wel echt een server is omdat de hardware is gemaakt om langdurig mee te gaan en ook kan het langer aan blijven.

Esxi
Dit is het hoofdbesturing systeem wat op de server komt te draaien. Dit systeem kan andere besturingssystemen virtueel draaien. Zo kunnen we straks meerdere Linux bakken naast elkaar draaien.

Ubuntu
Ubuntu is het besturingen systeem wat we virtueel gaan draaien in Esxi. Voor onze eerste opstelling gaan we vier virtuele containers maken met Ubuntu erin.

NodeJS & NPM
NodeJS is de taal en het systeem waarin de Node applicatie gaat leven. NPM is de Node Package Manager waarmee NPM packages geïnstalleerd kunnen worden.

Mysql
Mysql server is de database software. Deze kan je straks bereiken met een programma zoals Mysql Workbench.

Nginx
Dit is de proxy software. De proxy software praat straks met de buitenwereld en met de losse node Servers.

OpenVPN
Hiermee kan je straks verbinden maken. Deze server verschaft jou straks toegang tot alle andere servers als je mobiel wilt werken (buiten het netwerk waarin de server staat).
Laten we beginnen!

Als je een VPS hebt kan je de hosting vragen over de mogelijkheden voor Esxi. Als je een server hebt installeer Esxi met een usb stick. https://pubs.vmware.com/vsphere-51/topic/com.vmware.vsphere.solutions.doc/GUID-0A264828-3933-4F4F-82D7-B5006A90CDBA.html
Zodra je dit gedaan hebt is het belangrijk dat je dit IP adres static maakt. Dit doe je eerst in Esxi, daarna in je router.
Op alle ubuntu servers die je nu of in de toekomst aanmaakt is het ook belangrijk dat je ze static maakt!

Maak 4 virtuele Ubuntu containers aan. Het is aan te raden om de NodeJS 2GB ram te geven. De andere drie virtuele servers kunnen 1GB. Geef de NodeJS en minimaal 10 gigabyte opslag en de Mysql minimaal 5GB. Download Ubuntu hier: http://releases.ubuntu.com/14.04/ 

Installeer op de volgende 4 dingen op de op de verschillende virtuele servers:
MYSQL Server -> https://dev.mysql.com/downloads/
Dit is je database server. Voor je software installeert voer altijd eerst apt-update uit. Met ifconfig kan je bekijken welk ip adres deze server heeft.

NODEJS & NPM -> https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-an-ubuntu-14-04-server
Het is aan te raden om eerst NVM te installeren op de server. Dit zodat je altijd kan switchen tussen verschillende node versies. Start je Node server vanuit /var/www. Zodra je hier een test applicatie in draait kan je deze bereiken via het IP adres van de server gevold door de port die je hebt opgegeven in de app.js (bijvoorbeeld 192.168.0.4:3000). Als je verbinding wilt maken met de database server bekijk je op de MYSQL server wat het IP adres is. Vergeet niet dat daar nog een poort achter moet die staat ingesteld op je MYSQL server. Het is aan te raden om je Node applicatie levend te houden met PM2. Hiermee kan je logs terug kijken en van een afstand je server status monitoren. Ook kan je instellen dat je error logs gemaild krijgt als je server een error krijgt. PM2 houd je app aan. Als hij uitvalt start hij opnieuw op. Lees hier hoe je PM2 installeert: https://www.digitalocean.com/community/tutorials/how-to-use-pm2-to-setup-a-node-js-production-environment-on-an-ubuntu-vps

OpenVPN -> https://www.digitalocean.com/community/tutorials/how-to-set-up-an-openvpn-server-on-ubuntu-14-04
Nadat je deze tutorial gevolgd hebt kan je verbinding maken met deze OpenVPN server. Vervolgens kan je vanaf buitenaf inloggen en ssh’en naar de andere virtuale servers en de Esxi zelf.

Nginx -> https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-14-04-lts
Maak in de Nginx een profiel aan voor je nieuwe NodeJS server. Doe dit met behulp van deze tutorial: http://www.nikola-breznjak.com/blog/javascript/nodejs/using-nginx-as-a-reverse-proxy-in-front-of-your-node-js-application/


<a name="article_2"></a>
## Coding in NodeJS

In NodeJS worden een aantal termen gebruikt die belangrijk zijn om te begrijpen. Dit zijn NPM (Node package manager), NodeJS, app.js, modules, NPM scripts en package.json. Voordat je een Node project kan beginnen is het belangrijk om te begrijpen wat deze termen inhouden.

NPM
NPM is het “systeem” waarmee je losse modules kan inladen. Deze kan je zelf maken of vinden op npmjs.com.

Package.json & .gitigone
Deze modules zet je vervolgens in je “package.json”. Naast de gebruikte module, zet je ook het versie nummer erbij. Al deze modules worden ingeladen in het mapje: “node modules”. Dit mapje zet je in de .gitignore zodat ze niet mee worden geüpload naar Github. Zodra jij of iemand anders het project wilt gebruiken kan je het project clonen of kopiëren (zonder de “node modules” map) en het commando “npm install” uitvoeren. Ook is het belangrijk dat je aangeeft welke NPM Modules worden gebruikt voor de applicatie, en welke voor de development omgeving. 

Modules
Deze modules kunnen echt van alles zijn. Van hele simpele functies (voor bijvoorbeeld een tijdelijke sessie aanmaken en dan verwijderen) tot complexe tijd calculatie functies (moment.js). Dit zijn modules die je gebruikt voor je applicatie. Er zijn ook modules die je kan gebruiken voor je development omgeving. Bijvoorbeeld nodemon, deze module herstart je applicatie na iedere wijziging zodat je niet continu je server opnieuw hoeft op te starten.

NPM scripts
Met NPM scripts kan je meerdere commando’s laten uitvoeren met een soort van shortcuts die je van tevoren opgeeft. De NPM script definieer je in je package.json. Je kan met bijvoorbeeld een NPM script al je scss en javascript (es6) files laten watchen. Zodra je er eentje bewerkt en opslaat kan je ze automatisch laten compilen voor de uiteindelijke distributie.

NodeJS
NodeJS is de programmeertaal waarin je de applicatie maakt. Het hart van je applicatie leeft in app.js of index.js. Deze file kan je zelf noemen zoals je hem wilt. Je moet dit alleen wel aangeven in je package.json. In deze app.js start je de applicatie, verdeel je de routes en laad je alle modules in met de require functie. In de app.js begin je met het requiren van alle modules. Vervolgens schrijf je de code waarmee je een url request afvangt. Vervolgens start je de applicatie en laat je hem naar een port luisteren. Meestal doen mensen dit op poort 3000. Dit kan je veranderen naar alle anderen poorten die je wilt (zolang ze beschikbaar en vrij zijn). Wat een fijne combinatie is in Node is Express met Ejs (embedded javascript). Hiermee kan je twee belangrijke dingen doen. Je html pagina’s serveren aan de client, middleware toevoegen en makkelijk routes maken voor de url structuur van je applicatie.

Middleware
Hiermee kan je voordat een functie die een url opvangt andere functies laten uitvoeren. Stel dat je een middleware functie schrijft die bekijkt of een gebruiker is ingelogd, als de gebruiker is ingelogd mag de gebruiker verder gaan. Als de gebruiker niet is ingelogd verwijs je de gebruiker door naar een login pagina met de melding dat je ingelogd moet zijn om de pagina te bekijken. Als je deze middleware functie voor iedere pagina zet waar je voor ingelogd moet zijn scheelt je dat een hoop onderhoud en het is ook DRY (don’t repeat yourself).

EJS
Embedded javascript is een view engine waarin je de HTML structuur maakt die naar de eindgebruiker gaat. Een alternatief hiervoor is bijvoorbeeld JADE of Handlebars. In de .ejs files kan je html, javascript, css en ejs typen. De ejs view engine maakt hier uiteindelijk html van en geeft dat door aan de client die de pagina opvraagt.

<a name="article_3"></a>
## Waaraan te denken bij een CMS?

Een CMS. Iedereen heeft het erover. Maar wat is het eigenlijk? Een CMS is niet een soort magische oplossing om content te presenteren aan de gebruiker. Er zijn veel standaard content managementsystemen, maar eigenlijk is een CMS geen standaardoplossing omdat ieder bedrijf andere KPI’s en content heeft.

Een CMS werkt pas echt efficiënt als het op maat is gemaakt of zodanig is aangepast dat het maatwerk is. Dit is vaak te doen met plugins (denk aan alle talloze Wordpress plugins) of door een programmeur in te huren. Optie 1 is het snelst maar zeker niet het best. In de oplossingen, opensource of niet, komen altijd talloze extra functionaliteiten die niet gebruikt worden, dingen moeilijker en slomer maken en niet veilig zijn. Als je een CMS schrijft is het belangrijk om stil te staan bij de basis van het gebruik.

Voordat je aan een CMS begint is het altijd belangrijk om na te denken over de schillende doelen die de gebruikers hebben. Zo heb je minimaal admins, ingelogde gebruikers en gasten. Al deze gebruikers moeten andere functionaliteiten krijgen. Denk maar eens aan een menu. Ook is het belangrijk om uit te schrijven wat voor data je nodig hebt. Dan praat ik niet over wat objectjes maar over het ERD-schema. Hoe beter dit in elkaar steekt, hoe meer profijt je er later van hebt. Denk aan hoe makkelijk het is om later dingen toe te voegen en de relaties. Het is later vaak bijna onmogelijk om benamingen te veranderen of te verwijderen.

Wat ook vaak vergeten wordt is het feit dat niet alle user alle functionaliteiten mogen gebruiken. Als een gebruiker geen formulier heeft om een pagina aan te maken, betekend dit niet dat hij geen post request kan nabootsen waarmee hij een pagina aanmaakt. Het is niet alleen belangrijk dat permissies worden gecheckt aan de render kant, maar nog veel belangrijk aan de kant waar de functionaliteit wordt uitgevoerd. Er bestaan tools waarmee alle responses van een website mee uitgelezen kunnen worden. Als een kwaadwillige dit bemachtigt kan hij door url’s browsen en veel schade aanrichten.

Als je een CMS maakt is het handig om te beginnen met de CMS kant. Op basis van de content die erin wordt gestopt kan je nadenken over hoe de front-view opgebouwd moet worden. In de CMS kan je ook beter gelijk rekening houden met de permissies (wie mag wat zien, bewerken, aanmaken, editen), loginsysteem en het user management. In de praktijk blijkt vaak dat het moeilijk is om dit later in te bouwen. Daarnaast is de kans op fouten groter als dit er later omheen gebouwd wordt. Security fist!

Blijf consistent en houd een documentatie zodat andere mensen het ook kunnen onderhouden. Kijk ook naar andere CMS structuren. Hierdoor wordt het makkelijker om te begrijpen wat je hebt gemaakt voor anderen. “Don't pave the cowpath”.

Als laatste is het goed om je volledig op de gebruiker van het CMS te richten. Bekijk of je zoveel mogelijk wizards kan opdelen in kleine stukken of kan afvangen met logische flows. Houd de terminologie ook simpel en consistent. Let ook op de toegankelijkheid van het CMS. Is het toegankelijk voor slechtziende of bijvoorbeeld via mobiel?

<a name="article_4"></a>
## Accessibility

Hoe maak je iets toegankelijk voor het web? Er zijn talloze voorbeelden van hoe het niet moet. Het is in ieder geval belangrijk om een goede html structuur te hebben. Zorg dat je valide html schrijft en gebruik maakt van de juiste html elementen. Voor toegankelijkheid het vooral belangrijk dat je html semantisch goed is opgebouwd. Het is dan ook handig om je html altijd even door een html validatie systeem heen te halen. Die van het W3C is goed aan te bevelen. https://validator.w3.org/

Geef consistente benamingen aan afbeeldingen en links. Blinden kunnen niet zien wat een afbeelding is of in wat voor context een link is geplaatst. Daarom is het belangrijk dat deze elementen goede beschrijvingen hebben. En bij een link waar ze heen verwijzen. Dit doe je met de “alt” tag. Mocht je een cms gebruiken waar je niet alles in vult, is het nog belangrijker om hier rekening mee te houden. Zo zou een alt tag bij een image verplicht moeten zijn zodat jou content creators hier geen fouten in kunnen maken. Dan dwingt het systeem af dat de uiteindelijke front-view de juiste informatie voor screenreaders bevat.

Zorg voor slechtziende dat het contrast goed is. Dit is niet alleen voor slechtziende, wat als iemand bijvoorbeeld op een telefoon kijkt in de zon? Dan is het belangrijk dat het contrast goed is. Er zijn programma’s waarmee je kan uittesten of het contrast ook echt daadwerkelijk goed is. Toch kunnen deze het ook mis hebben! Test het altijd zelf even door met je telefoon of laptop in de zon te gaan staan, of knijp je ogen dicht en kijk of je contrast ziet.

Zorg dat knoppen goed groot zijn en goede states hebben. Vooral op mobiel is dit erg belangrijk. Ook is het goed om na te denken over waar knoppen komen op wat voor device. Als je bijvoorbeeld een touch table hebt waarbij de gebruiker aan de onderkant van het scherm staat, zou het vervelend zijn als de navigatieknoppen helemaal bovenaan de pagina staan. De states van de knoppen zijn ook erg belangrijk. Dit in combinatie met de affordance uiteraard. Is het klikbaar? Wat gaat er gebeuren als ik erop klik? Of geeft het systeem of website al een feedback over welke kant de pagina op gaat bewegen? Wat nog belangrijker is, is de focus state. Mensen die alleen met het toetenbord navigeren kunnen welke knop ze gaan gebruiken.

Zorg voor progressive enhancement. Javascript is erg krachtig, maar dat brengt ook zijn valkuilen mee. Als de verbinding slecht is, het device verouderd is, het device geen javascript kan uitvoeren of als javascript uit staat kan het zijn dat javascript niet goed functioneert. In dit geval is het belangrijk dat de fallbacks goed zijn. Als je met javascript een div klik baar maakt kan de gebruiker niks op het moment dat javascript niet goed werkt!

Zorg dat je webpagina’s en ontwerpen toegankelijker worden voor het hele web door de hierboven genoemde onderdelen minimaal toe te passen in al je websites en apps!

<a name="article_5"></a>
## Ethische data verzameling

Big data. Wat is dat? Kunnen we het meten? Hoeveel is het en hoeveel hebben we? Misschien een belangrijkere vraag, wie beheert het en wat kan hij ermee?

De belastingdienst hield rond in 2013 een vrouw aan op verdenking van belastingfraude, zei kreeg een uitkering maar kocht te veel excellent biefstuk met haar Albert Heijn bonus pas. Haar uitkering is uiteindelijk stop gezet. (Panopticon privacy - Peter Vlemmix 29:05)

Het is rechtvaardig dat de uitkering van deze vrouw is stopgezet. Maar was het niveau waarop deze vrouw onderzocht is de moeite waard? De oneindige datastroom die wij creëren door te leven wordt opgeslagen en kan op ieder gewenst moment worden gebruikt voor alle denkbare scenario’s.

Het klinkt alsof dit onderwerp ver verwijderd ligt van het onderwerp websites. Toch ligt het dichterbij dan je denkt. Websites zijn zoveel meer dan alleen een informatiebron. Met de talloze inlogsystemen, profielen, reclames, javascripts en databases wordt de mensheid gemonitord! Maar wat is ethisch om op te slaan of om verbanden mee te trekken? Door het gebruik van persuasive design zijn wij in staat gebruikers opdrachten te laten uitvoeren en te sturen in gedrag. Daarmee komt ook een grote verantwoordelijkheid. Designers en programmeurs zouden zo moeten programmeren en designen dat de veiligheid en privacy van de eindgebruikers gewaarborgd ligt.

Als je het hebt over performance, progressive enhancement, toegankelijkheid, tooling, etc. dan heb je het over websites en web apps. Maar waarom vergeten wij privacy altijd? Privacy en etnisch design zou op plek een moeten staan in deze lijst.

Met de komst van IoT wordt dit straks complexer. Onlinedata leeft straks niet alleen maar in onze computers, telefoons en smartwatches... Onlinedata leeft straks in onze koelkast, onze wekker, onze stofzuiger, onze auto en noem het maar op! Tegengaan kunnen we niet, en we moeten het ook zeker niet tegenhouden. Het is belangrijk dat wij ons er bewust van worden en veiligheden in bouwen om integriteit te waarborgen.

Hoe ver moeten wij gaan?

Ver. Als wij iets ethisch onverantwoord zouden moeten bouwen zouden we stop moeten zeggen en advies geven hoe het wel moet. Neem bijvoorbeeld een restaurant die graag hogere ratings wilt hebben en in het formulier standaard alle keuzes al invult op vier van de vijf sterren. Dan zouden wij stop moeten zeggen en uitleggen dat dit moet gaan over de kwaliteit van het eten en de service. Een voorbeeld over privacy: Als je op Bol.com een product bekijkt en vervolgens de website sluit, krijg je een paar dagen later een mail of je nog steeds geïnteresseerd bent in de bezochte producten. Dit onder het mom van: “Misschien ben je er nog wel in geïnteresseerd?” Het lijkt niet erg, maar waar trekken we de grens met hoever wij de gebruiker moeten volgens en data moeten verzamen om vervolgens verbanden mee te trekken?
