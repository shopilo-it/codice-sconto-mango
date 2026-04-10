# Codice sconto Mango, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Mango** da [shopilo.it](https://shopilo.it/negozi/mango.com). Restituisce **coupon Mango** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-mango](https://shopilo-it.github.io/codice-sconto-mango/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-mango
cd codice-sconto-mango
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Mango",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su moda donna e uomo",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/mango.com"
  }
]
```

## Coupon Mango disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su moda donna e uomo | [shopilo.it](https://shopilo.it/negozi/mango.com) |

Codici attivi: **[shopilo.it/negozi/mango.com](https://shopilo.it/negozi/mango.com)**

## Domande frequenti

### Come utilizzo un codice sconto Mango?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/mango.com), aggiungi i prodotti al carrello su Mango e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Mango?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Mango piu recenti?
La pagina [shopilo.it/negozi/mango.com](https://shopilo.it/negozi/mango.com) viene aggiornata quotidianamente con i codici sconto Mango, voucher Mango e coupon promozionali Mango piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Mango

Mango e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/mango.com) trovi i migliori codici sconto Mango, coupon Mango verificati e voucher Mango attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-mango
```

```javascript
const { fetchCoupons } = require('codice-sconto-mango');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
