# Instructable

Nadat we Plan B hebben samengesteld, kiezen we ervoor om het resultaat nog mooier afwerken. Het idee is om een printplaat te ontwerpen, die kan dienen als frame voor onze wagen. Hierbij zullen dus geen dupon meer nodig zijn, wat zal zorgen voor een mooier afgewerkt geheel. Op de printplaat zorgen we dus voor alle connecties tussen de verschillende componenten, met bijhorende gaten zodat we onze componenten hierop kunnen solderen.

### stap 1

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
|11                |Pinheaders                              |                                      |Recup            |/                   |40      |/            |

Nu we alle componenten hebben, kunnen we de printplaat beginnen ontwerpen. Dit werd gedaan via de website: https://easyeda.com/editor .
Het ontwerpen van deze printplaat gebeurd in 3 stappen.

### stap 2

Je tekent een elektronisch schema, waarbij je alle componenten terugzoekt in het programma. Het is belangrijk dat je de exacte componenten invoegt, zodat de afmetingen in de latere fases overeenkomen met onze componenten. Het elektrisch schema dat ik heb ontworpen is terug te vinden via de volgende link: https://github.com/jorenverdegem/Linefollower/tree/main/technische%20tekeningen/elektronisch/planA . Hierbij kan de JSON worden gebruikt om rechtsreeks in het programma te voegen, dan hoef je het schema niet meer zelf te tekenen.

## !BELANGRIJK! 
De component "DRV8833" staat verkeerd getekend in dit programma. De gaatjes voor de pinnen zijn te klein, en de component is 5 mm te dik getekend. Je gaat hier dus best opzoek naar de juiste component, of past de tekening aan zodat ze overeen komt met de afmetingen uit de datasheet.
Let er verder ook op dat je de QTR-8A sensor niet perfect in het midden plaatst! Wij maken enkel gebruik van de eerste 6 sensoren (want een arduino heeft maar 6 analoge inputs), waardoor het midden van de sensor zich op een andere positie bevindt. Zorg dat dit overeenkomt!

### stap 3

Nadat je het elektronisch schema hebt gemaakt, en gecontroleerd hebt dat alles correct is aangesloten kan je beginnen aan het mechanisch ontwerp. Hierbij kies je waar welke component staat op de printplaat, en kan je ook de vorm aanpassen. Mijn mechanische tekening is terug te vinden via de volgende link: https://github.com/jorenverdegem/Linefollower/blob/main/technische%20tekeningen/elektronisch/planA/readme.md .

### stap 4

Als laatste ga je op de mechanische tekening de verbindingen tekenen. Je kan dit automatisch laten genereren, maar ik raad aan om handmatig de verbindingen te leggen. Zo controleer je zelf nog eens of alles goed zit aangesloten. Mijn uiteindelijke PCB ontwerp is te vinden via de volgende link: https://github.com/jorenverdegem/Linefollower/tree/main/technische%20tekeningen/elektronisch/planA .

### stap 5

Nu alles is getekend kan je de pcb bestellen en hem laten maken. Dit alles duurt tussen de 1 à 2 weken.

#### Resultaat:

![403398636_370587428807641_8804265821271583842_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/437ea987-e8e1-4fa4-93a5-b4c21e8f9117)

![386886413_1037275554153914_3952061519202620705_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/0688d75c-3f29-4372-9f19-a29cb6ce4ca0)


### stap 6

Als de printplaat is toegekomen kan je starten met het solderen van je componenten.
- Waar de arduino komt, soldeer je pinheaders. Op deze manier kan je de arduino er steeds opklikken en weer afhalen.
- De QTR-8A sensor soldeer je aan de onderkant van de printplaat, zodat de sensoren naar de grond kijken.
- De batterijhouder kan je vastkleven met stevige lijm tegen de printplaat. De 2 draadjes soldeer je vast op de voorziene metalen vierkantjes.
- De bluetoothmodule kan je rechtopstaand solderen. Zorg ervoor dat de pinnen (zoals vcc en gnd) overeenkomen met de juiste gaatjes op de pcb.
- De motoren maak je vast met de bijhorende beugels, de gaatjes zijn hiervoor perfect gepositioneerd.
- De H-brug soldeer je ook vast op de correcte plek

Als alles goed vast zit kan je het geheel opnieuw beginnen testen. Indien er iets misloopt is het interessant om de proof of concepts er weer bij te halen en alles terug afzonderlijk te testen.
Zo was bij mij het geval dat een van de motoren kapot was gegaan. Deze werd zeer warm en draaide niet meer bij zeer lage snelheden. Ook als de reductie ervan tussen werd gehaald deden dezelfde problemen zich voor.

Indien je net zoals mij de fout hebt gemaakt om de component "DRV8833" zonder aanpassen in het pcb programma te gebruiken, kan je de component toch nog solderen aan de hand van vrouwelijke pinheaders, die wat schuin worden geplaatst. Het resultaat oogt iets minder mooi, maar ziet er als volgt uit:

![377144747_2392994354217988_3845947637720984982_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/9ef0b71b-e06e-4fb7-be87-d8fc30622752)


### stap 7

Proficiat! Nu alles werkt heb je een werkend geheel! Nu de wagen tot leven is gekomen kan je gaan spelen met de verschillende parameters, tot je het snelheidsrecord breekt!
Om het geheel helemaal af te werken kan je er eventueel ook een spoiler op monteren. Een getekende spoiler die kan worden afgedrukt met een 3D printer is te vinden via de volgende link:
https://github.com/jorenverdegem/Linefollower/tree/main/technische%20tekeningen/mechanisch 
Deze kan worden gemonteerd aan de onderkant van de pcb, met dezelfde vijsjes als waarmee de motoren zijn gemonteerd.

### eindresultaat:

![398428672_725404612801147_6601868790741897883_n](https://github.com/jorenverdegem/Linefollower/assets/146443076/36fac265-6aeb-4241-9f9e-2fd9b982a569)


