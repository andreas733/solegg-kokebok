# Kvitteringer

Database over alle kvitteringer. Legg til nye ved å sende bilde til Rigel.

## Alle kvitteringer

```dataview
TABLE dato, butikk, beløp, mva, kategori, betalingsmåte
FROM "Kvitteringer"
WHERE file.name != "_mal-kvittering" AND file.name != "Kvitteringer"
SORT dato DESC
```

## Kategorier

Gyldige kategorier:
- `mat` — dagligvarer og matbutikker
- `restaurant` — spisesteder og takeaway
- `klær` — klær og sko
- `elektronikk` — tech og gadgets
- `hjem` — interiør og husholdning
- `helse` — apotek og treningssenter
- `annet` — alt annet

## Betalingsmåter

- `kort` — debet-/kredittkort
- `vipps` — Vipps
- `kontant` — kontanter
