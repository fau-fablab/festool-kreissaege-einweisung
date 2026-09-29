Festool-Kreissäge Einweisung
============================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die Tauchsäge Festool TS 55 REBQ mit Führungsschiene.

Inhalt
------

- Technische Daten, allgemeine Sicherheitshinweise (Sägeblatt, Rückschlag, Holzstaub)
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

Die Einweisung und die Betriebsanweisung (`betriebsanweisung/ba_handkreissaege.tex`, BA-HK-01) sind selbst
formuliert und enthalten keine Texte oder Abbildungen aus der Festool-Betriebsanleitung, nur ISO-7010-Symbole.
Für Details wird auf die Originalanleitung von Festool verwiesen. **Beim Bearbeiten nichts aus der
Festool-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.** Bilder bitte selbst fotografieren.

Offen: Die Platzhalter `\todo` in der Einweisung stehen für eigene Fotos der Säge.
