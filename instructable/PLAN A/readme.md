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

Nu we alle componenten hebben, kunnen we de printplaat beginnen ontwerpen. Dit werd gedaan via de website: https://easyeda.com/editor .
Het ontwerpen van deze printplaat gebeurd in 3 stappen.

### stap 2

Je tekent een elektronisch schema, waarbij je alle componenten terugzoekt in het programma. Het is belangrijk dat je de exacte componenten invoegt, zodat de afmetingen in de latere fases overeenkomen met onze componenten. Het elektrisch schema dat ik heb ontworpen is terug te vinden via de volgende link: https://github.com/jorenverdegem/Linefollower/tree/main/technische%20tekeningen/elektronisch/planA . Hierbij kan de JSON worden gebruikt om rechtsreeks in het programma te voegen, dan hoef je het schema niet meer zelf te tekenen.

## !BELANGRIJK! 
De component "DRV8833" staat verkeerd getekend in dit programma. De gaatjes voor de pinnen zijn te klein, en de component is 5 mm te dik getekend. Je gaat hier dus best opzoek naar de juiste component, of past de tekening aan zodat ze overeen komt met de afmetingen uit de datasheet.

### stap 3


(wordt vervolgt)
