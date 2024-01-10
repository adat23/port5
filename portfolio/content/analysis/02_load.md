---
Title: Load
Description: Rapport om laddningstider
---

Laddningstider
=======================

Detta är en rapport om den analys jag gjort på tre olika hemsidor och resultatet av detta.

Urval
-----------------------

Jag har valt att analysera hemsidorna <a href="forsvarsmakten.se" target="_blank">Försvarsmakten.se</a>, <a href="apple.se" target="_blank">apple.se</a> och <a href="karlskrona.se" target="_blank">karlskrona.se</a>. Valen gjorde jag för att det var tre olika sidor som jag själv var lite nyfiken på hur snabbt dom laddar in, jag visste sedan tidigare att alla tre nyttjar en hel del bilder på sina hemsidor. 

Metod
-----------------------

Denna undersökning har gjorts primärt med <a href="https://pagespeed.web.dev/" target="_blank">pagespeed.web.dev</a> som var väldigt användbar för att se olika inladdningshastigheter. Uttöver pagespeed har jag även nyttjat inspekteringsmöjligheten som är inbyggd i Chrome samt även excel för att sätta upp en tabell för de olika sökningarna på hemsidorna. 

Resultat
-----------------------

Resultatet från min undersökning är något varierande. Apples hemsida var den som på de flesta punkter hamnade på sämst inladdningstid och prestanda poäng i jämförelse med dom andra sidorna, det var dock när man laddade in den mobilanpassade hemsidan. Apples datorhemsida var den som hade bäst resultat på flest punkter jämfört med de andra två hemsidorna. 

## Försvarsmakten:
<a href="%base_url%/image/load/FM.png" target="_blank" aria-label="Försvarsmakten">
    <picture>
        <source media="(min-width: 101px)" srcset="%base_url%/image/load/FM.webp">
        <img src="%base_url%/image/load/FM.webp?width=50%&q=10%" alt="Försvarsmakten">
    </picture>
</a>

Försvarsmaktens datorhemsida låg stadigt på i stort sett likadana inladdningstider från gång till gång, om man kollar på resutatet från denna hemsidan kan man se att enbart 4,8mb laddas in i samband med uppkopplningen hit. Dem har en förhållandevis hög prestandapoäng från pagespeed på 78,7 i snitt. 
Mobilhemsidan däremot ligger något mer varierande i resultatet, jag kunde inte till 100% slutföra undersökningen på denna hemsida med inladdningsstorleken då jag antagligen laddat om hemsidan för många gånger när jag skulle kontrollera det så min dator blev blockerad, förhoppningsvis inte för alltid. 
<a href="%base_url%/image/load/baffin.png" target="_blank" aria-label="baffin">
    <picture>
        <source media="(min-width: 101px)" srcset="%base_url%/image/load/baffin.webp">
        <img src="%base_url%/image/load/baffin.webp&w=100&q=50" alt="Baffin">
    </picture>
</a>
Men misstänker att detta är ett skydd mot att någon skulle försöka dra ner hemsidans prestanda vilket ju i sig är bra för deras del. jag hanns köra alla testerna med pagespeed innan denna blockering trädde i kraft dock. När man jämför enbart mobilanpassade hemsidorna så hade Försvarsmakten flest snabbast/bäst resultat så det är positivt. Med ett snittpoäng på 59,7 ligger dom dock precis över Karlskrona kommun men ganska långt över apples hemsida. 

## Apple
<a href="%base_url%/image/load/apple.png" target="_blank" aria-label="Apple">
    <picture>
        <source media="(min-width: 101px)" srcset="%base_url%/image/load/apple.webp">
        <img src="%base_url%/image/load/apple.webp&w=100&q=50" alt="Apple">
    </picture>
</a>
Apples hemsida var den som varierade mest i resultat, dem hade ganska stor skillnad i inladdningsmängd från gång till gång, skiftande mellan 8,4mb till 13,7mb gav ett snitt på 11,9mb gör att dom har den tyngsta av hemsidorna som jag testade. Detta syns dock inte när sidan testades i Pagespeedtesten då den hade högst poäng och kortast inladdningstid på största objektet. 
Apples mobilanpassade sida däremot hade flest av dom lägsta resultaten i mina tester, med ett snitt poäng på enbart 35 och inladdningstid på 15,9s för största objektet. Inladdningsmängden på mobilsidan fick ett snitt på 8,7mb men likt datorhemsidan skiftar det en del mellan omladdningarna. 

## Karlskrona kommun
<a href="%base_url%/image/load/karlskrona.png" target="_blank" aria-label="Karlskrona">
    <picture>
        <source media="(min-width: 101px)" srcset="%base_url%/image/load/karlskrona.webp">
        <img src="%base_url%/image/load/karlskrona.webp&w=100&q=50" alt="karlskrona">
    </picture>
</a>
Karlskrona kommuns hemsida är den sida som fick lägst poäng från Pagespeed, 78,3 kanske inte är så lågt men det är det lägsta resultatet mellan dessa tre sidor, dock är de snabbast i testet från Chromes dev tool där den har en inladdningstid i snitt på 1,4s. 
Mobilhemsidan från Karlskrona Kommun ligger nästa lika högt i poäng som Försvarsmakten, ett snitt på 59,3(FM: 59,7). 
Varken mobilhemsidan eller datorhemsidan varierar något i inladdningsmängd, 6mb varje gång för datorhemsidan och 6,2mb för mobilhemsidan. 
 
Analys
-----------------------

Det jag tyckte var mest förvånande var hur stor skillnad det var på att ladda in mobilhemsidan emot datorhemsidorna, jag var även något förvånad över att inte Apple hade bättre resultat som är ett stort företag jämfört med en Kommun och en statlig verksamhet, varken någon av hemsidorna är dock något som jag upplever som långsam inladdningstid. Högsta speedindex jag mätte upp var 9,4s för Apples mobilhemsida. 
Det som jag skulle kunna konstatera som eventuellt kan förbättra hemsidornas resultat något är antalet bilder och animationer som finns på respektive hemsida. Utöver bilder är det inte mycket mer information än text på indexsidorna så nästa steg skulle kunna vara att kontrollera servervalen dem olika företagen gjort. 

Referenser
-----------------------

<iframe class="excel" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQKFli6qCs_qUPrHGxHee_kLvBYSYbkA_SjLqHdQJu2b_El4njXoQyT3zE71d8YOA_PudSCJhGRliu1/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" title="referens"></iframe>

Övrigt
-----------------------

Denna rapport är skriven av Adam Antonsson. 