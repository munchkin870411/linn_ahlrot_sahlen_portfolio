# Linn Ahlrot Sahlén – portfolio

## Beskrivning och målgrupp

Det här är en responsiv portfolio-webbplats för Linn Ahlrot Sahlén, färdigutbildad frontendutvecklare som nu vidareutbildar sig inom backend. Projekten kommer från hennes publika GitHub-repositories och målgruppen är potentiella arbetsgivare, uppdragsgivare och andra som vill se hennes projekt och tekniska utveckling.

## Kravchecklista

- [x] Fyra HTML-vyer: Start, Projekt, Om mig och Kontakt.
- [x] Semantiska element: `header`, `nav`, `main`, `section`, `article` och `footer`.
- [x] Flexbox används bland annat i header, navigation, knapprader och footer.
- [x] CSS Grid används i hero-sektionen, projektlistan och värdekorten.
- [x] Mobil-först-styling med `min-width`-brytpunkter på 480 px, 640 px, 768 px och 1024 px, beroende på sida.
- [x] Responsiva, lokala projektbilder och porträtt med beskrivande alt-texter.
- [x] Tydlig rubrikhierarki, kontrasterande färger och anpassat radavstånd.
- [x] Synlig tangentbordsfokus och labels på alla formulärfält.
- [x] Kontaktformulär med namn, e-post och meddelande.
- [x] Logisk mappstruktur: `css/` och `assets/`, med gemensam `style.css` och separat CSS per sida.
- [x] Intern navigation och beskrivande länktexter utan döda länkar.
- [x] Tre riktiga projekt från GitHub med länkar till repositories och publicerad demo där det finns: ETA Skåne, Munchkin Travel App och AtYourPace.
- [x] Personlig logotyp med aliaset Munchkin och Linns namn.
- [x] Alla fyra HTML-sidor validerade med Nu HTML Checker: 0 errors.
- [x] Alla fem CSS-filer validerade med CSS Validator: 0 errors. Validatorns varningar om CSS-variabler förklaras nedan.

## Kör lokalt

Öppna `index.html` direkt i en webbläsare, eller starta en lokal server i projektmappen:

```text
python -m http.server 8000
```

Besök sedan `http://localhost:8000` i webbläsaren. Kontaktformuläret öppnar användarens lokala e-postprogram eftersom projektet inte har någon backend.

## Validering

Alla HTML- och CSS-filer har kontrollerats med [W3C Nu HTML Checker](https://validator.w3.org/nu/) respektive [W3C CSS Validator](https://jigsaw.w3.org/css-validator/). Resultat: 0 errors.

Förväntade varningar som kan ignoreras:

- `style.css` innehåller `@import url('https://fonts.googleapis.com/...')` för att hämta Google Fonts. Validatorn meddelar att importerade formatmallar inte granskas vid uppladdning eller direkt inmatning; det är en begränsning i hur validatorn hanterar externa importer, inte ett fel i koden. Typsnitten har systemfallbacks om importen skulle misslyckas.
- CSS-validatorn visar meddelandet "Due to their dynamic nature, CSS variables are currently not statically checked" för rader som använder CSS-variabler (t.ex. `var(--line)`, `var(--paper)`, `var(--green)`). Det är en generell begränsning i validatorn, inte ett fel i koden, och meddelandet kan förekomma i samtliga stilmallar (`style.css`, `home.css`, `projects.css`, `about.css`, `contact.css`) eftersom de alla använder CSS-variabler.

## Kända brister / att-göra

- Kontaktformuläret behöver en backend eller formulärtjänst för att skicka meddelanden utan ett lokalt e-postprogram.
- Projektbilderna består av en lokal bild från ETA Skåne, en egen SVG-illustration av Travel Appens landsökning och AtYourPace-appens logotyp. Egna skärmdumpar från applikationernas gränssnitt kan läggas till senare.
- Nästa steg är att publicera webbplatsen på exempelvis Netlify.
