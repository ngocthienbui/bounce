# Bounce
Dit is een uitbreiding door Amer en Thien van de originele versie  js-library "Bounce" die door Luuk Derkx is gemaakt.
## Korte inhoud

Een kleine library die de gekozen element kan laten bouncen (springen). 

## Oorspronkelijke code

Het originele code wordt gebruikt in een Index.html file. Hier ziet u basisopzet met twee div elementen en een stukje code waarin je parameters kan aanroepen. 
```javascript
<!-- Een voorbeeld waarin twee bounce elementen worden gemaakt -->
<div id='bounceContainer'>
    <div class='bounce1'>
        bounce element 1
    </div>
    <div class='bounce2'>
        bounce element 2
    </div>
</div>

<script>
    //hierin worden de elementen gekoppeld aan de javascript functies
    var bounce1 = new Bounce();
    bounce1.init('bounce1');
    
    var bounce2 = new Bounde();
    bounce2.init('bounce2');
</script>
```


## Oorspronkelijke demo
See bounce [demo](http://i874261.iris.fhict.nl/s4/bounce/demo)

## Oorspronkelijke functies

In deze library waren de volgende functies beschikbaar waarmee je als gebruiker kan de div elementen aanpassen. Deze waren: gravity en updateSpeed. Hiermee kon je doorgeven hoe snel je de elementen wil laten bewegen, en hoe sterk de zwaartekracht moet zijn.

```javascript

<script>
    //hierin worden de elementen gekoppeld aan de javascript functies

    var bounce1 = new Bounce();
    bounce1.init('bounce1', {gravity: 5, updateSpeed: 15});
    
</script>
```

Hierboven wordt de gravity: 5 en updateSpeed: 15 toegevoegd. Je kunt de gravity en speed aanpassen door andere waarde te geven om een andere resultaat te krijgen.

## Nieuwe functies

Amer en Thien hebben de originele demo aangepast door nieuwe functies te geven aan bestaande js file. Deze zij als volgt: 

- width , met deze functie wordt de breedte van elementen bepaald.
- height, met deze functie wordt de hoogte van elementen bepaald.
- moveX, met deze fucntie wordt de richting van element in X as aangegeven.
- borderRadius, met deze functie wordt de rondheid van element bepaald.
- backgrounColor, met deze functie wordt de achtergrond kleur van element bepaald.

Voorbeeld code van nieuwe toepassing:

```javascript

<script>
    //hierin worden de elementen gekoppeld aan de javascript functies

    var bounce1 = new Bounce();
    bounce1.init('bounce1', {gravity: 5, updateSpeed: 15, width: '500px', height: '200px', moveX: 4, borderRadius: '12px', backgroundColor: 'yellow'});
    
</script>
```

Hiermee krijg je je element sneller, die bounct hoger en die is best breed maar niet al te hoog. Die gaat van plek veranderen, met een rondere borders en een geele achtergrondkleur. Je kan natuurlijk die aanpassen volgens je smaak, en sommige dingen mag je ook achterlaten - dan worden de standard waarden vanuis js file toegepast.