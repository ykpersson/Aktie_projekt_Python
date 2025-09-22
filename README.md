# Aktie_projekt_Python

Ett modulärt, loggningsbart och testat Python-projekt för att hämta och exportera nyckeltal från årsredovisningar för samtliga aktier i OMX30 – inklusive A-, B- och C-aktier.

## Funktioner

- ✅ Hämtar nyckeltal via årsdata från yfinance
- ✅ Loopar igenom samtliga tickers i OMX30
- ✅ Loggar varje steg och fel via central logger
- ✅ Exporterar till CSV för vidare analys i Power BI
- ✅ Testbar via `pytest` eller `unittest`
- ✅ Kodstil enligt PEP8, verifierad med `pylint`

## Mappstruktur

omx30_analys/
├── main.py
│   Orkestrerar flödet via funktionsanrop
├── fetch.py
│   Hämtar nyckeltal från årsredovisning via yfinance
├── export.py
│   Sparar DataFrame till CSV i output/
├── logger.py
│   Central loggning + PDF-export + valbar mailfunktion
├── test.py
│   Tester för fetch, export, logger
├── output/
│   ├── omx30_nyckeltal.csv
│   ├── omx30_logg.txt
│   └── omx30_logg.pdf
│   Outputfiler (logg och data)
├── requirements.txt
│   Paket: pandas, yfinance, fpdf, etc.
└── README.md
    Dokumentation och körinstruktioner



## Installation

```bash
pip install -r requirements.txt


