# PROJECT TECH Wiki

## Inhoudsopgave

* Week 1
  * Les 1
  * Les 2
  * Les 3
  * Les 4

* Week 2
  * Les 1
  * Les 2
  * Les 3
    * Back-End
    * Front-End
  * Les 4

* Week 3
  * Les 1
    * Back-End
    * Front-End
  * Les 2
  * Les 3<br>



## Week 1

### Les 1

Bij deze eerste les zijn we bezig gegaan met het bekijken van de planning van dit project en met het opfrissen van onze JavaScript kennis. 
Hierbij waren er 4 verschillende oefeningen die ik gemaakt heb. Deze oefeningen gingen over:

* Variabelen
* Datatypen
* Logica
* Arrays

<br> **De code hiervan is:**

<details>

<summary>OEFENING 1</summary><br>

```javascript

/* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

/* OPDRACHT 1 Optellen en vergelijken */

// Maak twee variabelen 'getal1' en 'getal2' en wijs er numerieke waarden aan toe.
// Voeg ze samen en sla het resultaat op in een nieuwe variabele 'som'.
// Controleer vervolgens of 'getal1' en 'getal2' aan elkaar gelijk zijn en sla het resultaat op in een variabele 'gelijk'.

let getal1 = 10;
let getal2 = 20;

let som = getal1 + getal2;

console.log(som);

let gelijk = getal1 == getal2;

console.log(gelijk);


/* Opdracht 2 String concatenatie */ 

// Maak drie variabelen 'voornaam', 'tussenvoegsel' en 'achternaam'.
// Voeg ze samen tot een volledige naam en sla het resultaat op in de variabele 'volledigeNaam'.

var voornaam;
var tussenvoegsel;
var achternaam;

var volledigeNaam = `${voornaam} ${tussenvoegsel} ${achternaam}`;

console.log(volledigeNaam);

/* Opdracht 3 Logische operatoren */

// Maak drie variabelen 'isZonnig' (boolean), 'temperatuur' (number) en 'isWeekend' (boolean).
// Gebruik logische operatoren om een nieuwe variabele 'buitenActiviteit' te maken.
// Buitenactiviteit moet waar (true) zijn als het zonnig is, de temperatuur boven 20 graden ligt en het weekend is.
 
 let isZonning = true;
 let temperatuur = 23;
 let isWeekend = false;
 
 let buitenActiviteit = (isZonning == true && temperatuur > 20 && isWeekend == true);

 console.log(buitenActiviteit);
 

/* Opdracht 4 Vergelijking en negatie */

// Maak twee variabelen 'a' en 'b' en wijs er numerieke waarden aan toe.
// Maak een nieuwe variabele 'isNietGelijk' die waar is als 'a' niet gelijk is aan 'b'.

let a = 21;
let b = 43;

isNietGelijk = (a != b);

console.log(isNietGelijk)

```

</details> <br>

<details>
  <summary>OEFENING 2</summary><br>

  ```javascript

/* OPDRACHT 1 Herdeclaratie */

/* Selecteer regel 5 t/m 8. Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen om de opdracht te kunnen maken */

// Probeer de variabele score opnieuw te declareren en kijk of er fouten optreden
let score = 5;
// Plaats hier de juiste declaratie
score = 10;
console.log(score);



/* OPDRACHT 2 Hertoekennen van een constante */

const PI = 3.14;
// Probeer hier een nieuwe waarde aan de constante toe te kennen
// PI = 3.21;
console.log(PI); // Wat wordt hier uitgevoerd?



/* OPDRACHT 3 Function scope */

// Gebruik let en const in plaats van var. Wat is het gevolg voor de uitvoer?
function exampleScope() {
    if (true) {
        var x = 10;
    }
    console.log(x);
}

exampleScope()



/* Opdracht 4 Hoisting van variabele */

// 1. Wat wordt er gelogd en waarom? Test dit.
// console.log(z)
// var z = 15

// 2. Plaats de definitie boven de console.log. Wat is de uitvoer nu?
var z = 15
console.log(z)


/* Opdracht 5a Hoisting van functie declaratie */

// Wat wordt er gelogd en waarom?
hoistingVoorbeeld()

function hoistingVoorbeeld() {
    console.log("Dit is een voorbeeld van hoisting bij functies!")
}


/* Opdracht 5b Hoisting van functie definitie */ 

// Bekijk onderstaande code. Wat verwacht je dat er zal gebeuren?

// hoistingVoorbeeldTwee()

// var hoistingVoorbeeldTwee = function() {
//     console.log("Dit is een voorbeeld van hoisting met een functie-definitie!")
// }

// Plaats het aanroepen van de functie onder de definitie. Wat wordt de uitvoer? Voorspel en test. 

var hoistingVoorbeeldTwee = function() {
    console.log("Dit is een voorbeeld van hoisting met een functie-definitie!")
}

hoistingVoorbeeldTwee()

/* Opdracht 6 Global en local scope */

// Global scope
var globalVar = "Dit is een globale variabele (var)";
let globalLet = "Dit is een globale variabele (let)";
const globalConst = "Dit is een globale variabele (const)";

function voorbeeldScope() {
    // Local scope
    var localVar = "Dit is een lokale variabele (var)";
    let localLet = "Dit is een lokale variabele (let)";
    const localConst = "Dit is een lokale variabele (const)";

    console.log("In de lokale scope:");
    console.log(localVar); // Werkt
    console.log(localLet); // Werkt
    console.log(localConst); // Werkt

    console.log("In de globale scope (toegankelijk vanuit de lokale scope):");
    console.log(globalVar); // Werkt
    console.log(globalLet); // Werkt
    console.log(globalConst); // Werkt
}

// Probeer toegang te krijgen tot lokale variabelen buiten hun scope
// console.log(localVar); // Dit zou een fout veroorzaken
// console.log(localLet); // Dit zou een fout veroorzaken
// console.log(localConst); // Dit zou een fout veroorzaken

// De globale variabelen zijn beschikbaar in de globale scope
console.log("In de globale scope:");
console.log(globalVar); // Werkt
console.log(globalLet); // Werkt
console.log(globalConst); // Werkt

voorbeeldScope(); // Roep de functie aan om de lokale scope te betreden

```

</details> <br>

<details>
  <summary>OEFENING 3</summary> <br>

  ```javascript

  /* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

// Hier zijn vijf oefenopdrachten voor het aanmaken van arrays in JavaScript

/* OPDRACHT 1 Numerieke array */
// Maak een array met de naam `getallen` en voeg drie verschillende numerieke waarden toe.

let getallen = [1, 4, 6];



/* OPDRACHT 2 String array */
// Maak een array met de naam `woorden` en voeg vijf verschillende woorden of zinnen toe als strings.

let woorden = ['woord', 'dit is een zin', 'hallo', 'dit is de 4de zin', 'laatste zin']

/* OPDRACHT 3 Gemengde datatypen */
// Maak een array met de naam `gemengd` en voeg elementen toe van verschillende datatypen, zoals getallen, strings en booleans.

let gemengd = [1, 'woord', true] 

/* OPDRACHT 4 Nested array */
// Maak een array met de naam `nested` en voeg een andere array toe als een van de elementen.

let nested = [gemengd, 24, 'hallo', false]

console.log(nested);

```
</details> <br>

<details>
  <summary>OEFENING 4</summary><br>

  ```javascript
  /* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

// Hier zijn oefenopdrachten voor het gebruiken van array methoden in JavaScript

/* OPDRACHT 1. push */
// Maak een array `getallen` met enkele numerieke waarden. Voeg een nieuw getal toe aan het einde van de array met de `push`-methode.

let getallen = [1, 5, 6, 20];

getallen.push(25);

console.log(getallen);

/* OPDRACHT 2. pop */
// Maak een array `dieren` met enkele stringwaarden. Verwijder het laatste element uit de array met de `pop`-methode.

let dieren = ['leeuw', 'tijger', 'kat', 'giraffe'];

dieren.pop();

console.log(dieren);

/* OPDRACHT 3. shift */
// Maak een array `kleuren` met enkele stringwaarden. Verwijder het eerste element uit de array met de `shift`-methode.

let kleuren = ['rood', 'groen', ' blauw', 'paars', 'oranje']

kleuren.shift();

console.log(kleuren);

/* OPDRACHT 4. unshift */
// Maak een array `fruit` met enkele stringwaarden. Voeg een nieuw element toe aan het begin van de array met de `unshift`-methode.

let fruit = ['appel', 'peer', 'banaan', 'kiwi', 'sinasappel'];

fruit.unshift('lychee');

console.log(fruit);

/* OPDRACHT 5. indexOf */
// Maak een array `steden` met enkele stringwaarden. Gebruik de `indexOf`-methode om de index van een specifieke stad in de array te vinden.

let steden = ['Almere', 'Amsterdam', 'Utrecht', 'Rotterdam'];

console.log(steden.indexOf('Amsterdam'));

/* OPDRACHT 6. splice */
// Maak een array `gerechten` met enkele stringwaarden. Gebruik de `splice`-methode om een specifiek gerecht te vervangen door een nieuw gerecht.

let gerechten = ['sushi', 'pizza', 'pokebowl', 'hamburger'];

gerechten.splice(1, 1, 'pasta');

console.log(gerechten);

/* OPDRACHT 7. slice */
// Maak een array `nummers` met enkele numerieke waarden. Gebruik de `slice`-methode om een nieuw array te maken dat bestaat uit een deel van de originele array.

let nummers = [1, 2, 3, 4, 5, 6]
let nieuweNummers = nummers.slice(0, 3);

console.log(nieuweNummers);

/* OPDRACHT 8. Combinatie van methoden */
// Maak een array `namen` met enkele stringwaarden. Voer verschillende bewerkingen uit op de array, zoals het toevoegen, verwijderen en vervangen van elementen met behulp van verschillende array-methoden.

let namen = ['Jamie', 'Soraya', 'Jan']

namen.push('Yasin');

console.log(namen);

namen.shift();

console.log(namen);

namen.unshift('Tirbeni');

console.log(namen)

let paarNamen = namen.splice(0, 2);

console.log(paarNamen);

paarNamen.splice(0, 1, 'Jamie')

console.log(paarNamen);

```
</details><br>

### Les 2

In de tweede les van deze week hebben we geleerd wat GIT en Github is en hoe je deze kan gebruiken.
Ik heb uit deze les gehaald dat GIT erg handig is voor version control en samenwerken en ik zal ook zeker proberen om dit vanaf nu te gaan implementeren in mijn werk.
Ook hebben we het gehad over repositories in Github en daarvan heb ik voor dit project ook eentje aangemaakt.

![Afbeelding van een Github repository](https://static.codex.so/upload/redactor_images/o_602d344e24f1f5ac13cb05022089101e.jpg)
bron: [codex.so](https://codex.so/fork-and-pull-en)

Ook heb ik deze Wiki aangemaakt in deze les, de README.md en ben ik begonnen met de LICENSE.
Hiervoor hebben we gekeken naar andere repositories op Github om zo te kijken wat er allemaal in deze dingen moet komen te staan.
De belangrijkste dingen zijn:

* Titel project
* Inhoudsopgave
* Samenvatting van wat het project is
* Handleiding opzetten
* Libraries
* Contributors
* Versie
* License

### Les 3

### Les 4
