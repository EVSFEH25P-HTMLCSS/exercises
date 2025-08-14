# Övningar - Vecka 1

## Kom igång

Det finns många inställningar och tillägg i VSCode (Visual Studio Code). Du kan ändra färgtema, font och mer. Det rekommenderas att installera `Live Server` minst, vilket är ett tillägg som tillåter en att skapa en dev-server. Det betyder att du kan utveckla HTML & CSS smidigare.

Ett projekt med HTML & CSS innebär egentligen bara att skapa en fil, eller två om man vill dela upp koden i två delar (en fil för HTML och en för CSS). Börja med att skapa en `index.html` fil och starta den med `Live Server`. Du gör detta genom att högerklick på filen i VSCode och välja "Start Live Server".

## Del 1: Grundläggande HTML

### 1. Tags

Den mest fundamentala byggstenen i HTML är tags som används för att bilda element. Nämn några tags som finns i HTML.

### 2. Element

Det finns främst två typer av tags: start tags och end tags. Tillsammans bildar dem element. Skapa ett `div`-element, ett `span`-element och ett `button`-element.

### 3. Hur många element?

Hur många element finns i följande kod?

```html
<div>
  <span>
    <article></article>
  </span>
  <button></button>
  <p><div></div></p>
</div>
```

### 4. Hur många tags?

Hur många tags finns i följande kod?

```html
<section>
  <span> <div></div></span>
  <button></button>
  <span
    ><div>
      <article><p></p></article></div
  ></span>
</section>
```

### 5. Hur många barn?

Hur många barn finns i följande kod?

```html
<section>
  <span> <div></div></span>
  <button></button>
  <span
    ><div>
      <article><p></p></article></div
  ></span>
</section>
```

### 6. Hur många föräldrar?

Hur många föräldrar finns i följande kod?

```html
<div>
  <span>
    <article></article>
  </span>
  <button></button>
  <p><div></div></p>
</div>
```

### 7. Konstig formatering

Följande kod är inte formaterad korrekt. Indentera den manuellt, utan hjälpmedel (utan VSCode "format document"), så att det blir korrekt.

```
<div>
<div>
<div>
<div></div><div></div></div>
</div>
<div></div>
</div>
```

### 8. Klasser och idn

Skapa ett element med klassen "candy" och id:t "icecream".

### 9. Hitta alla fel

Hitta alla fel i följande avsnitt kod.

```
<div>
  <div>
    </p>Hello!</p>
  </div>
  <span>Welcome to my website!<span>
  <button>Click Me!</button>
</div>
```

```
<div>
  <span>
    <p><//p>
  </span>
  <span>
    <div></p>
  </span>
  <span>
    <span></span>
  </span>
  <span>
    <span><span></span>
  <span>
</div>
```

```
<div>
  <span>abcabcabcabcabcabc</div>
  <div>>abcabcabcabcabcabc</span>
  <button>abcabcabcabcabcabc</button>
  <p>abcabcabcabcabcabc
    <span>abcabcabcabcabcabc</span>
    <div>abcabcabcabcabcabc</div>
  <p>abcabcabcabcabcabc</p>
</div>
```

### 10. Numrerade listor

Skapa en numrerad lista (`ol`) med minst fem namn på länder.

### 11. Onumrerade listor

Skapa en onumrerad lista (`ul`) med minst tre valfria saker.

### 12. Knappar

Skapa tre olika knappar med valfri text.

### 13. Länkar

Skapa en länk till en rolig Youtube video.

### 14. Meeeeeeemes

Lägg in en bild på en rolig meme (eller annan valfri bild).

### 15. Byt titel

Byt titeln på din webbsida genom `<title>` taggen.

### 16 Kommentarer

Kopiera följande HTML kod och kommentera ut rad 3.

```html
<h1>My awesome website!</h1>
<p>Welcome to my website</p>
TODO: I need to remember to add a link here
```

### 17. Flerradskommentarer

Kopiera följande HTML kod och kommentera ut rad 3 och 4 med en enda kommentar.

```html
<h1>Music hits</h1>
<p>Welcome Music Hits! The best website to find awesome music.</p>
TODO: Add a picture of a popular music band. Also, make the picture fade into
the rest of the website to make it look cool.
```

### 18. Nedladdning

Gör så att man kan ladda ned följande bild (genom en länk): [https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.seobility.net%2Fen%2Fwiki%2Fimages%2Fthumb%2F0%2F04%2FFrontend-vs-Backend.png%2F675px-Frontend-vs-Backend.png&f=1&nofb=1&ipt=68fd05fa9ba6558bc2143e59bca7649a037b3715fa60e37a9e734489d32b17c2&ipo=images](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.seobility.net%2Fen%2Fwiki%2Fimages%2Fthumb%2F0%2F04%2FFrontend-vs-Backend.png%2F675px-Frontend-vs-Backend.png&f=1&nofb=1&ipt=68fd05fa9ba6558bc2143e59bca7649a037b3715fa60e37a9e734489d32b17c2&ipo=images)

### 19. Interna länkar

Kopiera följande HTML kod som innehåller information från Wikipedia. Lägg till tre länkar i början av dokumentet som kan användas för att hoppa mellan alla rubriker på sidan (HTML, History och Markup).

```html
<h1>HTML</h1>

<p>
  The HyperText Markup Language or HTML is the standard markup language for
  documents designed to be displayed in a web browser. It defines the meaning
  and structure of web content. It is often assisted by technologies such as
  Cascading Style Sheets (CSS) and scripting languages such as JavaScript. Web
  browsers receive HTML documents from a web server or from local storage and
  render the documents into multimedia web pages. HTML describes the structure
  of a web page semantically and originally included cues for its appearance.
  HTML elements are the building blocks of HTML pages. With HTML constructs,
  images and other objects such as interactive forms may be embedded into the
  rendered page. HTML provides a means to create structured documents by
  denoting structural semantics for text such as headings, paragraphs, lists,
  links, quotes, and other items. HTML elements are delineated by tags, written
  using angle brackets. Tags such as `img` and `input` directly introduce
  content into the page. Other tags such as `p` and `/p` surround and provide
  information about document text and may include sub-element tags. Browsers do
  not display the HTML tags but use them to interpret the content of the page.
  HTML can embed programs written in a scripting language such as JavaScript,
  which affects the behavior and content of web pages. The inclusion of CSS
  defines the look and layout of content. The World Wide Web Consortium (W3C),
  former maintainer of the HTML and current maintainer of the CSS standards, has
  encouraged the use of CSS over explicit presentational HTML since 1997.[2] A
  form of HTML, known as HTML5, is used to display video and audio, primarily
  using the `canvas` element, together with JavaScript.
</p>

<h2>History</h2>

<p>
  In 1980, physicist Tim Berners-Lee, a contractor at CERN, proposed and
  prototyped ENQUIRE, a system for CERN researchers to use and share documents.
  In 1989, Berners-Lee wrote a memo proposing an Internet-based hypertext
  system.[3] Berners-Lee specified HTML and wrote the browser and server
  software in late 1990. That year, Berners-Lee and CERN data systems engineer
  Robert Cailliau collaborated on a joint request for funding, but the project
  was not formally adopted by CERN. In his personal notes of 1990, Berners-Lee
  listed "some of the many areas in which hypertext is used"; an encyclopedia is
  the first entry.[4] The first publicly available description of HTML was a
  document called "HTML Tags",[5] first mentioned on the Internet by Tim
  Berners-Lee in late 1991.[6][7] It describes 18 elements comprising the
  initial, relatively simple design of HTML. Except for the hyperlink tag, these
  were strongly influenced by SGMLguid, an in-house Standard Generalized Markup
  Language (SGML)-based documentation format at CERN. Eleven of these elements
  still exist in HTML 4.[8]
</p>

<h2>Markup</h2>

<p>
  HTML markup consists of several key components, including those called tags
  (and their attributes), character-based data types, character references and
  entity references. HTML tags most commonly come in pairs like `h1` and `/h1`,
  although some represent empty elements and so are unpaired, for example `img`.
  The first tag in such a pair is the start tag, and the second is the end tag
  (they are also called opening tags and closing tags). Another important
  component is the HTML document type declaration, which triggers standards mode
  rendering.
</p>
```

### 20. **BOLD** text

Lägg till följande text som fet (bold) text med hjälp av HTML (ingen CSS):

**HTML is a markup language.**

### 21. Details

Skapa en "hint" komponent med HTML, likt denna:

<details>
Använd `details` egenskapen.
<summary>
Hint
</summary>
</details>

### 22. Dropdowns

Skapa en dropdown lista med följande alternativ:

- Godis
- Glass
- Chips
- Bullar

## Del 2: Gruppövning

Varje person väljer en av följande punkter att söka information om. Efter en stund så berättar varje person i gruppen om ämnet för alla andra i gruppen.

- Längd enheter (px, rem, % m.m)
- Färg enheter (rgb, hsl m.m)
- Display egenskapen
- Position egenskapen
- Skapa och länka till andra dokument (som man själv har)
- Vanliga saker som finns i `head` elementet
- Regler för namngivning på id:n och klasser
- Välj åtta attributer valfritt
- Välj åtta CSS egenskaper valfritt
- Välj åtta tags valfritt

## Del 3: Grundläggande CSS

### 1. Egenskaper

Egenskaper används i CSS för att styla element. Nämn några CSS egenskaper.

### 2. Selectors

För att applicera egenskaper på element så måste dem väljas med selectors.

1. Vilken symbol används för class-selectors?
2. Vilken symbol används för id-selectors?
3. Vad kan man skriva om man vill applicera egenskaper på alla element av en viss tag, exempelvis alla divs?

<details>
  <summary>
    Hints
  </summary>
    1. Den används i slutet av meningar.
    2. Hex färger kan beskrivas med denna symbol i början.
    3. Det är ingen symbol.
</details>

### 3. Blå och röd

Skapa två divs med HTML och lägg in valfri text i dem. Färga den ena blå och den andra röd.

<details>
  <summary>
    Hint
  </summary>
  Använd idn för att skilja på båda divs.
</details>

### 4. Gigantisk text

Skapa en paragraf med HTML och lägg in valfri text. Gör texten gigantisk med CSS.

<details>
  <summary>
    Hint
  </summary>
  font-size
</details>

### 5. Now you see me, now you don't

Lägg in följande kod som HTML. Gör sedan `div`-elementet osynligt med CSS.

```html
<div id="hello">Hello</div>
```

<details>
  <summary>
    Hint
  </summary>
  Det finns flera egenskaper som kan göra ett element osynligt.
</details>

### 6. Det går inte, men varför inte?

Du kan inte använda `px` på `background` egenskapen. Varför inte?

<details>
  <summary>
    Hint
  </summary>
  Man kan inte säga: Det är fem liter att gå till affären
</details>

### 7. Konstig formatering

Följande kod är inte formaterad korrekt. Indentera den manuellt, utan hjälpmedel (utan VSCode "format document"), och fixa andra fel, så att det blir korrekt.

```
div {
background:red;
    color:white
   height: 10px;
}
```

### 8. Rätt enheter

Nämn alla enheter som kan användas på `width` egenskapen.

### 9. Hitta alla fel

Hitta alla fel i följande avsnitt kod.

```
.card
  background: blue;
  color: red;
```

<details>
  <summary>
    Hint
  </summary>
  Var är mina måsvingar?
</details>

```
.card {
  background: 10px;
  font: red;
}
```

<details>
  <summary>
    Hint
  </summary>
  Du tänkte på detta i övning 6.
</details>

```
#image {
  width: rgb(10, 30, 60),
  height: rgb(60, 10, 30),
  color: 10px;
}
```

<details>
  <summary>
    Hint
  </summary>
  Semikolon? Rgb?
</details>

### 10. Färger och färger, och färger, och mera färger

Med både HTML och CSS, skriv en mening med varje bokstav i en egen färg. Det är okej att återanvända färger. Du kan exempelvis skriva "Sverige" där färgerna på bokstäverna alternerar mellan blå och gul.

### 11. Understräck

Skapa en div med valfritt innehåll. Med CSS, lägg till ett sträck under elementet med valfri färg och storlek.

<details>
  <summary>
    Hint
  </summary>
  borders
</details>

## Bonus utmaningar: Tabeller

### 1.

Skapa en tabell med följande kolumner: namn, invånare och kontinent. Lägg till 2-5 rader med värden på olika länder (exempelvis England, 67 milj, Europa).

### 2.

Skapa följande tabell: ![https://i.gyazo.com/673201f786cec493b1d29652685c52d3.png](https://i.gyazo.com/673201f786cec493b1d29652685c52d3.png)

### 3.

Skapa följande tabell: ![https://i.gyazo.com/700e831d212ed697472a90c1172998a9.png](https://i.gyazo.com/700e831d212ed697472a90c1172998a9.png)

### 4.

Skapa följande tabell: ![https://i.gyazo.com/2560562758654b163b37f069c88094f4.png](https://i.gyazo.com/2560562758654b163b37f069c88094f4.png)

### 5.

Skapa följande tabell: ![https://i.gyazo.com/f6699b84d9d8e04c5839b21314361508.png](https://i.gyazo.com/f6699b84d9d8e04c5839b21314361508.png)

### 6.

Skapa följande tabell: ![https://i.gyazo.com/f61cec80650440009aa104173054f586.png](https://i.gyazo.com/f61cec80650440009aa104173054f586.png)
