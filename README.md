# Il tuo nome è un peptide

App divulgativa per la Notte Europea dei Ricercatori: ogni lettera del nome diventa un amminoacido,
e l'app mostra la massa del peptide e uno spettro di massa MS/MS simulato.

## Come pubblicarla con GitHub Pages

1. Accedi a github.com (o crea un account gratuito).
2. In alto a destra: **+**, poi **New repository**. Nome: `peptide`. Lascia **Public**. Premi **Create repository**.
3. Nella pagina che si apre clicca **uploading an existing file** e trascina dentro tutti i file di questa cartella. Poi **Commit changes**.
4. Vai in **Settings**, poi **Pages** nella colonna a sinistra. In *Build and deployment*, *Source*: **Deploy from a branch**; *Branch*: **main** e cartella **/ (root)**. Premi **Save**.
5. Dopo uno o due minuti l'app è online all'indirizzo `https://tuonomeutente.github.io/peptide/`.

Aperta da quell'indirizzo, l'app mostra da sola il codice QR da far inquadrare ai visitatori,
e dal telefono si può installare con *Aggiungi a schermata Home*.

## File

- `index.html`: l'app completa
- `manifest.webmanifest`, `sw.js`, `icona-*.png`: servono per installarla come app e usarla senza rete
- `qrcode.js`: generatore di codici QR (Kazuhiko Arase, licenza MIT)

Masse monoisotopiche calcolate dalle formule degli amminoacidi; frammenti b e y a carica singola.
Le intensità dei picchi sono simulate.
