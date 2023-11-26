# Instructable

Todo: uploaden programma hierboven


### stap 1
Bestel alle componenten uit de bill of materials: 
<br />

|volgnummer        |naam                                    |omschrijving                          |nieuw/recup      |kostprijs/stuk      |aantal  |subtotaal    |
|----------        |----                                    |------------                          |-----------      |--------------      |------  |---------    |
|1                 |Microcontroller                         |ATmega32u4 (Arduino Leonardo)         |Recup            |€12,99              |1       |€12,99       |
|2                 |Mini Micro Metal Gear Motor 30:1        |6V DC Gear Motor                      |Nieuw            |€3,56               |2       |€7,12        |
|3                 |H-brug                                  |DRV8833 Dual Motor Driver Carrier     |Nieuw            |€12,52              |1       |€12,52       |
|4                 |Infrared Reflection Sensors (8)         |QTR-8A Reflectance Sensor Array       |Nieuw            |€16,13              |1       |€16,13       |
|5                 |18650 Li-ion Batterijen                 |Rechargeable Battery (3,7V - 19800mAh)|Nieuw            |€2,63               |2       |€5,26        |
|6                 |Batterijhouder                          |18650 Dubbele batterijhouder          |Nieuw            |€2,39               |1       |€2,39        |
|7                 |Batterijoplader                         |LiitoKala Lii-L2 3,7V 18650           |Nieuw            |€10,17              |1       |€10,17       |
|8                 |Bluetooth Module                        |HC-05                                 |Recup            |€11,96              |1       |€11,96       |
|9                 |Wielhouders                             |Micro Metal Gearmotor Bracket Pair    |Nieuw            |€5,39               |1       |€5,39        |
|10                |Wielen                                  |Polulu wheel 40x7mm Pair - Red        |Nieuw            |€7,69               |1       |€7,69        |
|11                |Weerstanden                             |1x1kOhm en 1x2kOhm OF 3x1kOhm         |Recup            |/                   |3       |/            |
|12                |Dupont-draadjes                         |20xman-vrouw en 5xman-man             |Recup            |/                   |25      |/            |

Verder zijn er nog een aantal andere benodigdheden, zoals houten blokjes, een houten plank en extra wielen, maar deze zijn optioneel en kunnen perfect vervangen worden door andere recup-materialen.

### stap 2
Nu we al het materiaal beschikbaar hebben, stellen we de linefollower samen. Als frame van de auto ga je best opzoek naar een houten plankje, of ander recupmateriaal die ongeveer een afmeting hebben van 160x100mm.
Er kan voor gekozen worden om met een figuurzaag extra vorm te geven, zodat dit het frame van een gestroomlijnde wagen kan voorstellen. Dit kan uiteraard ook achteraf gebeuren.
![403679670_808460354413685_5912383544201351500_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/feed7c43-2fa8-4d42-b192-6923e4285710)
Vervolgens monteren we de batterijhouder op ons houten frame. Deze zetten we op de achterkant van onze plank, mooi in het midden. Ernaast worden 2 blokjes (500x250x10mm) geplakt, zodat we later de arduino boven de batterijhouder kunnen plaatsen. Het vastplakken van de houtblokjes en batterijhouder kan gebeuren met behulp van houtlijm.
![405333687_223592240758807_7123575042251916946_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/daa8e4fe-3517-4284-bc2d-5f54fd6ee951)

### stap 3
In deze stap gaan we de motoren monteren op het frame. Hiervoor gebruiken we de "wielhouders" die samen met de motoren werden aangekocht. Bij het monteren van deze houders is het belangrijk dat ze allebei op de zelfde afstand worden gemonteerd, zodat ze mooi in lijn liggen met elkaar en de auto dus niet scheef zal gaan rijden. Via de volgende 2 foto's kan worden afgeleid waar ik deze ongeveer heb gemonteerd:

![405266047_1487613928690795_4685521728919634876_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/30f6ca06-9a14-4b49-a1dd-da7b3a4dbf25)
![404350260_309790145228844_7951685887738030043_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/bc523f6a-a4cd-44c8-aa38-afd30f6adf6a)

Vervolgens werden gaatjes geboord, zodat de bijgeleverde boutjes gemakkelijk in het hout konden worden gedraaid.

![405154670_3388969721320824_5026883236161777480_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/7c65f37e-e2cd-4d87-99d6-0feb242dba33)
![405283208_1006741277289677_2358455657544103621_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/6f2edf54-4b0a-4c79-b65c-759d0153a044)

Als laatste solderen we 2 dupontdraadjes aan de motoren, alvorens we deze vaststeken in de gemonteerde klemmen. Dit zodat we alle ruimte hebben om dit te kunnen doen.

![403688872_365273492548581_5732422698806328131_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/e94c658b-2e3a-458c-8b61-b7e67ce9bd96)

### stap 4
Om de andere componenten, zoals de H-Brug en de bluetooth module te monteren gebruiken we simpelweg een elastiekje zodat alles mooi blijft zitten.

![405139945_312554088254143_3331511207421659937_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/743c7d06-7842-4dc1-b1e1-acb5af38c558)

Vervolgens nemen we het elektronisch schema erbij en gaan we alles aansluiten aan de hand van dupont-draadjes. In het schema is te zien dat er 3 knooppunten zijn. 2 bij de batterijspanning en 1 bij de 5V spanning. Hiervoor gaan we gebruik maken van 3 kroonklemmen:

![403625895_3664321383829692_851847983461746198_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/aa911c33-f785-4f6b-847b-4d8f4b3db0f3) 

Ook de sensor moet nog worden gemonteerd aan de onderzijde van de wagen. Hiervoor werden als eerst de twee sensoren die afzonderlijk kunnen werken van het breakout board gebroken. Zo hebben we nog steeds 6 sensoren, wat alles wat compacter maakt.
![image](https://github.com/jorenverdegem/Linefollower/assets/146443076/ecabba76-e05e-405a-9520-b96922925518)

Hierna meten we af waar de draadjes via de onderkant van ons frame naarboven zullen komen, als de sensor mooi in het midden gemonteerd zit. Op deze plek worden verschillende gaatjes geboord, waar we uiteindelijk een mooie gleuf van maken:

![403804083_266288663098954_5267448171383346415_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/a3c8a458-9a44-4903-86a6-5b314f499ed3) 

![405217240_2342251582633342_3867722100881489745_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/fac74e2f-af9b-49a5-b04f-c9e2c6771c2a)

Als laatste word de sensor nog eens extra vastgezet door 2 kleine boutjes in het frame te vijzen.

![403641477_1091571545612815_5156694672164627113_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/b8e49645-920f-4b37-9211-0aa776ef76b4)

### stap 5
In de voorlaatste stap zetten we de arduino op de twee houten blokjes, die we opnieuw vastmaken met een simpel elastiekje. Vervolgens verbinden we alle componenten, zoals in het elektronisch schema wordt weergegeven:

![image](https://github.com/jorenverdegem/Linefollower/assets/146443076/a4b4eb02-db5e-4f55-979f-d4512fc759f4)

![405132827_636497835104419_2663353506568405863_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/206910ab-60d3-42ab-8102-bc3ff8db17fe)

De 3 kroonklemmen kunnen opnieuw met houtlijm worden vastgeplakt op de voorzijde van het frame. Als extra optie kunnen ook twee extra wielen worden gemonteerd aan de voorzijde. Je kan er ook voor kiezen om de auto te laten slepen.

![403647766_1569203267187191_374478284157019129_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/267d4551-9efe-42b8-8f91-2861b06aaa8f)

Indien de voorgaande stappen correct werden gevolgd, zou het eindresultaat er ongeveer zo moeten uitzien:

![400920108_895944135587999_7262908235151916565_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/e1d3a3cc-2b83-4a0e-b95b-40a63d31a59b)

### stap 6
Nu moeten we enkel nog het juiste programma gaan uploaden in de arduino. De code die moeten worden upgeload kan worden teruggevonden als bestand in deze repository. Als je dit bestand opent met de arduino IDE software kan linksboven op de upload knop worden gedrukt. Nadat het uploaden is geslaagd kunnen de batterijen in de auto worden gestopt, kan verbinding via bluetooth worden gemaakt met de telefoon, en zal de auto werken!
(Voor meer info over de bediening van de auto via bluetooth, zie https://github.com/jorenverdegem/Linefollower/tree/main/gebruiksaanwijzing .
