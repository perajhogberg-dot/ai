# ai

Källkod för Per Högbergs bibliotek över utredningar och AI-program, publicerad via GitHub Pages.

## Struktur

```
/index.html                          Startsida
/utredningar/index.html              Lista över utredningar
/utredningar/<slug>/index.html       En utrednings egen sida
/utredningar/<slug>/filer/           Nedladdningsbara dokument (PDF/Word)
/ai-program/index.html               Lista över AI-program
/ai-program/<slug>/index.html        Ett programs egen sida (dokumentation eller körbar demo)
/assets/style.css                    Delad stilmall för hela sajten
```

## Lägga till en ny utredning

1. Skapa `/utredningar/<ny-slug>/index.html` (kopiera strukturen från `ai-paverkan-pa-arbetskraften`).
2. Lägg dokumenten i `/utredningar/<ny-slug>/filer/`.
3. Lägg till ett kort i `/utredningar/index.html`.

## Lägga till ett nytt AI-program

1. Skapa `/ai-program/<ny-slug>/index.html`.
2. Om det är en körbar demo: bygg den som en fristående HTML/JS-sida i samma mapp.
3. Lägg till ett kort i `/ai-program/index.html`.

## Hosting

Statisk sajt via GitHub Pages. Inget byggsteg — filerna serveras som de ligger i repot.
Anpassad domän kopplas via en `CNAME`-fil i repots rot plus DNS-poster hos domänleverantören.
