# Ånge Camping · Elanalys 2025–2026

Statisk webbsida som visualiserar elförbrukning och spotelpriser för Ånge
Camping (ideell förening) under perioden 1 april 2025 – 31 mars 2026.

**Live:** https://speakman.github.io/ange-camping-elanalys/

## Innehåll

- `docs/index.html` — sidan (single-file, vanilla HTML/CSS/JS, hand-tecknade SVG-diagram)
- `docs/data.json` — pre-aggregerade siffror som sidan läser

## Källdata

- Timvis förbrukning från elnätsmätaren (455 dygn × 24 timmar = 10&thinsp;920 mätpunkter)
- Spotpriser för Elområde SE2 (Norra Mellansverige), månadsmedelvärden

## Vad räknas

Endast spotandelen av elkostnaden — påslag, energiskatt, nätavgift och moms
tillkommer på faktiskt fakturerad summa. Verklig totalkostnad ligger typiskt
2–3× högre än ren spot.

## Lokalt

```bash
cd docs && python3 -m http.server 8000
# öppna http://localhost:8000
```
