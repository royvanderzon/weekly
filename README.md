- [url](#article_1)
[Take me there](#article_1)

# Weekly

## 02-07 Steven -> Catawiki
Steven Hay vertelde over het bedrijf Catawiki. Steven had meerdere bedrijven, hield van Lo Fi sketching, graphic design, design en usability.
Hij is een enorme voorstander van de web richtlijnen die het makkelijker maken voor blinden en andere webgebruikers die met omwegen het web bezoeken.
Ook is hij tegen het gebruik van dark patterns. Hij liet interessante voorbeelden zien hierover.

## 02-14 Justus -> Docent HvA (gemist)

## 02-28 -> Peter Paul Koch
Peter Paul Koch is een interessante man die echt terug naar de basis van het web is gegaan. Alles moet werken op alle apparaten waar dan ook. Zo is hij dagelijks bezig met het testen van websites. Ook doet Peter een aantal bijzondere uitspraken (waar ik het grotendeels eens mee ben) waardoor veel ophef is ontstaan.
1 – Websites worden te veel als native apps gemaakt
2 – Te veel features
3 – Teveel libs/tools/frameworks
4 - De website is geen platform

## 03-14 Titus Wormer -> Docent HvA (over github)
Het is belangrijk dat je altijd de eigenaar van gekopieerd werk crediteert (als je de code mag gebruiken). Ook heeft Titus een stukje geschiedenis laten zien van open source en over de bedenker van GitHub.
Aan het eind van de Weekly Nerd heeft Titus een mini stukje live demo gegeven omdat er niet veel tijd meer over was.
“Free, not as in free beer”

## 03-28 Jasper (Voorhoede)
Optimalisatie van websites. Laten zien hoeveel winst je kan maken met het optimaliseren van websites. Maar ook hoeveel meer conversie je kan halen. Dit is altijd een bijzonder goed werkend verkooppraatje voor nieuwe klanten.

Ook vertelde Jasper over een nieuwe beweging waarin je makkelijker PwA’s kan maken. Dit doordat veel native functionaliteit van mobiele devices beschikbaar wordt gemaakt in de verschillende browsers.

## 04-14 Bram -> Accessibility
Bram is blind en nam daarom zijn hond mee naar de Weekly Nerd. Hij is in het eerste gedeelte van de Weekly Nerd door een aantal websites heen gegaan om te laten zien hoe dit nou precies in zijn werk ging. Ook kon hij er wel gevatte opmerkingen over maken. De HvA website zit bijvoorbeeld goed in elkaar maar toch zijn er een hoop dingen onduidelijk voor bijvoorbeeld slechtzienden.
De kern van het verhaal is dat je altijd moet zorgen dat iedere website altijd goed te gebruiken is voor mensen die het web op een andere manier bezoeken.

## 04-14 Peter Peerdeman -> Lifely
Peter kende we al van Lifely. Hij liet startdashboard.nl zien, het is een applicatie in Meteor. Deze applicatie bevat een intranet met realtime features. Het wordt vanuit een eigen server gedraaid wat zorgt voor privacy. Het is niet ge-connect met facebook of Whatsapp.
-	Distributed data protocol
-	Connection
-	Managing data
-	Remote Procedure Calls
-	Error

## 04-28 Niels -> IoT specialist
Niels is de oprichter van HTML5test.com en heeft ook meerdere projecten gestart zoals Solonhub. Niels is afkomstig uit Groningen! Niels heeft de techniek bedacht “klik aan klik uit”. Het is een simpele manier om IoT te developen door middel van een draggable interface. Ook maakt hij gebruik van Z-wave. Dat zorgt ervoor om een mash netwerk te creëren. (Wifi hotspot aanzicht)

## 05-16 Nick de Bruijn -> CEO Lifely
Nick is de CEO van Lifely. Hij is op zijn 12e begonnen met ondernemen. Hij begon met het verkopen van Pokemon kaarten online over de hele wereld! Nick vertelde dat de mainfocus van het bedrijf gaat naar de backend van het bedrijf. Hij is op dit moment bezig met veel verschillende projecten. Een ervan is die over de integratie van vluchtelingen in Nederland.
-	Wees uniek
-	Leer van je fouten
-	Doe maar een ding tegelijk
-	Je moet je producten kunnen verkopen

## 05-23 Guido Bouman -> Q42
Guido is een interaction engineer bij Q42. Q42 heeft vestigingen in Nederland en Amerika. Ze maken websites, webapplicaties, native apps en IoT. Dit doen ze in verschillende programmeertalen. Hij heeft verteld over hoe ze zijn koffie zet apparaat hebben aangeloten op het netwerk. Dit hebben ze doormiddel van een Raspberry pie! Ze konden uiteindelijk uitlezen wat de zero state was en wat er veranderd was. Zo konden ze zien wat voor verschillende koffie er gedronken wordt. Dit laten ze realtime zien op de website.

## 05-31 Leonie Watson -> Accessibility developer (blind)
Leonie wilde een aantal dingen vertellen over screen readers:
-Voor wie screen readers zijn! (Bijvoorbeeld ook voor slecht ziende)
-Wanneer screenreaders gebruikt worden
-Waar ze gebruikt worden
-Waarom je er moet voor ontwikkelen

# Artikelen

## Hoe zet je een schaalbare proctieomgeving op voor NodeJS en MYSQL?
[create an anchor](#article_1)

Hoe zet je een productie omgeving op die je echt kan gebruiken om je applicatie bezoekbaar te maken voor gebruikers? In dit artikel lees je over hoe je dit het beste kan opzetten. We gaan het voornamelijk hebben over NodeJS, Mysql, Nginx, security, OpenVPN, Ubuntu en Esxi.

Om te beginnen heb je een aantal ingrediënten nodig:
- VPS met VPN of een hobby server
- Esxi
- Ubuntu
- NodeJS & NPM
- Mysql server
- Nginx
- OpenVPN op je computer

Wat zijn al deze dingen?

VPS & VPN (Virtual private server & virtual private network) of hobby server
Dit is gewoon een computer waarop jou applicatie en database draaien. Het is belangrijk dat dit wel echt een server is omdat de hardware is gemaakt om langdurig mee te gaan en ook kan het langer aan blijven.

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

Maak 4 virtuele Ubuntu containers aan. Het is aan te raden om de NodeJS 2GB ram te geven. De andere drie virtuele servers kunnen 1GB. Geef de NodeJS en minimaal 10 gigabite opslag en de Mysql minimaal 5GB. Download Ubuntu hier: http://releases.ubuntu.com/14.04/ 

Installeer op de volgende 4 dingen op de op de verschillende virtuele servers:
MYSQL Server -> https://dev.mysql.com/downloads/
Dit is je database server. Voor je software installeert voer altijd eerst apt-update uit. Met ifconfig kan je bekijken welk ip adres deze server heeft.

NODEJS & NPM -> https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-an-ubuntu-14-04-server
Het is aan te raden om eerst NVM te installeren op de server. Dit zodat je altijd kan switchen tussen verschillende node versies. Start je Node server vanuit /var/www. Zodra je hier een test applicatie in draait kan je deze bereiken via het IP adres van de server gevold door de port die je hebt opgegeven in de app.js (bijvoorbeeld 192.168.0.4:3000). Als je verbinding wilt maken met de database server bekijk je op de MYSQL server wat het IP adres is. Vergeet niet dat daar nog een poort achter moet die staat ingesteld op je MYSQL server. Het is aan te raden om je Node applicatie levend te houden met PM2. Hiermee kan je logs terug kijken en van een afstand je server status monitoren. Ook kan je instellen dat je error logs gemaild krijgt als je server een error krijgt. PM2 houd je app aan. Als hij uitvalt start hij opnieuw op. Lees hier hoe je PM2 installeert: https://www.digitalocean.com/community/tutorials/how-to-use-pm2-to-setup-a-node-js-production-environment-on-an-ubuntu-vps

OpenVPN -> https://www.digitalocean.com/community/tutorials/how-to-set-up-an-openvpn-server-on-ubuntu-14-04
Nadat je deze tutorial gevolgd hebt kan je verbinding maken met deze OpenVPN server. Vervolgens kan je vanaf buitenaf inloggen en ssh’en naar de andere virtuale servers en de Esxi zelf.

Nginx -> https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-14-04-lts
Maak in de Nginx een profiel aan voor je nieuwe NodeJS server. Doe dit met behulp van deze tutorial: http://www.nikola-breznjak.com/blog/javascript/nodejs/using-nginx-as-a-reverse-proxy-in-front-of-your-node-js-application/

## Coding in NodeJS
[create an anchor](#article_2)

In NodeJS worden een aantal termen gebruikt die belangrijk zijn om te begrijpen. Dit zijn NPM (Node package manager), NodeJS, app.js, modules, NPM scripts en package.json. Voordat je een Node project kan beginnen is het belangrijk om te begrijpen wat deze termen inhouden.

NPM
NPM is het “systeem” waarmee je losse modules kan inladen. Deze kan je zelf maken of vinden op npmjs.com.

Package.json & .gitigone
Deze modules zet je vervolgens in je “package.json”. Naast de gebruikte module, zet je ook het versie nummer erbij. Al deze modules worden ingeladen in het mapje: “node modules”. Dit mapje zet je in de .gitignore zodat ze niet mee worden geupload naar Github. Zodra jij of iemand anders het project wilt gebruiken kan je het project clonen of kopieren (zonder de “node modules” map) en het commando “npm install” uitvoeren. Ook is het belangrijk dat je aangeeft welke NPM Modules worden gebruikt voor de applicatie, en welke voor de development omgeving. 

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

