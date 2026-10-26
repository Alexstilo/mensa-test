# Menù mensa — app GitHub Pages

Questa cartella contiene la versione italiana dell’app: mostra un solo giorno alla volta, navigazione tra settimane e giorni, ricerca alimenti, condivisione, suoni clic e link al PDF originale. Il PDF deve chiamarsi sempre **`menu.pdf`**.

## Come gestire il cambio stagione

La data del cambio non deve essere conosciuta in anticipo. Fino a quando la scuola non comunica la nuova data, lascia invariato il menu attivo e il relativo `menu-data.json`.

Quando arriva il nuovo menu:

1. Sostituisci il vecchio PDF con il nuovo file, mantenendo il nome `menu.pdf`.
2. Aggiorna `menu-data.json` con i nuovi piatti.
3. Imposta `season` su `estivo` o `invernale`.
4. Inserisci la data ufficiale in `startDate` e `weekAnchor` nel formato `AAAA-MM-GG`.
5. Pubblica i file aggiornati su GitHub Pages.

L’app continuerà a mostrare il menu precedente finché non aggiorni il JSON. Una volta impostata la data, prima di quel giorno mostrerà automaticamente “Menu non ancora attivo” e dal giorno indicato userà la nuova stagione.

## File da pubblicare insieme

- `menu_mensa_invernale.html` — pagina principale
- `menu-data.json` — dati e data di attivazione
- `menu.pdf` — PDF originale, con nome fisso
- `illustrazione-invernale.png` — banner grafico

Il caricamento del JSON e il collegamento al PDF sono relativi e funzionano su GitHub Pages.
