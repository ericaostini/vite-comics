## Vite DC Comics 

Creazione sito clone pagina web DC Comics, dedicato alla vendita di fumetti, film, giochi, video, merchandise.
Utilizzo framework Vue.js.

![homepage](/src/assets/images/Screenshot%202024-01-31%20alle%2015.16.35.png)

### Fase 1
Creo nuovo progetto con Vite e Vue 
* Creo file in GitHub 'vite-comics'
* In vs code apro Terminal e digito 
    ```sm 
        npm create vite@latest
        Project name: .
        Framework: Vue
        variant: JavaScript
    ```
* Creati i file installo e controllo se tutto funziona con i comandi suggeriti 
    ```sm
        npm install
        npm run dev
    ```

* Su file .gitignore aggiungo file package-lock.json

Dopo di che svuoto file App.vue e file style.css

### Fase 2
Creo 3 componenti principali e li aggiungo alla cartella components:
1. HeaderComponent
2. MainComponent
3. FooterComponent
E li importo del mio file Vue principale 'App.vue'

Per ognuno personalizzo con html + scss 

### Fase 3
Per la sezione header creo file da importare in HeaderComponent che contiene la creazione della Navbar 
```sm
    NavBar.vue
```
Struttura nav bar da Bootstrap e ciclo for sui vari link della nav bar, aggiungendo classe active a link in cui active: true

Per la sezione del main con le icone, creo un quarto file da aggiungere alla cartella components e da importare nel mio componente MainComponents
```sm
    IconComponent.vue
```
Ciclo for su array images, per testo e url immagine 

Per componente FooterComponent
* Ciclo for per elenco informazioni su array object footerInfos (footer-top)
* imagine logo in position: relative e contenitore in overflow:hidden 
* Ciclo for su array icons per visualizzare le immagini relative ai social (footer-bottom)

### Fase 4 
Stistemo css per l'intera pagina
* Aggiunto font
* Sistemo colori
* Padding e margin 

## Fase 5 
Utilizzo file dc-comics.json per importare l'array delle card.
Creo componente nuova Card, che verrà interita al posto della scritta 
--Content goes here--

Passo il contenuto del file .json al componente Card con props 