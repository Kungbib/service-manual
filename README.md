# Kungl. bibliotekets tjänstemanual
Manual för tjänsteutveckling hos Kungl. Biblioteket


## Redigera innehållet

Manualen är genererad från markdown-filer för att det ska vara så enkelt som möjligt att redigera innehållet.

För att redigera innehållet på en sida, navigera till mappen ``_content`` och en mapp som motsvarar den sektionen du vill redigera. Om du trycker på en fil med ändelsen ``.md`` kommer du att få se markdown-filen i GitHubs preview. Klicka sedan på Pennan uppe till höger.

![Screenshot of edit button](http://kungbib.github.io/service-manual/assets/readme/screenshot_edit.png)

[Här kan du lära dig om Markdown-syntaxen](https://help.github.com/articles/markdown-basics/).

Om du vill förhandsgranska dina ändringar så kan du trycka på fliken "Preview changes". Metadatan kommer att synas som en tabell längst upp på sidan, i övrigt så speglar förhandsgranskningen det som kommer att synas i manualen.

När du är nöjd med dina ändringar så trycker du på knappen "Commit changes".

### Skapa ny sida

För att skapa en ny sida, tryck på + ovanför mappstrukturen i repositoriet.

![Screenshot of new file button](http://kungbib.github.io/service-manual/assets/readme/screenshot_new_file.png)

Döp filen till ``pagename.md`` (byt ut pagename).

För att din sida ska läsas in korrekt av template-generatorn så behöver du lägga till ett par rader metadata ovanför ditt innehåll.

#### Exempel (från styleguide.md)

    ---
    layout: guide
    section: styleguide
    title: Stilguide
    permalink: /styleguide/
    author: Ola Blissing
    authormail: ola.blissing@kb.se
    icon: paint-brush
    top: true
    ---
    
##### Förklaring

  ``layout`` : Här anger du in vilken template din sida ska använda. Sannolikt ska du ange ``guide`` här.
  
  ``section`` : Vilken sektion din sida tillhör, sektionen har samma namn som mappen under ``_content`` (t ex ``styleguide`` eller ``communications``).
  
  ``title`` : Titel på sidan
  
  ``permalink`` : Vilken permalink som ska gälla för din sida. Följ mappstrukturen.
  
  ``top`` : Sätt denna till ``true`` om din sida är toppnivå för en sektion, annars ska du inte ange detta fältet.
  
  ``author`` : Gäller endast toppnivå för en sektion. Namn på kontaktperson.
  
  ``authormail`` : Gäller endast toppnivå för en sektion. Mail till kontaktpersonen.
  
  ``icon`` : Gäller endast toppnivå för en sektion. Ikon från [fontawesome](http://fontawesome.io/icons/), används bland annat till navigeringslistan. Ange ikonens namn utan ``fa-``-prefixen 
