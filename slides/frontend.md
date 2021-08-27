# Front end

### 2021-08-06

---

## Vad är front end?

--

### User interface (UI)

- Output (text, bilder, video)
- Input (knappar, textfält, reglage)

--

### Client side

![Smartphone](img/Smartphone_icon.png)
![Cloud](img/Cloud_icon.png) <!-- .element: class="fragment fade-left"  -->

--

### Exempel

- Webbsida
- Mobilapp
- Smart högtalare

--

### Användarupplevelse

- Användaren i fokus
- Det nödvändiga, och det lilla extra

---

## Webbutveckling

- Bygg en gång, använd var som helst
- www, since 1989
- En länk bort ifrån en fullfjädrad användarupplevelse
- Enorm utvecklar-community
- Sammtaget - Väldigt roligt!

--

### HTML

> Inga problem, det vet jag hur man skriver!

..eller? <!-- .element: class="fragment fade-in"  -->

--

#### HTML

- Struktur, information, och inbyggd logik
- Enkelt att lära sig, svårt att bemästra

--

#### Labb

[HTML playground](https://codesandbox.io/s/how-to-html-nkbpo?file=/index.html)

![Klicka "Fork" för att få en kopia av sandboxen](img/codesandbox_fork.PNG) <!-- .element: class="fragment fade-in"  -->

Spara fork-länken/skapa ett konto och spara den där, vi kommer tillbaka hit! <!-- .element: class="fragment fade-in"  -->

--

#### Begränsningar

- Svårt att återanvända
- Svårt att få dynamiskt (on-the-fly databas-baserade val i en Dropdown till exempel)

--

#### Nästa steg

- Förstå hur template-språk så som [JSX](https://reactjs.org/docs/introducing-jsx.html) (React), [HTML-templates](https://v3.vuejs.org/guide/template-syntax.html) (Vue) förhåller sig till HTML
- Förstå vikten av semantisk HTML
- Förstå hur HTML förhåller sig till CSS och JavaScript (coming up!)

--

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

Inspo: Josh CSS-kurs

- Rule
- Property
- etc.

--

#### HTML-integration

- Klasser! (men också andra properties)
- inline-\<style\>
- `<link>...`

--

#### Labb

Använd länken från HTML-labben

Olika nivåer, ~3 förslag så att något passar

--

#### Vanliga problem

- Repetetivt
- Specificitetskrig

#### Nästa steg

- Förstå hur [Sass](https://sass-lang.com/), [Styled components](https://styled-components.com/), [Tailwind](https://tailwindcss.com/) förhåller sig till CSS
- Förstå hur [BEM](http://getbem.com/), [CSS Modules](https://github.com/css-modules/css-modules) förenklar CSS genom att undvika specificitetskrig
- Förstå hur vi genom att nyttja snarare än programmera bort kaskaden kan skriva effektiv CSS, se [Every Layout](https://every-layout.dev/layouts/)

--

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

---

## React

- Används i de allra flesta uppdrag idag
- Ett bibliotek med mycket frihet, som ramverk så som NextJS och Gatsby bygger på
- Deklarativ JSX-kod
- Hur hjälper React oss att skriva återanvändbar kod?

---

#### Labb

React-(TypeScript?)-template, återskapa funktionalitet från tidigare labb, jämför kod

---

## React, SCSS och TypeScript till HTML, CSS och JavaScript

- Bundler
- Transpiler/Compiler

---

## Tooling

- Linter
- Kodformatterare

---

## Data och APIer

- JavaScripts fetch-API används i moderna webbapplikationer
- Hämtar ofta data som JSON från REST-APIer
- JSON behandlas sedan och används i applikationen
- Mycket spännande innovation så som react-query, RTK Query och swr
- GraphQL

---

## Hosting

---

## Made using

[reveal.js](https://github.com/hakimel/reveal.js)
