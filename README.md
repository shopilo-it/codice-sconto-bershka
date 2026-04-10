# Codice sconto Bershka, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Bershka** da [shopilo.it](https://shopilo.it/negozi/bershka.com). Restituisce **coupon Bershka** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-bershka](https://shopilo-it.github.io/codice-sconto-bershka/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-bershka
cd codice-sconto-bershka
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Bershka",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto sulla collezione nuova",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/bershka.com"
  }
]
```

## Coupon Bershka disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto sulla collezione nuova | [shopilo.it](https://shopilo.it/negozi/bershka.com) |

Codici attivi: **[shopilo.it/negozi/bershka.com](https://shopilo.it/negozi/bershka.com)**

## Domande frequenti

### Come utilizzo un codice sconto Bershka?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/bershka.com), aggiungi i prodotti al carrello su Bershka e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Bershka?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Bershka piu recenti?
La pagina [shopilo.it/negozi/bershka.com](https://shopilo.it/negozi/bershka.com) viene aggiornata quotidianamente con i codici sconto Bershka, voucher Bershka e coupon promozionali Bershka piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Bershka

Bershka e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/bershka.com) trovi i migliori codici sconto Bershka, coupon Bershka verificati e voucher Bershka attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-bershka
```

```javascript
const { fetchCoupons } = require('codice-sconto-bershka');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
