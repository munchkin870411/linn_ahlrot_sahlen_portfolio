# Linn Ahlrot Sahlén – portfolio

## Beskrivning och målgrupp

Responsiv portfolio-webbplats för Linn Ahlrot Sahlén, färdigutbildad frontendutvecklare som nu vidareutbildar sig inom backend. Målgruppen är potentiella arbetsgivare och uppdragsgivare som vill se hennes projekt.

## Kravchecklista

- [x] Fyra sidor: Start, Projekt, Om mig och Kontakt.
- [x] Semantisk HTML: `header`, `nav`, `main`, `section`, `article`, `footer`.
- [x] Flexbox: hero på startsidan (`.hero`), header och navigation (`.header-bar`, `.site-nav`), knapprader och footer.
- [x] CSS Grid: projektkort (`.project-preview-grid`), värdekort (`.values-grid`), projektsidan (`.project-detail`) och kontaktsidan (`.contact-layout`).
- [x] Mobil först med två brytpunkter, 640 px och 1024 px (hamburgermeny under 1024 px).
- [x] Responsiva bilder med alt-texter.
- [x] Rubrikhierarki (h1–h3), radavstånd och färger med god kontrast.
- [x] Tillgänglighet: synlig tangentbordsfokus, labels på alla formulärfält, beskrivande länkar.
- [x] Kontaktformulär (namn, e-post, meddelande).
- [x] Mappstruktur: `css/` och `assets/`.
- [x] Validerad med W3C: 0 errors i alla HTML- och CSS-filer.

## Kör lokalt

Öppna `index.html` i en webbläsare. Kontaktformuläret öppnar användarens e-postprogram eftersom projektet saknar backend.

## Validering

Alla filer är kontrollerade med [W3C Nu HTML Checker](https://validator.w3.org/nu/) och [W3C CSS Validator](https://jigsaw.w3.org/css-validator/): 0 errors. Följande meddelanden kan ignoreras:

- **`@import` i `style.css`** (Google Fonts): validatorn granskar inte importerade stilmallar. Det är en begränsning i verktyget, inte ett fel i koden.
- **"CSS variables are currently not statically checked"**: validatorn kan inte kontrollera `var(--...)` i förväg. Meddelandet förekommer i alla stilmallar eftersom de använder CSS-variabler.

## Kända brister

- Kontaktformuläret skickar via `mailto:` och behöver en formulärtjänst för att fungera utan e-postprogram.
- Webbplatsen är inte publicerad ännu (t.ex. på Netlify).
