## Instrumente - Google Gemini
## Cerințe cheie
- ### 1. Am întrebat: De ce serverul Vite nu pornea.
- Am primit: Mi s-a explicat că Vite a creat un subfolder nou, deci a trebuit să rulez `cd app` înainte de `npm run dev`.
- Modificat sau respins: Aplicat cu succes.

- ### 2. Am întrebat: Cum să rezolv eroarea "ReactDOMClient.createRoot()" din consolă.
- Am primit: Mi-a indicat faptul că am duplicat accidental blocul de inițializare React și am pus greșit importurile atunci când am copiat codul din laborator. 
- Modificat sau respins: Am curățat fișierul `main.jsx` și eroarea a dispărut.

## Ce am învățat / ce nu a funcționat
Rularea comenzii `npm run dev` în folderul principal nu a funcționat; am învățat că trebuie să navighez mai întâi în subfolderul Vite. De asemenea, am învățat că instrucțiunile `import` din JavaScript trebuie să fie plasate întotdeauna la începutul fișierului, iar `createRoot` din React trebuie apelat o singură dată pentru a evita erorile de randare.