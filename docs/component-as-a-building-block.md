# Don't Repeat Yourself - Component Library

## Component as a Building Block

Ontwerp en ontwikkel een component voor jouw component library.

## Aanpak
Het ontwikkelen van een component voor een component library zorgt voor herbruikbaarheid, consistentie en schaalbaarheid binnen projecten. Het maakt samenwerking tussen teams eenvoudiger, versnelt de ontwikkeling en verbetert de onderhoudbaarheid van de code.

N.B.: Zorg er voor dat stap 1 t/m 5 voor woensdag zijn afgerond. Tijdens de les over *the new responsive* wordt aandacht gegeven aan container queries, het is belangrijk dat je de ontwerpfase dan afgerond hebt!

1. Beschrijf tekstueel de functie en eigenschappen die het component heeft. Het is handig als je met iemand uit je team overlegt om te bepalen of het idee wat je hebt bij het component volledig is. Meestal plaats je deze tekst in de issue of sub-issue.
2. Maak (op papier!) een morphologische kaart om variatie in de uitwerking van het component te onderzoeken. Elke functie kan immers op veel verschillende manieren uitgewerkt worden en een goed onderbouwde keuze heeft minstens een aantal alternatieven onderzocht.
3. Onderweg zoek je inspiratie op het web, kijk naar hoe anderen bepaalde dingen hebben aangepakt. Bewaar de door jou gevonden inspiratie door screenshots in Figma bij elkaar te plaatsen. [divergeren]
3. Gebruik jouw morphologische kaart om vijf variaties te genereren. Werk deze variaties grof uit in Figma door een LoFi wireframe te ‘schetsen’. [divergeren]
4. Beargumenteer welke variatie of combinatie van eigenschappen van variaties je uiteindelijk kiest. [convergeren]
5. Maak een HiFi wireframe van de door jou gekozen variatie. Zorg ervoor dat je weet hoe jouw component er uit ziet op verschillende schermgroottes, maak een *repsonsive design*. [convergeren]
6. Implementeer jouw component in sveltekit. Begin met het neerzetten van een semantische HTML structuur met dummy-content. Werk *mobile-first* aan de CSS en gebruik hierbij container queries voor *responsivity*, vanzelfsprekend werk je *progressive enhanced*. Dit houdt in dat de pagina waarop je dit component gebruikt bepaalt hoeveel breedte er is. Het kan helpen om een kale test-route met een `+page.svelte` te maken waarin je jouw component meerdere keren met verschillende ruimte aanroept. Op die manier zie je de verschillende verschijningsvormen van jouw component terwijl je aan de CSS werkt.
7. Test jouw component lokaal doorlopend. Responsiviteit is eenvoudig want je werkt met container-queries. Test met lighthouse op *accessibility* en *performance*, zorg ook dat je de handmatige tests uitvoert. Je hoeft in deze fase nog geen device- of user test uit te voeren.
8. Als je lokaal tevreden bent voer je een pull-request uit naar de `dev`-branch om jouw component te integreren met de code-base. Na controle door een teamlid kan jouw component gemerged worden.
9. Test na publicatie remote door de url naar jouw netlify pagina te openen in de browser. Remote testen levert een ander inzicht dan lokaal omdat jouw component nu in relatie met andere paginaonderdelen ingeladen wordt. Voer opnieuw tests uit voor *accessibility* en *performance*. Probeer ook de url op verschillende mobiele devices te openen, doe een grondige devicetest.
10. Als meerdere componenten uit jouw team geïntegreerd zijn, plan je [een user test](https://github.com/fdnd-task/fix-the-flow-interactive-website/blob/main/docs/code-design-review-user-testing.md#user-testing) om de werking van jullie systeem te testen. Een user test heeft een plan (wat wil je testen) en wordt uitgevoerd op personen die i) niet in jouw ontwikkelteam zitten en ii) geen frontender zijn.

## Bronnen

- [Morphological Chart uit de Delft Design Guide @ Cornell.edu](https://arl.human.cornell.edu/PAGES_Delft/Morpholigical_Chart-deeper.pdf)
- [Learn how to Brainstorm Ideas with a Morphological Chart @ YouTube](https://www.youtube.com/watch?v=ZsT2F1eTpMM)
