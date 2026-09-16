# Emporio del Falegname F.lli Scandura — sito web

Sito statico multipagina (HTML/CSS/JS puro, nessuna build necessaria), ispirato nella struttura a falegnamerialamoderna.it: home, pagina "chi siamo", una pagina per ogni reparto prodotto e una pagina contatti con mappa.

## Struttura
```
index.html            Home
chi-siamo.html         Storia e valori
contatti.html          Indirizzo, telefono, email, social, mappa
prodotti/
  index.html            Hub con i 5 reparti
  ferramenta.html
  utensili.html
  fissanti.html
  sigillanti.html
  legname.html
css/style.css
js/main.js
```

## Come pubblicarlo su una nuova repository GitHub

1. Vai su [github.com/new](https://github.com/new) e crea una nuova repository (es. `emporio-falegname`), senza README.
2. Sul tuo computer, apri il terminale nella cartella di questo progetto ed esegui:
   ```bash
   git init
   git add .
   git commit -m "Primo commit: nuovo sito Emporio del Falegname"
   git branch -M main
   git remote add origin https://github.com/TUO-UTENTE/emporio-falegname.git
   git push -u origin main
   ```
3. Su GitHub, vai in **Settings → Pages**, imposta come sorgente il branch `main` e la cartella `/ (root)`.
4. Dopo qualche minuto il sito sarà online su `https://TUO-UTENTE.github.io/emporio-falegname/`.

## Da personalizzare
- Sezione "Progetti realizzati" in home: sostituisci i riquadri segnaposto con le foto reali dei lavori.
- Le illustrazioni sono disegni (SVG), non foto reali del negozio: se hai foto del punto vendita o dei prodotti, sostituiscile ai riquadri `.block-figure` e `.detail-art` in ogni pagina.
- Orari di apertura: non li ho inseriti perché non mi sono stati forniti. Aggiungili nella pagina `contatti.html` (c'è già lo stile `.orari-table` pronto in `css/style.css`).
- Collega un dominio personalizzato da Settings → Pages se vuoi usare www.emporiodelfalegname.it.
