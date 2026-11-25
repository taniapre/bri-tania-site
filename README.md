# BriTania – sito statico

Copia fedele di [bri-tania.com](https://bri-tania.com/) in HTML/CSS/JS, pronta per GitHub Pages.

- Italiano: `index.html`
- English: `en/index.html` (switch IT | EN in alto a destra)

## Anteprima locale

Apri `index.html` nel browser, oppure dalla cartella:

```powershell
cd "$env:USERPROFILE\Desktop\britania-site"
python -m http.server 8080
```

Poi vai su `http://localhost:8080`.

## Form contatti

Il form usa [FormSubmit](https://formsubmit.co/) e invia a `taniaprestini@gmail.com`.

1. Dal sito online (o in anteprima) invia un messaggio di prova.
2. Alla **prima** richiesta, FormSubmit manda a Tania un’email di attivazione: deve cliccare Conferma.
3. Da quel momento i messaggi arrivano in Gmail.

Niente hosting PHP, niente WordPress.

## Cosa è stato lasciato fuori di proposito

- Il titolo spurio “Elementor #91” del sito WordPress (bug di layout, non branding).
- Sezioni duplicate generate da Elementor (nel nuovo sito ogni blocco c’è una sola volta).

## Pubblicazione su GitHub Pages

1. Crea un repo (es. `britania-site`).
2. Carica il contenuto di questa cartella (puoi omettere `_source-home.html` e i CSS Elementor in `assets/post-*.css`).
3. In Settings → Pages: branch `main` / root.
4. Punta `bri-tania.com` dai DNS Register (record A/CNAME per `@` e `www` verso GitHub), **senza toccare** i record della PEC.
