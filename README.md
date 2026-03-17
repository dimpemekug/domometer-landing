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

## Avvio locale

Per una preview veloce puoi aprire `index.html` nel browser, ma la modale privacy usa `fetch()` per leggere il file markdown. Per evitare problemi di CORS o caricamento locale, è meglio usare un piccolo server statico.

Esempi:

```bash
python3 -m http.server 8000
```

Poi apri:

`http://localhost:8000`

## Deploy su GitHub Pages

1. Pubblica la repository su GitHub.
2. Vai in `Settings > Pages`.
3. In `Build and deployment`, seleziona `Deploy from a branch`.
4. Scegli il branch principale e la cartella `/ (root)`.
5. Salva e attendi la pubblicazione.

L'URL finale sarà simile a:

`https://dimpemekug.github.io/domometer-landing/`

## Personalizzazione rapida

- Sostituisci i link `href="#"` dei pulsanti App Store e Google Play in [`index.html`](./index.html)
- Aggiorna email di supporto, testi marketing e recensioni demo
- Mantieni [`PRIVACY_POLICY_IT.md`](./PRIVACY_POLICY_IT.md) nella stessa cartella di [`index.html`](./index.html), altrimenti la modale non riuscirà a caricarlo
- Se cambi nome o formato dell'icona, aggiorna il riferimento a `icon.png` nel `<head>` e nella hero

## Note

- Il progetto non usa bundler o pipeline di build
- Tailwind viene caricato da CDN, quindi serve connessione internet per lo styling
- I contenuti presenti nei mockup e nelle recensioni sono demo visive della landing page
