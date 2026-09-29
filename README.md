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

**Noch ungeklärt:** Die Einweisung enthält Texte und Abbildungen aus der Betriebsanleitung von Festool, deren Rechte bei Festool liegen.

Die Betriebsanweisung (`betriebsanweisung/ba_handkreissaege.tex`, BA-HK-01) ist dagegen komplett
selbst formuliert und enthält keine Texte oder Abbildungen von Festool, nur ISO-7010-Symbole.
Sie kann daher unabhängig von der Festool-Frage veröffentlicht werden. **Beim Bearbeiten nichts
aus der Festool-Anleitung übernehmen, auch nicht sinngemäß Satz für Satz.**

Eine lizenzsichere Einweisung ließe sich genauso aufbauen: eigene Formulierungen, eigene Fotos
statt Festool-Grafiken, für Details Verweis auf die Originalanleitung (Link auf festool.com)
statt Abdruck. Alternativ Festool um schriftliche Erlaubnis bitten.
