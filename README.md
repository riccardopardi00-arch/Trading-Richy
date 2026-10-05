# Trading Richy — versione definitiva

Web app personale per monitoraggio portafoglio e analisi informativa.

- 12 posizioni iniziali configurate
- prezzi EOD reali
- EODHD come fonte primaria
- Yahoo Finance come fallback server-side quando disponibile
- RSI, Stocastico, Williams %R, SMA 20/50
- P/L per posizione
- nessuna esecuzione di ordini
- chiave EODHD letta esclusivamente dalla variabile Netlify `EODHD_API_KEY`
- Netlify Function: `/.netlify/functions/market-data`

## Deploy
Usare un deploy che esegua il build/deploy delle Netlify Functions (Git/Agent Runner/CLI/API). Il semplice drag-and-drop statico non pubblica la Function.
