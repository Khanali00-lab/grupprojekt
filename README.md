# grupprojekt

#Grupp 28 med medlemmar: 
#Ali Ahsani
#Niklas Pallon
#Christer Dahl
---------------

##### Vi bestämde oss att göra det klassiska Sanke spelet. Först gjorde gjorde vi ett schema över hur spelet ska fungera samt vad det ska göra. Vi kom på 7 olika steg: skapa # en orm kropp, flytta ormen, styra ormen, upptäcka kollison med mat, skapa en poöngtavla, upptäck kollision med svans och upptäck kollision med vägg. Därefter gjirde vi # klassdiagram med tillhörande klasser och attributer för att göra det enklare för oss att skriva kod. Vi delade upp koden i 4 olika filer. 
 Klassen "Mat" ärver från Turtle och har metoder för att skapa och uppdatera maten. Klassen "Orm" har metoder för att skapa och styra ormen samt upptäcka kollision med   mat, vägg och svans. Klassen "Poangtavla" ärver också från Turtle och har metoder för att hantera poängsystemet och Game Over-texten.

I huvudprogrammet skapas en skärm och dess dimensioner sätts. En svart bakgrund och titel sätts också på skärmen. Tracer-metoden används för att hindra skärmen från att  uppdateras tills det behövs.

Sedan skapas instanser av ormen, maten och poängtavlan. Key-listeners läggs till skärmen för att reagera på upp, ner, vänster och höger piltangenterna. Ett boolskt   värde "spelet_är_igång" skapas och används för att avsluta spelet när ormen kolliderar med väggen eller sig själv.

Medan spelet fortlöper uppdateras skärmen och en "sleep" används för att avgränsa hur ofta ormen rör sig. Ormen rör sig med hjälp av metoden "flytta". Kollision med mat upptäcks och poängtavlan, maten och ormen uppdateras. Kollision med vägg eller svans upptäcks också och spelet avslutas.

Till sist anropas exitonclick-metoden för att avsluta spelet när användaren klickar på skärmen.
