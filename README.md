# creminem94.github.io

Il mio portfolio personale: siti, web app e piccoli strumenti che ho sviluppato.

**Online su:** [creminem94.github.io](https://creminem94.github.io)

## Struttura

```
index.html   l'intera pagina (HTML, CSS e un po' di JavaScript, senza framework)
img/         screenshot dei progetti
.nojekyll    dice a GitHub Pages di pubblicare i file così come sono
```

Non c'è nessun passaggio di build: il file `index.html` è già la pagina finale.

## Pubblicazione

Il sito è servito da GitHub Pages. Ogni push sul branch `main` lo aggiorna in automatico, di solito entro un paio di minuti.

Impostazione richiesta, una volta sola: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, cartella `/ (root)`.

## Aggiornare la pagina

- **Testi e progetti:** ogni progetto è un blocco `<article class="project">` in `index.html`. Per aggiungerne uno, copia un blocco esistente e cambia testi, tag e link.
- **Immagini:** salva lo screenshot in `img/` (circa 1440×900 per i siti, formato verticale per le app da telefono) e sostituisci il riquadro `<div class="shot">…</div>` del progetto con un `<img class="full" src="img/nome-file.jpg" alt="…">`.
- **Anteprima in locale:** apri `index.html` nel browser, oppure avvia un piccolo server con `npx serve .`.

## Dominio personalizzato (facoltativo)

1. Compra il dominio da un registrar.
2. In **Settings → Pages → Custom domain** inserisci il dominio: GitHub crea il file `CNAME` nel repository.
3. Nel pannello DNS del registrar aggiungi i record indicati nella [guida di GitHub](https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site).
4. Quando disponibile, attiva **Enforce HTTPS**.
