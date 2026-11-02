## Instrumente - Google Gemini
https://share.gemini.google/YvfsDubcC6Bf
## Cerințe cheie
- ### 1. Am întrebat: De ce pagina era goală și cum să procedez având două fișiere `index.html`.
- Am primit: AI-ul a explicat diferența dintre vechiul site static din HTML și noua structură Vite, clarificând faptul că React are nevoie doar de `<div id="root">` ca punct de pornire.
- Modificat sau respins: Am păstrat `index.html`-ul de la Vite și am păstrat vechea mea structură statică de HTML in afara folderului api, alegând să construiesc toată interfața direct din componente React, așa cum cere laboratorul.

- ### 2. Am întrebat: De ce lista de destinații nu se actualiza pe ecran când dădeam click pe butonul "Marchează vizitat".
- Am primit: Mi-a reamintit că în React nu pot modifica array-ul de date direct și că trebuie să mut lista într-un hook `useState` în `App.jsx` pentru a forța pagina să se redeseneze la click.
- Modificat sau respins: Am implementat funcția `handleToggle` folosind `useState`, dar am scris logica de actualizare a stării singură, integrând funcțiile utilitare (`marcheazaVizitat`) pe care le aveam deja făcute din laboratorul trecut.

## Ce am învățat / ce nu a funcționat
Inițial am încercat să copiez tot vechiul meu fișier HTML (cu `<header>`, `<main>`) direct în proiectul Vite, ceea ce nu a funcționat și a stricat afișarea paginii. Am învățat că în React structura DOM-ului se construiește dinamic prin componente (JSX), nu prin etichete statice. De asemenea, am înțeles că transmiterea funcțiilor ca parametri (props, precum `onToggle` sau `onDelete`) este singurul mod prin care un copil (cardul destinației) poate "comunica" cu părintele (`App.jsx`) pentru a modifica starea globală a aplicației.