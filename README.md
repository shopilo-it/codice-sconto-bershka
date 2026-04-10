# Cod reducere Bershka — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Bershka** de pe [shopilo.it](https://shopilo.it/magazin/bershka.com). Returneaza **cupoane Bershka** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-bershka](https://shopilo-it.github.io/codice-sconto-bershka/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-bershka
cd codice-sconto-bershka
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Bershka",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto sulla collezione nuova",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/bershka.com"
  }
]
```

## Cupoane Bershka disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% di sconto sulla collezione nuova | [shopilo.it](https://shopilo.it/magazin/bershka.com) |

Codurile active: **[shopilo.it/magazin/bershka.com](https://shopilo.it/magazin/bershka.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Bershka?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/bershka.com), adauga produsele in cos pe Bershka, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Bershka?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Bershka?
Pagina [shopilo.it/magazin/bershka.com](https://shopilo.it/magazin/bershka.com) este actualizata zilnic cu cele mai noi cod reducere Bershka, voucher Bershka si cupon promotional Bershka.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Bershka

Bershka este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/bershka.com) cele mai bune cod reducere Bershka, cupoane Bershka verificate si voucher Bershka active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-bershka
```

```javascript
const { fetchCoupons } = require('codice-sconto-bershka');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
