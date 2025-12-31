# Personal Website – Fabrizio De Masi

Portfolio personale statico realizzato in **HTML + SCSS + Bootstrap 5**, pubblicato tramite **GitHub Pages**.

Il sito racconta il mio percorso dalla tecnologia alla **Medicina Cinese**, presenta il mio **CV tecnico** e offre una pagina di **contatto**.

---

## 🔗 Live Demo

> **URL:** `https://fabrypostrock.github.io/`  


---

## 📄 Pagine principali

Il progetto è composto da **tre pagine**:

### 1. `index.html` – About me

Pagina principale, con:

- **Navbar fissa** in alto con:
  - Logo circolare
  - Nome: *Fabrizio De Masi*
  - Link a: `About me`, `Contatti`, `CV`
  - Versione mobile con **offcanvas menu** Bootstrap
- **Hero section**:
  - Titolo principale (`<h1>`) animato con effetti CSS/SCSS
  - Immagine centrale con animazione (slide / rotateY)
- **Racconto personale**: infanzia, studi in ingegneria elettronica, esperienza Erasmus, transizione dal mondo industriale al **Machine Learning / Data Science**, incontro con la **Medicina Cinese** e nascita del progetto **KurAI**
- **Immagini di contesto**:
  - Foto personali (Erasmus, famiglia, progetto con il co-founder)
- **Divider decorativi**:
  - Sezioni separate da poligoni creati con `clip-path` e mixin SCSS
  - Palette colori personalizzata: `#241d18` (scuro) e `#e26a08` (arancione)

---

### 2. `cv.html` – CV & Skills

Pagina dedicata al profilo professionale e alle competenze tecniche:

- **Years of Experience**
  - Titolo con icona `trophy` (Material Symbols)
  - Conteggio anni di esperienza totale (es. **12 Years**)
- **Languages Experience** (hard skills tecniche)
  - Serie di coppie **[skill, percentuale]**
  - Ogni skill è rappresentata da una **progress bar Bootstrap** personalizzata (altezza ridotta, colore arancione, animazione della larghezza)
- **Professional Experience** (Timeline sinistra)
  Timeline verticale con anni e descrizione dettagliata:
  - **2023 – Oggi – Cofounder KurAI**
  - **2021 – 2025 – Innovation Engineer (GEFRAN)**
  - **2011 – 2021 – Sviluppo Software PLC / Visual Basic**
- **Qualification & Education** (Timeline destra)

---

### 3. `contacts.html` – Contatti

Pagina per entrare in contatto in modo strutturato:

- **Navbar** coerente con le altre pagine
- **Form di contatto** con:
  - Campo **Email** (`type="email"` con `required` e messaggi di help/validation)
  - **Motivo del contatto** (`select`) con opzioni:
    - Proposta di collaborazione
    - Proposta di lavoro in P.IVA
    - Caffè virtuale
    - Altro
  - **Textarea** per descrivere la richiesta
  - Pulsante `Invia`
- **Divider grafici** (poligoni scuri/orange) che mantengono la coerenza estetica con il resto del sito

---

## 🧱 Tecnologie utilizzate

- **HTML5**
- **SCSS (Sass)** per:
  - Mixin riutilizzabili (animazioni, divider poligonali, progress bar)
  - Gestione variabili di colore e spaziature
- **Bootstrap 5.3 (via CDN)** per:
  - Grid system responsive
  - Navbar, offcanvas, button styles, progress bar
- **Google Fonts**:
  - `Nunito` per la tipografia principale
- **Google Material Symbols**:
  - Icone come `trophy`, `work`, `school`, `mail`, `call`
- **IcoMoon**:
  - Icone social personalizzate (Instagram, Facebook, LinkedIn, GitHub)

---

## 📁 Struttura del progetto (semplificata)

```text
.
├── index.html          # Pagina "About me"
├── cv.html             # Pagina CV & Skills
├── contacts.html       # Pagina Contatti
├── assets/
│   ├── css/
│   │   └── scss/
│   │       └── main.css      # CSS compilato da SCSS
│   ├── fonts/
│   │   ├── fonts.css         # Font IcoMoon
│   │   └── icomoon.*         # File font (ttf, woff, ecc.)
│   └── img/
│       ├── logo_fabri.png
│       ├── intro_photo.jpg
│       ├── opole1.JPG
│       ├── opole2.JPG
│       ├── opole-auschwitz.JPG
│       ├── son-skiing.png
│       ├── my-son.jpg
│       └── fabri-tommi.png
└── README.md
