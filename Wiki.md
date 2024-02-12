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
Ook hebben we aan de hand van [deze video](https://www.youtube.com/watch?v=i_23KUAEtUM) geleerd hoe je GIT in VS code kan gebruiken.
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

<br>

### Les 3

Bij de derde les zijn we bezig gegaan met het opfrissen van onze JavaScript kennis. Hierbij waren er 3 verschillende oefeningen die ik gemaakt heb. Deze oefeningen gingen over:

* Functies (parameters, return, arrow functies)
* Objecten (dot & bracket notatie)
* Loops
* import and export

<br> **De code hiervan is:**

<details>
 <summary>OEFENING 6</summary> <br>
 
 ```javascript
 /* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

/* OPDRACHT 1: Toon een Groetbericht */
// Schrijf een functie-expressie met de naam toonGroet die een groetbericht naar de console logt. De functie accepteert één parameter, naam, en toont een groetbericht met de opgegeven naam.

let toonGroet = function(naam) {
  console.log("Hallo " + naam + "!");
}

toonGroet("Jamie");

/* OPDRACHT 2: Tel getallen op en log het resultaat */
// Schrijf een functie-expressie met de naam telOpEnLog die twee getallen optelt en het resultaat naar de console logt. De functie accepteert twee parameters, getal1 en getal2, telt ze op en logt het resultaat.

let telOpEnLog = function(getal1, getal2) {
  console.log(getal1 + getal2);
}

telOpEnLog(2, 8);

// Onderstaande opdrachten vereisen het gebruik van het return sleutelwoord

/* OPDRACHT 3: Bereken de Oppervlakte van een Rechthoek */
// Schrijf een functie-expressie met de naam `berekenOppervlakteRechthoek` die de oppervlakte van een rechthoek berekent. De functie accepteert twee parameters, `lengte` en `breedte`.

let berekenOppervlakteRechthoek = function(lengte, breedte) {
  return lengte * breedte;
}

console.log(berekenOppervlakteRechthoek(3, 4))

/* OPDRACHT 4: Bepaal of een Getal Even is */
// Schrijf een functie-expressie met de naam `isEven` die controleert of een gegeven getal even is. De functie accepteert één parameter, `getal`.

let isEven = function(getal) {
  if(getal == getal) {
    console.log("Is even")
  } else {
    console.log("Is oneven")
  }
}

isEven(3);

/* OPDRACHT 5: Concateneer Twee Strings */
// Schrijf een functie-expressie met de naam `concateneerStrings` die twee strings concateneert. De functie accepteert twee parameters, `string1` en `string2`.

let concateneerStrings = function(string1, string2) {
  console.log(`${string1} ${string2}`)
}

concateneerStrings("Welkom,", "Jamie")

/* OPDRACHT 6: Herschrijf functies uit opdracht 1 en 5 naar een arrow functie */

let toonGroetArrow = (naam) => {
   console.log("Hallo " + naam + "!");
}

toonGroet("Jamie");


let telOpEnLogArrow = (getal1, getal2) => {
  console.log(getal1 + getal2);
}

telOpEnLogArrow(2, 8);


let berekenOppervlakteRechthoekArrow = (lengte, breedte) => {
  return lengte * breedte;
}

console.log(berekenOppervlakteRechthoekArrow(3, 4))


let isEvenArrow = (getal) => {
  if(getal == getal) {
    console.log("Is even")
  } else {
    console.log("Is oneven")
  }
}

isEvenArrow(3);


let concateneerStringsArrow = (string1, string2) => {
  console.log(`${string1} ${string2}`)
}

concateneerStringsArrow("Welkom,", "Jamie");
```

</details> <br>

<details>
 <summary>OEFENING 7</summary> <br>

 ```javascript
 /* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

/* OPDRACHT 1: Definieer een object */
// Definieer een eenvoudig object met de naam persoon dat de eigenschappen naam en leeftijd heeft. Geef het object de waarden "John" voor naam en 30 voor leeftijd.

let persoon = {
    naam: "John",
    leeftijd: 30
};

/* OPDRACHT 2: Uitbreiding */
// Breid het object persoon uit met verschillende soorten eigenschappen, zoals een string, een numerieke waarde, een boolean, en een array.

persoon.hobbies = ["gamen", "films kijken", "coderen"]
persoon.achternaam = "Bakker"
persoon.hasJob = false
persoon.droomBaan = "developer"

console.log(persoon);

/* OPDRACHT 3: Dot & bracket notation */
// Gebruik zowel dot notatie als bracket notatie om de waarde van de naam-eigenschap van het persoon-object op te halen en naar de console te loggen.

console.log(persoon.naam)
console.log(persoon.achternaam)
console.log(persoon['droomBaan'])
console.log(persoon['hasJob'])

/* OPDRACHT 4: Methode */
// Voeg een methode verjaardagVieren toe aan het persoon-object. Deze methode moet de leeftijd van de persoon met één verhogen. Je kan binnen het object naar de eigenschap leeftijd verwijzen met "this.leeftijd".

let persoon = {
   naam: "John",
   leeftijd: 30,
   verjaardagVieren() {
       this.leeftijd++;
       console.log(this.leeftijd)
   }
};

persoon.verjaardagVieren();

console.log(persoon.leeftijd)

/* OPDRACHT 5: Boodschap loggen */
// Breid de methode verjaardagVieren uit om een bericht naar de console te loggen waarin de naam en nieuwe leeftijd van de persoon worden weergegeven.


persoon.verjaardagVieren = function() {
    console.log(`Gefeliciteerd ${this.naam}, je bent alweer ${this.leeftijd}!`);
}

persoon.verjaardagVieren();
```
</details> <br>

<details>
 <summary>OEFENING 8</summary> <br>
 
 ```javascript
/* Met de toetscombinatie [CMD] + [/] kun je '//' voor de regel weghalen en terugplaatsen */

/* OPDRACHT 1: For loop - Tel tot 5 */
// Schrijf een for-loop die de getallen van 1 tot 5 logt naar de console.

for (let i = 1; i <= 5; i++) {
   console.log(i)
}

/* OPDRACHT 2: For loop - Maak de tafel van 3 */
// Schrijf een for-loop die de tafel van 3 logt naar de console (van 3 tot 30).

for (let i = 0; i <= 30; i+=3) {
   console.log(i)
}

/* OPDRACHT 3: While loop */
// Programmmer de herhalingen van opdracht 1 met een while loop

let i = 0; 
while(i < 5) {
i++
console.log(i)
}

/* OPDRACHT 4: While loop */
// Programmmer de herhalingen van opdracht 2 met een while loop

let i = 0; 
while(i < 30) {
i+=3
console.log(i)
}


/* OPDRACHT 5: For ... of loop - Log kleuren */
// Gegeven een array met kleuren (['rood', 'groen', 'blauw']), schrijf een for...of-loop om elke kleur naar de console te loggen.

let kleuren = ['rood', 'groen', 'blauw']

for (let kleur of kleuren) {
   console.log(kleur);
}


/* OPDRACHT 6: For ... of loop - Lengte van elk woord */
// Gegeven een array met woorden, schrijf een for...of-loop om de lengte van elk woord naar de console te loggen.

let woorden = ['appel', 'banaan', 'kiwi']

for (let letters of woorden) {
   console.log(letters.length)
}


/* OPDRACHT 7: For ... in loop - Log Eigenschappen */
// Gegeven een object met eigenschappen, schrijf een for...in-loop om elke eigenschap naar de console te loggen.

let persoon = { naam: 'John', leeftijd: 25, stad: 'Amsterdam' }

for (let property in persoon) {
   console.log(`${property}: ${persoon[property]}`)
}


/* OPDRACHT 8: For ... in loop - Log waarden */
// Gegeven een object met eigenschappen, schrijf een for...in-loop om elke eigenschap naar de console te loggen.

let telefoon = { merk: 'Samsung', model: 'Galaxy', jaar: 2022 }

for (let waarden in telefoon) {
   console.log(`${telefoon[waarden]}`);
}

```
</details> <br>

<details>
  <summary>EXTRA OEFENING (FILTEREN)</summary> <br>

  ```javascript
let valorant = {
    name: "VALORANT",
    genre: "FPS",
    multiplayer: true,
    developer: "Riot Games",
    rating: 5
}

let leagueoflegends = {
    name: "League of Legends",
    genre: "MOBA",
    multiplayer: true,
    developer: "Riot Games",
    rating: 4.5
}

let csgo = {
    name: "CS:GO",
    genre: "FPS",
    multiplayer: true,
    developer: "Valve",
    rating: 4
}

let assasinscreed = {
    name: "Assasin's Creed",
    genre: ["Action", "Adventure", "Stealth"],
    multiplayer: false,
    developer: "Ubisoft",
    rating: 3
}

let games = [valorant, csgo, leagueoflegends, assasinscreed]

console.log(games)

games.forEach(game => console.log(game.rating))

const FPSgames = games.filter(game => game.genre == "FPS" && game.rating > 4.5).forEach(game => console.log(game.name));

// console.log(FPSgames);

// FPSgames.forEach(game => console.log(game));

```
</details>

### Les 4

In les 4 hebben we voor het eerst kennis gemaakt met JSON. We hebben het gehad over de volgende onderwerpen en daar hebben we ook een opdracht bij gemaakt:

* JSON-notatie & -bestanden
* Fetch Web API & lokaal JSON bestand
* Promise afhandelen met .then()
* Fetch in Async functie met await <br>

**De code hiervan is:**

<details>
  <summary>OEFENING 9</summary> <br>

  ```json
{
    "games": [
        {
            "name": "VALORANT",
            "genre": "FPS",
            "rating": 5
        },
        {
            "name": "League of Legends",
            "genre": "MOBA",
            "rating": 4.5
        },
        {
            "name": "CS:GO",
            "genre": "FPS",
            "rating": 3
        },
        {
            "name": "Assasin's Creed",
            "genre": "Action-Adventure",
            "rating": 4
        }
    ]
}
```

  ```javascript
fetch('games.json')
    .then(response => {
        if(!response.ok) {
            throw new Error('Er is een error')
        }
        return response.json()
    })
    .then(allGames => {
        allGames.games.forEach(game => {
            console.log(game.name)
            const liElement = document.createElement('li')
            liElement.innerText = game.name
            ulElement.appendChild(liElement)
            h1Element.innerText = "Games"
        })
    })
    .catch(error => {
        console.error('Er heeft een fout plaatsgevonden')
    })
```
</details>
