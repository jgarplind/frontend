# Front end

### 2021-08-06

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

### CSS

![CSS](img/css.gif) <!-- .element: class="fragment fade-in"  -->

... fast så illa är det inte! <!-- .element: class="fragment fade-in"  -->

--

#### Några exempel

1. [Plain HTML](https://motherfuckingwebsite.com/)
2. [HTML med CSS](http://bettermotherfuckingwebsite.com/) <!-- .element: class="fragment fade-in"  -->
3. [Inspiration!](https://www.joshwcomeau.com/) <!-- .element: class="fragment fade-in"  -->

--

#### Hårda fakta

- Alla moderna webbläsare har inbyggd default-CSS
- Definierar hur HTML ska visualiseras
- Globalt scope
- Cascading
- _Implicit_

--

#### Anatomi och begrepp

- Rule
- Property
- Selector
- Declaration
- Unit

--

#### HTML-integration

- inline-\<style\>
- `<link>...`
- Klasser! (men också andra properties)

--

#### Labb

Använd länken från HTML-labben

Olika nivåer, ~3 förslag så att något passar

--

#### Vanliga problem

- Repetetivt
- Specificitetskrig

--

#### Nästa steg

- Förstå hur [Sass](https://sass-lang.com/), [Styled components](https://styled-components.com/), [Tailwind](https://tailwindcss.com/) förhåller sig till CSS
- Förstå hur [BEM](http://getbem.com/), [CSS Modules](https://github.com/css-modules/css-modules) förenklar CSS genom att undvika specificitetskrig
- Förstå hur vi genom att nyttja snarare än programmera bort kaskaden kan skriva effektiv CSS, se [Every Layout](https://every-layout.dev/layouts/)

---

### JavaScript

- Ger liv till våra statiska dokument
- Ett någorlunda konventionellt programmeringsspråk - det enda som webbläsare förstår
- Hatat och älskat
- "Vanilla"-JS

--

#### Generella kodexempel

- const, let, var
- datatyper

--

#### DOM-manipulation

- document-API:et

--

#### HTML-integration

- Inline-script
- Referens till annan fil
- Referens till fil på webben

--

#### Labb

Mini-labb i sandbox: textfält + knapp lägger till nytt select-option

--

#### Node och npm

- Node - JavaScript utanför webbläsaren
- npm - Portalen till återanvändning av miljontals JavaScript-paket

--

#### Nästa steg

- Grundlig förståelse för "Vanilla" JS
- TypeScript
- Utforska ekosystemet

---

## Ramverk

- Abstraherar HTML/CSS/JavaScript
- React, Vue, Svelte, etc.
- Skjuter ofta mycket ansvar till JavaScript

--

### React

- Används i de allra flesta uppdrag idag
- Ett bibliotek med mycket frihet, som ramverk så som NextJS och Gatsby bygger på
- Deklarativ JSX-kod
- Hur hjälper React oss att skriva återanvändbar kod?

--

### Komponenter

- Används i de allra flesta uppdrag idag
- Ett bibliotek med mycket frihet, som ramverk så som NextJS och Gatsby bygger på
- Deklarativ JSX-kod
- Hur hjälper React oss att skriva återanvändbar kod?

--

### React - Viktiga koncept och begrepp

- Rendering
- Virtual DOM
- Hooks
- JSX

--

#### Labb

React-template, återskapa funktionalitet från tidigare labb, jämför kod

---

## React, SCSS och TypeScript till HTML, CSS och JavaScript

- Bundler
- Transpiler/Compiler

---

## Tooling

- Linter
- Kodformatterare
- Versionshantering

---

## Data och APIer

- JavaScripts fetch-API används i moderna webbapplikationer
- Hämtar ofta data som JSON från REST-APIer
- JSON deserialiseras sedan och används i applikationen
- Mycket spännande innovation så som react-query, RTK Query och swr
- GraphQL
- Streaming - inte bara för film!

---

## Hosting

Busenkelt när det kommer till statiska webbapplikationer

- Enklast: Öppna en HTML-fil du har lokalt i din webbläsare
- Nästan lika enkelt: Kolla in Netlify/Heroku eller dylik tjänst
- I typiska projekt: Ungefär som #2, fast med den provider kunden nyttjar, t ex Azure DevOps

---

## Made using

[reveal.js](https://github.com/hakimel/reveal.js)
