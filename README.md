# The Client - Website

Ontwerp en maak een website voor een opdrachtgever en bespreek het resultaat tijdens de Sprint Review.

De instructie van deze leertaak staan in de [WIKI](https://github.com/fdnd-task/the-client-website/wiki)



## Inhoudsopgave Readme

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Intro
Voor deze opdracht ben ik aan de slag gegaan aan het project PediaConnect. PediaConnect is bedacht om de drempel voor sociale contacten te verlagen voor kinderartsen. Door hier een platform voor te maken, kunnen artsen makkelijker contact leggen met elkaar en kennis delen. 

## Beschrijving
De website voor PediaConnect is op dit moment nog in ontwikkeling en wordt mobile-first gecodeerd. Dit houdt in dat het als eerst werkende moet zijn op telefoon en daarna op desktop. Hierdoor is er te zien dat de website nog minder "af" voelt zodra de website geschaald wordt tot desktop-grootte.
Op de website kom je binnen op het dashboard. Vanuit daar krijg je een overzicht te zien van wat er allemaal mogelijk is op de website. De website wordt op dit moment gebouwd met de gedachte dat de gebruiker al is ingelogd waardoor alle opties zichtbaar zijn. Zo zouden gebruikers vanuit het dashboard naar andere pagina's kunnen via de drie grote knoppen bovenaan of kunnen ze gebruik maken van het hamburger-menu bovenin om te navigeren naar andere pagina's. Ook staan er onderin het scherm allemaal mogelijkheden, zoals de knop "home" en "berichten". 

Dit is de link naar de PediaConnect website:
https://xinjuliette.github.io/the-client-website/
<img width="495" height="1203" alt="Schermafbeelding 2026-10-08 094447" src="https://github.com/user-attachments/assets/9c74c6ea-345a-4f8b-9a68-60d364080194" />
<img width="2556" height="1266" alt="Schermafbeelding 2026-10-08 094557" src="https://github.com/user-attachments/assets/dc568d10-8fc9-45f9-8188-47f21842d607" />
<!-- In de Beschrijving staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->

## Kenmerken
Om deze website te bouwen is er gebruik gemaakt van HTML, CSS en een klein gedeelte javascript. De website wordt nagebouwd op basis van het werk van een voormalig CMD-student die deze website heeft ontworpen.
De code is begonnen bij HTML waar de volgorde van coderen op basis van de website is (van boven naar beneden). Ik ben begonnen met de navigatie (logo, dashboard en het hamburger-menu). Voor het hamburger-menu staat er een klein onderdeel javascript. Dit script zorgt ervoor dat de navigatie uitklapt wanneer je erop klikt.
```ruby
        <script>
            function myFunction() {
            var x = document.getElementById("navlinks");
            if (x.style.display === "grid") {
                x.style.display = "none";
            } else {
                x.style.display = "grid";
            }
            }
        </script>
```
Zowel de <na> en de <footer> staan in de style.css omdat dit geldt door de gehele website heen. Elementen die enkel op één pagina zitten van de website staan in de CSS voor die specifieke pagina. Ik heb hier duidelijk onderscheid in gemaakt zodat alles overzichtelijk blijft.

Bepaalde onderdelen delen dezelfde code omdat deze bijna precies hetzelfde zijn. Zoals de twee buttons bij "recommended for you" en ook de twee buttons bij "your bookmarked content"

```purple
.recommended-buttons, .bookmarked-buttons {  
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 100%;

    button {
        border-color: transparent;
    }
    button:nth-of-type(1) {
        width:fit-content;
        justify-self: start;
        padding: 0.5em 1em 0.5em 1em;
        border-radius: 8px;
        background-color: var(--midgrey); 
    }
    button:nth-of-type(1):hover {
        background-color: var(--darkgrey);
        color: white;
            svg {
                path {
                    fill: white;
                }
            }
    }
    button:nth-of-type(2) {
        width: fit-content;
        justify-self: end;
        padding:1em;
        border-radius: 8px;;
    }
    button:nth-of-type(2):hover {
        background-color: var(--darkgrey);
                    svg {
                path {
                    fill: white;
                }
            }
    }
} 	  
```
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framework of library gebruikt? -->



## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
