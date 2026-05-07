# Obce v datech — návrh nového webu

HTML mockupy pro nový web datové společnosti **Obce v datech**.

## Kanonické vstupní body

Vždy linkujte na tyto názvy — automaticky ukazují na nejnovější verzi:

| Soubor | Co je to |
|---|---|
| `index.html` | Domovská stránka |
| `navrh-rozcestnik.html` | Rozcestník po vyhledání obce (3 stavy: město / obec s produkty / obec bez produktů) |
| `navrh-profil-obce.html` | Datový profil obce — Index kvality života |
| `navrh-koupit-report.html` | Stránka prodeje reportu |

## Verze (pracovní iterace)

- `navrh-home-v1…v6.html` — iterace home
- `navrh-profil-obce-v1…v11.html` — iterace profilu obce

`index.html` = kopie poslední verze home, `navrh-profil-obce.html` = kopie poslední verze profilu.

## Datové soubory (embedded)

- `data.json` — kompletní zdroj (206 měst × 30 indexů × 88 ukazatelů × 8 let)
- `_profil_data.json` — extrakt pro embed do profilu (~85 KB)
- `_obce_data.json` — databáze 256 obcí pro autocomplete
- `_ikz_mini.json` — mini data pro náhled v rozcestníku

## Stack

- Tailwind CSS (CDN) + inline `tailwind.config`
- Plus Jakarta Sans + Inter (Google Fonts)
- Vanilla JS — žádný build, otevřete kterýkoli HTML přímo v prohlížeči

## Spuštění

Otevřete `index.html` v prohlížeči, nebo spusťte lokální server:

```bash
python -m http.server 8000
# pak http://localhost:8000
```

## GitHub Pages

Repo lze publikovat přes GitHub Pages — `index.html` je automatický vstupní bod.
