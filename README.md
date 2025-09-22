# Aktie_projekt_Python

# OMX30 Nyckeltalsmotor

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
├── main.py # Orkestrerar flödet via funktionsanrop 
├── fetch.py # Hämtar nyckeltal från årsredovisning 
├── export.py # Sparar CSV till output/ 
├── logger.py # Loggning + mailfunktion (valbart) 
├── test.py # Tester för fetch, export, logger 
├── output/ # Outputfiler 
│ ├── omx30_nyckeltal.csv 
│ └── omx30_logg.txt
├── requirements.txt # Paket: pandas, yfinance, etc. 
├── README.md # Dokumentation


## Installation

```bash
pip install -r requirements.txt


