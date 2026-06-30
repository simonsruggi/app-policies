# app-policies

## Scopo

Repository centralizzato di documenti legali e di marketing per le app iOS (e relative versioni Android/web). Raccoglie **Privacy Policy**, **Terms of Use**, **Support** e pagine **Marketing** in formato Markdown, una sottocartella per app. Serve a fornire gli URL pubblici richiesti da App Store Connect / Google Play (privacy policy, supporto, termini) senza dover ospitare un sito per ogni app.

## Stack / hosting

- **Solo Markdown**, nessun codice/build. Niente config, niente dipendenze.
- Pubblicato via **GitHub Pages** (repo `simonsruggi/app-policies`, branch `main`). I commit storici includono "Trigger GitHub Pages deploy": push su `main` = deploy. URL pubblici nella forma `https://simonsruggi.github.io/app-policies/<app>/<FILE>` (o dominio Pages configurato).
- `README.md` in root funge da indice con i link alle pagine principali.

## Struttura cartelle

```
app-policies/
├── README.md              # Indice con link alle policy principali
├── PROJECT.md             # Questo file
├── esamenautica/          # Esame Patente Nautica (IT)
│   ├── PRIVACY.md
│   └── MARKETING.md
├── farmastock/            # FarmaStock — inventario farmaci (EN), iOS+Android+web
│   ├── PRIVACY.md         # include disclosure backend: Supabase/UPCitemdb/OpenFoodFacts/Anthropic
│   ├── TERMS.md           # termini + subscription + riferimento sito farmastock.app
│   └── MARKETING.md
├── phototrim/             # PhotoTrim — compressione foto/storage (EN)
│   ├── PRIVACY.md
│   └── MARKETING.md
├── pokerodds/             # PokerOdds (EN)
│   ├── PRIVACY.md
│   └── MARKETING.md
├── pureanalytics/         # PureAnalytics — web analytics (EN)
│   ├── PRIVACY.md
│   └── MARKETING.md
├── scirocco/              # Scirocco — navigazione marina (EN)
│   ├── PRIVACY.md         # include disclosure map tiles OSM/OpenSeaMap
│   └── MARKETING.md
├── stasera/               # Che facciamo stasera? (IT) — set più completo
│   ├── PRIVACY.md
│   ├── TERMS.md
│   ├── SUPPORT.md
│   └── MARKETING.md
└── zenflip/               # ZenFlip (EN)
    ├── PRIVACY.md
    └── MARKETING.md
```

## Tipi di documento

- **PRIVACY.md** — privacy policy (tutte le app la hanno). Le app "offline-first" dichiarano nessuna raccolta dati; quelle con backend (FarmaStock, Scirocco, PureAnalytics) dichiarano i servizi terzi usati.
- **TERMS.md** — termini d'uso (solo `farmastock`, `stasera`): include clausole subscription, IP, termination.
- **SUPPORT.md** — pagina supporto con email + FAQ (solo `stasera`).
- **MARKETING.md** — copy promozionale / feature list (tutte le app).

## Convenzioni

- Lingua per app: `esamenautica` e `stasera` in **italiano**; le altre in **inglese**.
- Ogni documento ha un header con titolo `# <Tipo> — <Nome App>` e una data "Last updated / Ultimo aggiornamento".
- Email di contatto: `simone.ruggiero97@gmail.com`.

## Workflow / deploy

1. Aggiungere/modificare il `.md` nella cartella dell'app.
2. Aggiornare `README.md` se serve un nuovo link in indice.
3. Commit + push su `main` → GitHub Pages pubblica automaticamente.

Nessun comando di build. Per testare un link basta aprire l'URL GitHub Pages corrispondente.

## Note

- Quando si aggiunge una nuova app iOS, creare la cartella con almeno `PRIVACY.md` (URL richiesto da App Store Connect) e idealmente `MARKETING.md`.
- Se un'app introduce un backend o servizi terzi nuovi, aggiornare la relativa `PRIVACY.md` (vedi pattern FarmaStock/Scirocco).
