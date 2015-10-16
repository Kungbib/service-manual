# service-manual
Checklistor och manualer för tjänsteutveckling.


## Redigera innehållet

Manualen är genererad från markdown-filer för att det ska vara så enkelt som möjligt att redigera innehållet.

För att redigera innehållet på en sida, tryck på en .md fil som ligger i roten av respositoriet. Då kommer du att få se markdown-filen i GitHubs preview. Klicka sedan på Pennan uppe till höger.

![Screenshot of edit button](http://kungbib.github.io/service-manual/assets/readme/screenshot_edit.png)

[Här kan du lära dig om Markdown-syntaxen](https://help.github.com/articles/markdown-basics/).

Om du vill förhandsgranska dina ändringar så kan du trycka på fliken "Preview changes". Metadatan kommer att synas som en tabell längst upp på sidan, i övrigt så speglar förhandsgranskningen det som kommer att synas i manualen.

När du är nöjd med dina ändringar så trycker du på knappen "Commit changes".

### Skapa ny sida

För att skapa en ny sida behöver du klona ner respositoriet och lägga till en egen fil som du döper till ``pagename.md`` (byt ut pagename).

För att din sida ska läsas in korrekt av template-generatorn så behöver du lägga till ett par rader metadata ovanför ditt innehåll.

#### Exempel (från styleguide.md)

    ---
    layout: guide
    title: Stilguide
    permalink: /stilguide/
    author: Ola Blissing
    authormail: ola.blissing@kb.se
    icon: image
    ---
    
#### Förklaring

  ``layout`` : Här matar du in vilken template din sida ska använda. Detta reglerar även var din sida kommer att dyka upp. Eftersom min sida är en guide så ska den använda layouten `guide`. Detta gör att den anropar de korrekta HTML-elementen och även att sidan dyker upp i våran lista på Guider.
  
  ``title`` : Titel på guiden
  
  ``permalink`` : Vilken URL som ska gälla för din guide
  
  ``author`` : Namn på kontaktperson
  
  ``authormail`` : Mail till kontaktpersonen
  
  ``icon`` : Ikon från [fontawesome](http://fontawesome.io/icons/), används bland annat till guidelistan.
