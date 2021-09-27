# Front end

### 2021-09-30

---

## Vad är front end?

--

### User interface (UI)

- Output
- Input

Note: Output: text, bilder, video. Input: knappar, textfält, reglage. GUI, TUI. Så brett/generellt att det är svårt att hänvisa till tydliga källor.

--

### Client side

![Smartphone](img/Smartphone_icon.png)
![Cloud](img/Cloud_icon.png) <!-- .element: class="fragment fade-left"  -->

Note: Klient - vanligt begrepp i tekniska sammanhang, utveckla. (Jag gjorde ikonerna i Figma på 10 minuter, testa om ni är intresserade!)

--

### Exempel

- Webbsida
- Mobilapp
- Smart högtalare

Note: Pratar nästan alltid om front end i webbsammanhang. Kanske mindre klyfta i andra discipliner? Tycker även att det kan vara forcerat ibland i webbsammanhang.

--

### Användarupplevelse

- Användaren alltid i fokus
- [Kan skapa en bra användarupplevelse, oavsett förutsättningar](https://uxdesign.cc/what-you-should-know-about-skeleton-screens-a820c45a571a)
- [Kan också förstöra allt](https://userinyerface.com/)
- Det nödvändiga, och [det lilla extra](https://www.joshwcomeau.com/animation/3d-button/)

Note: Front end/UX -> användare i första rummet. Ganska roligt, gör något åt sig själv. Välformulerade felmeddelanden, roliga laddningsindikatorer kan överbrygga problem.

---

## Webbutveckling

- Bygg en gång, använd (nästan) var som helst
- [World Wide Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works), [sen 1989](https://webfoundation.org/about/vision/history-of-the-web/)
- En [länk](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) bort ifrån en fullfjädrad användarupplevelse
- Enorm (utvecklar-)community [a11y](https://twitter.com/i/lists/1436358567456563202), [CSS](https://twitter.com/i/lists/1436357966400217090), [webbplattformen](https://twitter.com/i/lists/1436358858352611333)
- Sammantaget - väldigt roligt och inspirerande!

Note: Mobil, dator, smart TV, smart klocka, allt med en skärm och en webbläsare. Klicka in och läs under 'World Wide Web' innan nästa slide.

---

### HTML

> Inga problem, det vet jag hur man skriver!

..eller? <!-- .element: class="fragment fade-in"  -->

Note: Förväntas alltid, men lärs sällan ut. Förlåtande, webbläsarna jobbar med "silent failure". Inte _lika_ viktigt för personer med god kognitiv förmåga.

--

### [HTML](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)

- [Struktur](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html), information, och [inbyggd logik](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)
- Enkelt att lära sig, [svårt att bemästra](https://www.htmhell.dev/)

--

#### [HTML-Labb](https://codesandbox.io/s/how-to-html-nkbpo?file=/index.html)

--

### Innan vi lämnar labben

![Klicka "Fork" för att få en kopia av sandboxen](img/codesandbox_fork.PNG)

**Spara** fork-länken, eller skapa ett konto och spara den där, vi kommer tillbaka hit i kommande labbar!

--

#### HTML - Begränsningar

- [Svårt att återanvända](https://developer.mozilla.org/en-US/docs/Web/Web_Components/HTML_Imports)
- Svårt att få dynamiskt (on-the-fly databas-baserade val i en [Dropdown](https://www.carbondesignsystem.com/components/dropdown/usage/#live-demo) till exempel)

Note: Bekant med front end? Borde väl bara kunna importera en HTML-fil? Nope (se länk)

--

#### Nästa steg

- Förstå hur template-språk så som [JSX](https://reactjs.org/docs/introducing-jsx.html) (React), [HTML-templates](https://v3.vuejs.org/guide/template-syntax.html) (Vue) förhåller sig till HTML
- Förstå vikten av _semantisk_ HTML
- Förstå hur HTML förhåller sig till CSS och JavaScript (coming up!)

---

### [CSS](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)

![CSS](img/css.gif) <!-- .element: class="fragment fade-in"  -->

... fast så illa är det inte! <!-- .element: class="fragment fade-in"  -->

Note: Ökänt för att vara svårt att skala, vilket ofta bygger på dålig grundförståelse, lite som HTML, fast märks tydligare för alla

--

### CSS - Några exempel

1. [Plain HTML](https://motherfuckingwebsite.com/)
2. [HTML med CSS](http://bettermotherfuckingwebsite.com/) <!-- .element: class="fragment fade-in"  -->
3. [Inspiration!](https://www.joshwcomeau.com/) <!-- .element: class="fragment fade-in"  -->

--

### CSS - Blandade fakta

- Definierar hur HTML ska visualiseras
- Alla (moderna) webbläsare har [inbyggd default-CSS](https://motherfuckingwebsite.com/)
- [Globalt scope](https://codesandbox.io/s/affectionate-benz-wppjz?file=/index.html)
- [Cascading](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade)
- [Implicit](https://www.joshwcomeau.com/css/the-importance-of-learning-css/#it-improves-your-quality-of-life)

Note: Öppna DevTools.

--

### CSS - [Anatomi](https://courses.joshwcomeau.com/css-for-js/00-recap/02-anatomy) och begrepp

- Rule
- Property
- Selector
- Declaration
- Unit

--

### CSS - HTML-integration

- [inline-\<style\>](https://codesandbox.io/s/affectionate-benz-wppjz?file=/index.html)
- `<link>`, tryck F12!
- HTML-attributet "class" (men också andra properties)

--

### CSS - Labb

[Codesandbox - utgångspunkt](https://codesandbox.io/s/huckleberry-hk4jq?file=/index.html)

Beroende på ambitions-/kunskapsnivå:

1. Försök att efterlikna enskilda element
2. Gör något som liknar helheten
3. Gör en responsiv lösning som fungerar oavsett skärmstorlek

Note: Demonstrera [facit](https://courses.joshwcomeau.com/css-for-js/01-rendering-logic-1/15-flow-workshop) lokalt. [Min dugliga lösning](codesandbox.io/s/huckleberry-forked-6c3zl)

--

### CSS - Vanliga problem

- [Repetetivt](https://codesandbox.io/s/eager-drake-u85x5?file=/index.html). Motmedel: [Utility classes](https://adamwathan.me/css-utility-classes-and-separation-of-concerns/), komponenter (coming up!)
- [Specificitetskrig](https://css-tricks.com/a-specificity-battle/)

Note: Repetition förekommer alltid, optimera inte för tidigt

--

### CSS - Nästa steg

- Förstå hur [Sass](https://sass-lang.com/), [Styled components](https://styled-components.com/), [Tailwind](https://tailwindcss.com/) och andra CSS-relaterade bibliotek förhåller sig till CSS
- Förstå hur [BEM](http://getbem.com/), [CSS Modules](https://github.com/css-modules/css-modules) förenklar CSS genom att undvika specificitetskrig
- Förstå hur vi genom att nyttja snarare än programmera bort kaskaden kan skriva effektiv CSS, se [Every Layout](https://every-layout.dev/layouts/)

---

### JavaScript

- Ger [liv](https://www.joshwcomeau.com/react/animated-sparkles-in-react/) till statiska HTML-dokument
- Ett någorlunda konventionellt programmeringsspråk - det enda\* som webbläsare förstår
- [Hatat](https://dev.to/zimspy007/why-we-love-to-hate-javascript-nfd) och älskat
- Benämns ibland "VanillaJS"

_\* [sanning med modifikation](https://developer.mozilla.org/en-US/docs/WebAssembly)_

--

### JavaScript - Generella kodexempel

- const, let, var
- datatyper
- es6

Tips:

- [API-referens](https://developer.mozilla.org/en-US/)
- [Vettig kurs, scrolla till botten och hämta din "Free Preview"](https://justjavascript.com/)

--

### JavaScript - DOM-manipulation

- [document-API:et](https://developer.mozilla.org/en-US/docs/Web/API/Document)

Note: Öppna DevTools. `document.` (autocomplete) `location.hostname`. `document.getElementById('... vadå?'). Kolla Elements. ById.toString(). Kolla upp i MDN. Hidden. Byt innerText.

--

### JavaScript - [HTML-integration](https://codesandbox.io/s/link-html-and-javascript-6vj6b)

- Inline-script
- Referens till annan fil i samma projekt
- [Referens till tredjepartsfil på webben](https://reactjs.org/docs/cdn-links.html)
- [... men tänk till först](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/loading-third-party-javascript)

--

### JavaScript - Labb

(Anpassa till Jenny/Backend)

--

#### JavaScript - Node och npm

- [Node](https://nodejs.org/en/) - JavaScript utanför webbläsaren
- [npm](https://www.npmjs.com/package/react) - Portalen till återanvändning av miljontals JavaScript-paket, [se Jonathan berätta mer och ge exempel](https://web.microsoftstream.com/video/f406c765-a041-44fd-b41b-cb5a219d472c?st=924)

Note: Node - främst relevant för JavaScript i server-sammanhang. Men, också basen för npm som är vitalt för JavaScripts ekosystem

--

#### Nästa steg

- Grundlig förståelse för JavaScript
- [TypeScript](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
- Utforska ekosystemet

---

## Ramverk

- Abstraherar HTML/CSS/JavaScript
- [React](https://reactjs.org/docs/getting-started.html), [Vue](https://vuejs.org/), [Svelte](https://svelte.dev/), med flera.
- Skjuter ofta [mycket ansvar till JavaScript](https://codesandbox.io/s/practical-andras-97i1d?file=/public/index.html)

--

### React

- Används i de allra flesta av våra uppdrag idag
- Ett _bibliotek_ med mycket frihet, som ramverk så som [NextJS](https://nextjs.org/) och [Gatsby](https://www.gatsbyjs.com/) bygger på
- Skrivs oftast som _deklarativ_ [JSX](https://reactjs.org/docs/introducing-jsx.html)-kod
- Hjälper oss att skriva återanvändbar kod

Note: Mycket frihet = unopinionated. Bring your own... router, etc.

--

### React - Komponenter

- Små, isolerade, återanvändbara delar av webbapplikationer
- Inte unikt för React
- [Exempelkomponent](https://codesandbox.io/s/react-counter-functional-component-xge6o?file=/src/Counter.js)

Note: Komponenter kan vara väldigt simpla (knapp) eller väldigt komplexa (hela vyer). Gått från sidor till vyer. Kolla igenom exempelkomponent och prata lite om props.

--

### React - Viktiga koncept och begrepp

- [State](https://reactjs.org/docs/hooks-state.html)
- [Virtual DOM](https://javascript.plainenglish.io/react-the-virtual-dom-comprehensive-guide-acd19c5e327a)
- [Rendering](https://dev.to/teo_garcia/understanding-rendering-in-react-i5i)
- [Hooks](https://reactjs.org/docs/hooks-intro.html)

--

### React - Labb

React-template, återskapa funktionalitet från förra labben, jämför kod

---

## React, [SCSS](https://sass-lang.com/) och TypeScript till HTML, CSS och JavaScript

- [Bundler](https://webpack.js.org/concepts/why-webpack/) - buntar ihop många små filer till en stor.
- [Transpiler/Compiler](https://babeljs.io/repl/) - låter oss skriva kod som webbläsaren inte förstår
- [...kanske inte nödvändigt i en nära framtid](https://world.hey.com/dhh/modern-web-apps-without-javascript-bundling-or-transpiling-a20f2755)

Note: Bundler - Webpack. Transpiler - Babel/tsc

---

## Vanligt förekommande tooling

- Editor - [VS Code](https://code.visualstudio.com/)
- Linter - [ESLint](https://eslint.org/)
- Kodformatterare - [Prettier](https://prettier.io/)
- Versionshantering - [git](https://git-scm.com/)
- Pakethantering - npm, som kommer med [Node](https://nodejs.org/en/)

---

## Data och API:er

- JavaScripts [fetch-API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) används i moderna webbapplikationer, ibland genom bibliotek så som [Axios](https://github.com/axios/axios)
- Hämtar ofta data som [JSON](https://json.org/example.html) från [REST](https://restfulapi.net/)-API:er
- JSON [deserialiseras](https://developer.mozilla.org/en-US/docs/Glossary/Deserialization) sedan och används i applikationen

Note: fetch-API - red ut API-begreppet. Ofta pragmatiskt förhållningssätt till REST

--

## Data och API:er framöver

- Smartare front ends med t ex [react-query](https://react-query.tanstack.com/)
- [GraphQL](https://graphql.org/) som [några kollegor snackade om](https://web.microsoftstream.com/video/fcf4e3f4-316a-4156-8634-57e0b83c1619?referrer=https:%2F%2Fl.workplace.com%2F)
- [Streaming](https://www.youtube.com/watch?v=G9PpImUEeUA) - inte bara för video, fast länken går till en video..

---

## Hosting

Okomplicerat när det kommer till [statiska webbapplikationer](https://en.wikipedia.org/wiki/Static_web_page)

- Kolla in [Netlify](https://www.netlify.com/)/[Heroku](https://www.heroku.com/) eller dylika tjänster
- I typiska projekt: Ungefär samma sak, fast med den provider kunden nyttjar, t ex Azure

Note: Statisk webbapplikationer är de som har all dynamik på klient-sidan. Visa Netlify om tid. Kan ofta vara mer customization på typiska uppdrag - lära sig mer på DevOps-session.

---

## Tack för idag

Presentation gjord med [reveal.js](https://github.com/hakimel/reveal.js)
