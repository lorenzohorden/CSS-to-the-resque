# CSS-to-the-resque
Voor dit project ga ik een interactieve site maken die er visueel mooi uit ziet en dit doe ik met alleen HTML en CSS. Hier leg ik mijn onderzoeken en experimenten vast.

## opdracht
modular control panel: Ik ga form elementen gebruiken om daarmee de stijl van andere elementen in de html aan te passen.


## plan van aanpak

Mijn plan is om verschillende kamers te maken van een huis waar je doorheen kunt klikken en waar je dingen aan en uit kan zetten, bijvoorbeeld een kraan aanzetten als je op de kraan klikt of het licht aan en uit zetten.
Ik wil beginnen met een kamer, ik denk een badkamer, omdat daar niet mega veel dingen in staan weet ik vrij zeker dat ik dat af krijg. Daarna kan ik altijd extra kamers maken.
Ik wil ook in elke kamer een raam en een knop ergens in de hoek om het dag of nacht te maken.

Er zijn een aantal dingen waar ik (meer) over wil leren om dit te kunnen doen:
1. Verdiepen in CSS-nesting en :has()
2. 3D gebruiken en perspective
3. Animation om bijvoorbeeld stromend water uit een kraan te laten lopen of gas uit het fornuis te laten komen


## voorbeelden voor code
3D-kamer:
https://codepen.io/ricardoolivaalonso/pen/mdPzrpe?editors=1100
Dit is hoe ik het perspectief wil, alleen het mag van mij minder realistisch, zie inspiratie voor hoe ik het wil hebben

switch:
https://codepen.io/ricardoolivaalonso/pen/QWJxYXE
Dit is qua stijl een beetje waarvoor ik wil gaan, alleen als ik een hele kamer maak ga ik denk ik voor iets minder detail


## stijlinspiratie
![image](https://github.com/user-attachments/assets/d331ca6e-145e-4852-bc98-03f9f87c3c9b)
Ik vind de stijl van deze game erg mooi en denk dat dit best haalbaar is met HTML en CSS.

![image](https://github.com/user-attachments/assets/bd84c12a-351f-4162-9034-bd3aa4237479)
Ik wil ongeveer zo een perspectief hebben met in de hoek een deur om naar een andere kamer te gaan.

![image](https://github.com/user-attachments/assets/ff7c1faf-faab-41e1-a16c-71101e8b1352)
Deze stijl vind ik mooi, ik wil het alleen niet in pixels, maar zo veel dingen in een kamer om mee te interacteren lijkt me leuk.


## week 2
Deze week ben ik begonnen met het maken van de kamer in 3D, ik heb gekeken naar deze video: https://www.youtube.com/watch?v=niwUUtgn4-o&t=172s

Aan de hand daarvan heb ik drie vlakken gemaakt om een vloer en twee muren te maken en zo gedraaid dat het op een kamer lijkt. Ik heb gespeeld met rotate van transform om de kamer zo te draaien dat je alle muren goed kunt zien.

Vervolgens heb ik chatGPT gevraagd of het mogelijk is in pure css met scroll animations de rotate te veranderen, hiervoor heb ik het main element (de parent) 200vw en 200vh gegeven. Toen ik de code van chatGPT wilde uitproberen op alleen het rotaten van de x-as werkte de y-as ook en toen kwam ik erachter dat het veranderen van perspectief vanzelf gebeurd wanneer je door de parent scrollt. Het probleem is dat het draaien nu de andere kant op is van wat ik wil.

Daarna wilde ik een blok maken, ik begon met de andere drie kanten van de achtergrond, maar Sanne vertelde me dat ik beter een cuboid kon maken, toen heb ik daar research naar gedaan en uiteindelijk heb ik op dat concept mijn eigen variatie gemaakt.

## week 3
Ik was deze week op maandag ziek, dus hier heb ik niet super veel kunnen doen. Op dinsdag heb ik de wasbak geprobeerd om diepte te geven, dat wilde ik eerst doen met een background image met een angle die veranderd zodat het de ilusie geeft dat hij hol is. Ik kwam er al snel achter dat het makkelijker is om voor elke zijde van de wasbak een cuboid te gebruiken.
Nadat ik dat gedaan had heb ik nog een kraan toegevoegd aan de wasbak.

### BONUS weekend
Omdat ik maandag ziek was en bang was dat ik niet genoeg zou hebben voor de deadline ben ik in het weekend nog even aan de gang gegaan aan voorbereiding voor de week erop.

## week 4
Dit is alweer de laatste week van het project, op maandag kwam Sanne met een idee om de kleur van het water in de wasbak aan te passen aan de hand van hoe lang het warme en koude water aan heeft gestaan. Hij heeft hier een voorbeeld voor uitgewerkt [https://codepen.io/shooft/pen/WbNMRZb?editors=0100] en dat was erg handig, alleen het voorbeeld werkt als je één kleur tegelijkertijd wilt aanpassen en ik heb er twee nodig.
