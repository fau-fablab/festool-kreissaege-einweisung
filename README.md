Festool-Kreissäge Einweisung
============================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die Tauchsäge Festool TS 55 REBQ mit Führungsschiene.

Inhalt
------

- Technische Daten, Bedienelemente (Fotos mit Bedienhinweisen), allgemeine Sicherheitshinweise (Sägeblatt, Rückschlag, Holzstaub)
- Schutzausrüstung, bestimmungsgemäße Verwendung, Aluminiumbearbeitung
- Einstellungen: Schnitttiefe, Schnittwinkel, Sägeblattwechsel

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/festool-kreissaege-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/einweisung_Kreissaege.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/einweisungsliste_Kreissaege.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/festool-kreissaege-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/festool-kreissaege-einweisung.git
cd festool-kreissaege-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/status.svg)](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/festool-kreissaege-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/festool-kreissaege-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/festool-kreissaege-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

Die Einweisung und die Betriebsanweisung (`betriebsanweisung/ba_handkreissaege.tex`, BA-HK-01) sind selbst
formuliert und enthalten keine Texte oder Abbildungen aus der Festool-Betriebsanleitung, nur ISO-7010-Symbole.
Die Fotos in `bilder/` stammen von Oxensepp (Wikimedia Commons) und stehen unter CC BY-SA 3.0, siehe
[bilder/QUELLEN.md](bilder/QUELLEN.md).
Für Details wird auf die Originalanleitung von Festool verwiesen. **Beim Bearbeiten nichts aus der
Festool-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.** Bilder bitte selbst fotografieren
oder nur mit freier, kompatibler Lizenz verwenden.
