# FEKT.tex

LaTeX šablona pro sazbu studijních materiálů vytvořených studenty k přípravě na zkoušky.
Dokument obsahuje základní nastavení a představení různých funkcí.

## Použití

Nejjednodušší je stáhnout tento repozitář jako zip a nahrát jej do online LaTeX compileru [Overleaf](https://overleaf.com).

### Co upravit: `main.tex`

Soubor [`main.tex`](main.tex) pak obsahuje konkrétní nastavení dokumentu.

| Příkaz       | Popis | Příklad |
|--------------|-------|---------|
| \name        | Nadpis | BPC-SPR |
| \subname     | Podnadpis | Softwarové právo |
| \authors     | Seznam autorů dokumentu | A, B, C |
| \corrections | Seznam korektorů gramatiky či oprav formátování | C, A |
| \docdesc     | Popis dokumentu | Poznámky k předmětu |
| \docgroup    | Cílová skupina dokumentu | Informační bezpečnost, FEKT VUT |
| \docurl      | URL repozitáře | https://github.com/... |

Tyto příkazy jsou definovány v samém vrcholu dokumentu.
Pokud je smažete nebo zakomentujete, v dokumentu se nevyskytnou.

### Kam psát: `text/`

Dokumenty je zvykem členit do souvislých částí (kapitol), které se ukládají do složky `text/`.

Nejprve smažte soubor `text/00_fekt-tex`, protože ten pouze ukazuje jak tuto šablonu použít.
Poté vytvořte dokument nový, například `text/01_uvod.tex`. Do něj budete psát obsah samotný.
Pro každou novou kapitolu vytvořte samostatný soubor, kód se vám tak bude lépe udržovat.

## Údržba

Své úpravy stylu dokumentu provádějte pouze ve spodní části souboru, v kategorii DOKUMENT.

Když dojde k aktualizaci FEKT.tex, můžete otevřít zdrojový soubor `main.tex` a zkopírovat z něj vše mezi kategoriemi OBECNÉ NASTAVENÍ až DOKUMENT.

### GitHub releases

S pomocí GitHub Actions je nyní možné používat GitHub release na vydání nové verze pdf.
Stačí pouze nový commit v `main` větvi a GitHub Actions se o build a release postará.
Taktéž máme workflow pro kontrolu příchozích Pull Requestů, který neprojde pokud build selže.
Nejnovější release této šablony můžete vidět [zde](https://github.com/VUT-FEKT-IBE/FEKT.tex/releases/latest).
