# DomoMeter Landing Page

Landing page statica per **DomoMeter**, app mobile per monitorare i consumi domestici di luce, gas e acqua.

Il progetto è pensato per una pubblicazione semplice su **GitHub Pages**: non richiede build, dipendenze o framework lato app. Tutto vive in una singola pagina `index.html`, con **Tailwind CSS via CDN** e un minimo di **JavaScript vanilla** per tema e modale privacy.

## Demo

Landing page online:

`https://dimpemekug.github.io/domometer-landing/`

## Funzionalità

- Hero con branding DomoMeter e CTA per store mobile
- Doppio mockup 3D che mostra i due stili dell'app: moderno e retro
- Tema chiaro/scuro con salvataggio preferenza in `localStorage`
- Sezione feature in layout bento grid
- Slider recensioni in marquee continuo
- Sezioni legali e supporto in accordion
- Modale che carica il contenuto di [`PRIVACY_POLICY_IT.md`](./PRIVACY_POLICY_IT.md)
- Layout responsive, adatto a desktop e mobile

## Stack

- HTML5
- Tailwind CSS via CDN
- JavaScript vanilla
- Google Fonts

## Struttura

```text
.
├── index.html
├── icon.png
├── PRIVACY_POLICY_IT.md
└── README.md
```