# perhogberg.se — PHU · Analyser av Per Högberg

Statisk webbplats på GitHub Pages med egen domän (perhogberg.se). Ingen byggprocess: ren HTML och CSS.

## Struktur

```
index.html                  Startsida (senaste utredningen framhävd)
utredningar/index.html      Lista över alla PHU-utredningar
phu01/index.html            Permanent adress för PHU01 (perhogberg.se/phu01)
phu01/filer/                Nedladdningsbara PDF:er (endast PDF publiceras)
phu01/rapport/              Hela rapporten som webbsida (svenska), byggs med pandoc
phu01/report/               Hela rapporten som webbsida (engelska)
phu01/*.md                  Textversioner för AI-verktyg
llms.txt, sitemap.xml       Vägvisare för sökmotorer och AI-verktyg
om/index.html               Om författaren, intressen och kontakt
ai-program/index.html       AI-program (tom tills första publiceras)
assets/style.css            Gemensam stilmall
assets/fonts/               Fira Sans, självhostad (OFL-licens), inga anrop till Google
assets/img/                 Märke (E, Avvikelsen), favicon, berättelsefält, delningsbilder
utredningar/ai-paverkan-pa-arbetskraften/   Vidarebefordran till /phu01/
```

## Grafiska regler

- Märke: E, Avvikelsen (rutnät där en punkt lämnat sin plats). Samma för alla rapporter.
- Beskrivning: "Analyser av Per Högberg" / "Analysis by Per Högberg".
- Fasta färger: navy #15213D, dimma #F2F6F8, bärnsten #C4701A (endast slutsatser), grå #5F6B7A.
- Accentfärg per rapport: 01 turkos #00939A, 02 grön #4E8A5E, 03 plommon #6B5B95, 04 stålblå #3D6A9E.
- Metodspråk (CSS-klasser .tag): fakta, berakning, antagande, scenario, slutsats.

## Lägga till en ny utredning (t.ex. PHU02)

1. Skapa `phu02/index.html` genom att kopiera `phu01/index.html`.
2. Sätt `--accent` för sidan till rapportens färg och byt innehåll, filer och trovärdighetsblock.
3. Lägg till ett kort i `utredningar/index.html` och uppdatera "Senaste utredningen" på startsidan.
