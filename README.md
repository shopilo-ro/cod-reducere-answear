# Cod reducere Answear — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Answear** de pe [shopilo.ro](https://shopilo.ro/magazin/answear.ro). Returneaza **cupoane Answear** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-answear](https://shopilo-ro.github.io/cod-reducere-answear/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-answear
cd cod-reducere-answear
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Answear",
    "code": "SHOPILO25",
    "discount": "25%",
    "description": "25% reducere la produse cu pret intreg",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/answear.ro"
  }
]
```

## Cupoane Answear disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 25% | 25% reducere la produse cu pret intreg | [shopilo.ro](https://shopilo.ro/magazin/answear.ro) |

Codurile active: **[shopilo.ro/magazin/answear.ro](https://shopilo.ro/magazin/answear.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Answear?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/answear.ro), adauga produsele in cos pe Answear, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Answear?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Answear?
Pagina [shopilo.ro/magazin/answear.ro](https://shopilo.ro/magazin/answear.ro) este actualizata zilnic cu cele mai noi cod reducere Answear, voucher Answear si cupon promotional Answear.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Answear

Answear este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/answear.ro) cele mai bune cod reducere Answear, cupoane Answear verificate si voucher Answear active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-answear
```

```javascript
const { fetchCoupons } = require('cod-reducere-answear');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
