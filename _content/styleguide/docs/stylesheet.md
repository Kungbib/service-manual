---
layout: guide
section: styleguide
title: Stilmall
permalink: /styleguide/stylesheet
---

Som en del av stilguiden finns en tillhörande stilmall.

Stilmallen är ett tema ovanpå [Twitter Bootstrap](http://getbootstrap.com/).

I den byggda CSS-filen inkluderar vi Bootstraps CSS inuti vår. Om du vill bygga ihop våra LESS-filer själv så behöver du importera Bootstraps LESS-filer när du bygger din CSS för att temat ska fungera.

## Användning

Stilmallen går att använda på ett par olika sätt som förklaras nedan.

### Färdig CSS-fil

Om du inte vill anpassa din tjänsts utseende i större grad så kan du [ladda ner CSS-filen](https://raw.githubusercontent.com/Kungbib/frontend-guide/master/dist/css/kb-style.css) och använda den rakt av. **Observera** att direkt länkning till denna fil inte bör göras, eftersom uppdateringar av stilmallen kan bryta din tjänsts layout.

Om du vill ha mer kontroll över vilken version du använder så kan du använda dig av Bower.

    $ bower install kungbib/frontend-guide
    
Alternativt (specifik version)

    $ bower install kungbib/frontend-guide#1.0.0
    
Sedan använder du dig av filen som ligger i mappen ``CSS``.

### LESS-filer

Om ditt projekt behöver större möjlighet för anpassning rekommenderas att du istället använder dig av våra LESS-filer och kompilerar dessa själv tillsammans med Bootstrap. Då får du tillgång till samtliga variabler från både Bootstrap och vårat tema.

LESS-filerna laddar du ner med hjälp av Bower.

    $ bower install kungbib/frontend-guide
    
Alternativt (specifik version)

    $ bower install kungbib/frontend-guide#1.0.0
    
Du bör sedan skapa en egen samlingsfil i ditt eget projekt där du importerar Bootstrap och våran samlingsfil ``kb-styles.less`` från mappen ``LESS``.

__Observera att våra LESS-filer inte inkluderar Bootstraps LESS-filer.__

Exempel:

    // Import standard bootstrap
    @import '../path/to/bootstrap/less/bootstrap.less';
    // Import KB styles
    @import '../path/to/kungbib-styles/dist/less/kb-styles.less';
    
    // Projekt specific styles
    h1 {
      background-color: @happy-magenta;   // variable from kb-styles
      border-radius: @border-radius-base; // variable from bootstrap
    ...
