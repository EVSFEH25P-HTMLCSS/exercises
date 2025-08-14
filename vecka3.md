# Övningar - Vecka 3

## Del 1: Responsive Design

### 1.

Skapa en enkel webbsida som ändrar layout vid olika skärmstorlekar.

1. Skapa en ny HTML-fil med grundläggande struktur (header, nav, main, sidebar, footer).
2. Lägg till följande HTML:
   ```html
   <!DOCTYPE html>
   <html lang="sv">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Responsive Layout</title>
       <link rel="stylesheet" href="style.css">
   </head>
   <body>
       <header>
           <h1>Min Responsiva Webbplats</h1>
       </header>
       <nav>
           <ul>
               <li><a href="#">Hem</a></li>
               <li><a href="#">Om oss</a></li>
               <li><a href="#">Tjänster</a></li>
               <li><a href="#">Kontakt</a></li>
           </ul>
       </nav>
       <div class="container">
           <main>
               <h2>Huvudinnehåll</h2>
               <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
           </main>
           <aside>
               <h3>Sidoinnehåll</h3>
               <p>Information som är sekundär för huvudinnehållet.</p>
           </aside>
       </div>
       <footer>
           <p>&copy; 2025 Min Responsiva Webbplats</p>
       </footer>
   </body>
   </html>
   ```

3. Skapa en CSS-fil med följande kod:
   ```css
   * {
     box-sizing: border-box;
     margin: 0;
     padding: 0;
   }

   body {
     font-family: Arial, sans-serif;
     line-height: 1.6;
   }

   header, nav, footer {
     background-color: #333;
     color: white;
     padding: 1rem;
     text-align: center;
   }

   nav ul {
     display: flex;
     justify-content: center;
     list-style: none;
   }

   nav li {
     margin: 0 10px;
   }

   nav a {
     color: white;
     text-decoration: none;
   }

   .container {
     display: flex;
     flex-direction: column;
     padding: 1rem;
   }

   main, aside {
     padding: 1rem;
     margin-bottom: 1rem;
   }

   main {
     background-color: #f4f4f4;
   }

   aside {
     background-color: #e4e4e4;
   }

   /* Media Queries */
   @media screen and (min-width: 768px) {
     .container {
       flex-direction: row;
     }

     main {
       flex: 2;
       margin-right: 1rem;
       margin-bottom: 0;
     }

     aside {
       flex: 1;
     }
   }

   @media screen and (max-width: 600px) {
     nav ul {
       flex-direction: column;
     }

     nav li {
       margin: 5px 0;
     }
   }
   ```

4. Öppna webbsidan i en webbläsare och ändra fönsterstorlek för att se hur layouten anpassas.
5. Experimentera med olika brytpunkter och layoutändringar.

### 2.

Skapa ett bildgalleri som anpassar sig efter skärmstorlek.

1. Skapa en ny HTML-fil:
   ```html
   <!DOCTYPE html>
   <html lang="sv">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Responsiv Bildgalleri</title>
       <link rel="stylesheet" href="gallery.css">
   </head>
   <body>
       <header>
           <h1>Fotogalleri</h1>
       </header>
       <div class="gallery">
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 1">
               <div class="caption">Bildtext 1</div>
           </div>
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 2">
               <div class="caption">Bildtext 2</div>
           </div>
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 3">
               <div class="caption">Bildtext 3</div>
           </div>
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 4">
               <div class="caption">Bildtext 4</div>
           </div>
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 5">
               <div class="caption">Bildtext 5</div>
           </div>
           <div class="gallery-item">
               <img src="https://via.placeholder.com/400x300" alt="Bild 6">
               <div class="caption">Bildtext 6</div>
           </div>
       </div>
   </body>
   </html>
   ```

2. Skapa en CSS-fil (gallery.css):
   ```css
   * {
     box-sizing: border-box;
     margin: 0;
     padding: 0;
   }

   body {
     font-family: Arial, sans-serif;
     line-height: 1.6;
   }

   header {
     background-color: #333;
     color: white;
     padding: 1rem;
     text-align: center;
     margin-bottom: 20px;
   }

   .gallery {
     display: grid;
     grid-template-columns: 1fr;
     gap: 20px;
     padding: 0 20px;
   }

   .gallery-item {
     box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
     transition: transform 0.3s ease;
   }

   .gallery-item:hover {
     transform: scale(1.03);
   }

   .gallery-item img {
     width: 100%;
     height: auto;
     display: block;
   }

   .caption {
     padding: 10px;
     text-align: center;
     background-color: #f4f4f4;
   }
   ```

3. Lägg till media queries för att visa flera bilder bredvid varandra (horisontellt) på större skärmar
4. Gör steg 3 men med flexbox istället

### 3.

Skapa en navigationsmeny som blir till en hamburgaremeny på mindre skärmar och visar alla menyval på större skärmar.

1. Skapa en ny HTML-fil:
   ```html
   <!DOCTYPE html>
   <html lang="sv">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Responsiv Navigation</title>
       <link rel="stylesheet" href="nav.css">
   </head>
   <body>
       <header>
           <div class="logo">LogoTyp</div>
           <input type="checkbox" id="nav-toggle" class="nav-toggle">
           <label for="nav-toggle" class="nav-toggle-label">
               <span></span>
           </label>
           <nav>
               <ul>
                   <li><a href="#">Hem</a></li>
                   <li><a href="#">Om oss</a></li>
                   <li><a href="#">Tjänster</a></li>
                   <li><a href="#">Portfölj</a></li>
                   <li><a href="#">Kontakt</a></li>
               </ul>
           </nav>
       </header>
       <main>
           <h1>Välkommen till vår webbplats</h1>
           <p>Detta är ett exempel på responsiv navigation.</p>
       </main>
   </body>
   </html>
   ```

2. Skapa en CSS-fil (nav.css):
   ```css
   * {
     margin: 0;
     padding: 0;
     box-sizing: border-box;
   }

   body {
     font-family: Arial, sans-serif;
   }

   header {
     background: #333;
     color: white;
     text-align: center;
     position: relative;
     padding: 1em;
   }

   .logo {
     font-weight: bold;
     font-size: 1.5em;
     margin-bottom: 1em;
   }

   nav {
     position: absolute;
     background: #333;
     width: 100%;
     left: 0;
     top: 100%;
     transform: scale(1, 0);
     transform-origin: top;
     transition: transform 0.3s ease;
   }

   nav ul {
     list-style: none;
     margin: 0;
     padding: 0;
   }

   nav li {
     margin-bottom: 1em;
     margin-top: 1em;
   }

   nav a {
     color: white;
     text-decoration: none;
     font-size: 1.2rem;
     opacity: 0;
     transition: opacity 0.15s ease;
   }

   nav a:hover {
     color: #ddd;
   }

   .nav-toggle {
     display: none;
   }

   .nav-toggle-label {
     position: absolute;
     top: 0;
     right: 0;
     margin-right: 1em;
     height: 100%;
     display: flex;
     align-items: center;
     cursor: pointer;
   }

   .nav-toggle-label span,
   .nav-toggle-label span::before,
   .nav-toggle-label span::after {
     display: block;
     background: white;
     height: 2px;
     width: 2em;
     position: relative;
   }

   .nav-toggle-label span::before,
   .nav-toggle-label span::after {
     content: "";
     position: absolute;
   }

   .nav-toggle-label span::before {
     bottom: 7px;
   }

   .nav-toggle-label span::after {
     top: 7px;
   }

   .nav-toggle:checked ~ nav {
     transform: scale(1, 1);
   }

   .nav-toggle:checked ~ nav a {
     opacity: 1;
     transition: opacity 0.25s ease 0.15s;
   }

   main {
     padding: 2em;
   }
   ```

3. Sidan består av en hamburger-menu för telefoner, lägg till en media query som visar alla menyval på större skärmar (utan en hamburger-menu)

### 4.

Skapa en layout med kort som ändrar från flera kolumner till en kolumn baserat på skärmstorlek.

1. Skapa en ny HTML-fil:
   ```html
   <!DOCTYPE html>
   <html lang="sv">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Responsiva Kort</title>
       <link rel="stylesheet" href="cards.css">
   </head>
   <body>
       <header>
           <h1>Våra Tjänster</h1>
       </header>
       <div class="card-container">
           <div class="card">
               <div class="card-icon">🚀</div>
               <h2>Webbdesign</h2>
               <p>Vi skapar snygga och funktionella webbplatser anpassade för dina behov.</p>
               <button>Läs mer</button>
           </div>
           <div class="card">
               <div class="card-icon">📱</div>
               <h2>App-utveckling</h2>
               <p>Professionell utveckling av mobilapplikationer för iOS och Android.</p>
               <button>Läs mer</button>
           </div>
           <div class="card">
               <div class="card-icon">📊</div>
               <h2>SEO-optimering</h2>
               <p>Vi hjälper din webbplats att synas högre upp i sökresultaten.</p>
               <button>Läs mer</button>
           </div>
           <div class="card">
               <div class="card-icon">🔒</div>
               <h2>IT-säkerhet</h2>
               <p>Skydda din verksamhet med våra säkerhetstjänster.</p>
               <button>Läs mer</button>
           </div>
       </div>
   </body>
   </html>
   ```

2. Skapa en CSS-fil (cards.css):
   ```css
   * {
     box-sizing: border-box;
     margin: 0;
     padding: 0;
   }

   body {
     font-family: Arial, sans-serif;
     line-height: 1.6;
     background-color: #f4f4f4;
   }

   header {
     background-color: #333;
     color: white;
     text-align: center;
     padding: 2rem;
     margin-bottom: 2rem;
   }

   .card-container {
     display: flex;
     justify-content: center;
     max-width: 1200px;
     margin: 0 auto;
     padding: 0 20px;
   }

   .card {
     background-color: white;
     border-radius: 5px;
     box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
     padding: 2rem;
     margin: 1rem;
     display: flex;
     flex-direction: column;
     align-items: center;
     text-align: center;
     transition: transform 0.3s ease;
   }

   .card:hover {
     transform: translateY(-10px);
   }

   .card-icon {
     font-size: 3rem;
     margin-bottom: 1rem;
   }

   .card h2 {
     margin-bottom: 1rem;
     color: #333;
   }

   .card p {
     margin-bottom: 1.5rem;
     color: #666;
   }

   button {
     background-color: #333;
     color: white;
     border: none;
     padding: 0.7rem 1.5rem;
     border-radius: 5px;
     cursor: pointer;
     transition: background-color 0.3s ease;
   }

   button:hover {
     background-color: #555;
   }
   ```

3. Gör så att korten är läsbara på mindre skärmar (lägg dem vertikalt)
4. Experimentera med olika flex-properties för att ändra beteendet.

### 5.

Implementera en webbsida med typografi som anpassar sig till olika skärmstorlekar.

1. Skapa en sida med rubriker (h1-h3), brödtext och citat
2. Använd relativa enheter (em, rem) för textstorlekar
3. Implementera CSS-variabler för att definiera en typografiskala
4. Använd media queries för att justera bas-fontstorleken vid olika skärmstorlekar
5. Justera radavstånd och textmellanrum för optimal läsbarhet på olika enheter
6. Implementera minst två brytpunkter för typografiska ändringar

**Tips:** Överväg att använda `clamp()` för responsiva fontstorlekar, t.ex. `font-size: clamp(1.5rem, 5vw, 3rem);`

### 6.

Skapa ett kontaktformulär som anpassar sig till olika skärmstorlekar.

1. Skapa ett kontaktformulär med namn, e-post, ämne, meddelande och skicka-knapp
2. På större skärmar ska formfälten organiseras i två kolumner
3. På mindre skärmar ska alla fält staplas vertikalt i en kolumn
4. Använd CSS Grid eller Flexbox för layouten
5. Säkerställ att alla formulärelement är tillräckligt stora för pekskärmsinmatning på mobiler
6. Implementera hover- och fokus-stilar för alla interaktiva element
7. Säkerställ tillräckligt mellanrum mellan elementen på alla skärmstorlekar

**Tips:** Använd `padding` relativt till viewport-bredden för responsivt utrymme, t.ex. `padding: 2vw;`
