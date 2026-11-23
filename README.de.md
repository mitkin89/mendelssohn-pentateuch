# Moses Mendelssohns Pentateuch – Übersetzung und Biur

[English](README.md) · **Deutsch**

Moses Mendelssohns deutsche Übersetzung der fünf Bücher Mose und der hebräische Kommentar, der sie begleitete, der **Biur**, nach den gedruckten Ausgaben transkribiert:

| Teil | Ausgabe | Verse | Zeichen |
| --- | --- | ---: | ---: |
| **Biur** (`biur/`) – hebräischer Kommentar | *Sefer Netiwot ha-Schalom*, Wien 1795 | 4.126 Verse mit Kommentar | 3,2 Mio. |
| **Taitsch** (`taitsch/`) – die deutsche Übersetzung in hebräischen Buchstaben, wie Mendelssohn sie druckte | dieselbe Ausgabe, Wien 1795 | 5.847 | 0,8 Mio. |
| **Deutsche Übersetzung in lateinischer Schrift** (`dessau-1815/`) | *Die fünf Bücher Mose*, hg. von D. Fränkel und M. H. Bock, Dessau 1815 | 5.846 | 0,8 Mio. |
| **Wortzuordnung** (`dessau-1815/alignment/`) – der Dessauer Text Wort für Wort gegen das Hebräische | Westminster Leningrad Codex | 5.846 | 81.190 Segmente |

Der Biur ist ein Gemeinschaftswerk: Nach der üblichen Zuschreibung stammt Genesis größtenteils von Salomon Dubno, Exodus von Mendelssohn selbst, Leviticus von Naphtali Herz Wessely, Numeri von Aaron Jaroslaw und Deuteronomium von Herz Homberg, durchgehend mit Mendelssohns Überarbeitung. Die Einleitung *Or li-Netiwa* ist nicht enthalten.

Die Daten entstanden für die freie Desktop-Bibliothek [Safran](https://github.com/mitkin89/Safran). Dort lässt sich die Übersetzung unter jedes hebräische Wort stellen (Interlinear), und der Biur steht als Kommentar neben dem Text.

Aufbau und Auszeichnung sind in der [englischen Fassung](README.md#format) beschrieben.

## Methode und Verlässlichkeit

- Die Wiener Bände von 1795 (Taitsch und Biur) wurden Seite für Seite mit Claude (Anthropic, 2026) nach Seitenbildern in eScriptorium transkribiert; unsichere Stellen wurden ein zweites Mal geprüft. Der Dessauer Text von 1815 wurde gegen den Druck berichtigt, wo die Prüflisten es angeben; die Wortzuordnung entstand mit Claude und wurde geprüft.
- Das ist eine Arbeitstranskription, **keine kritische Edition**, und nicht vollständig gegen den Druck Korrektur gelesen. Fehler bitte als Issue melden, mit Buch, Vers und Teil.

## Lizenz

- Moses Mendelssohn (†1786) und seine Mitarbeiter: Die gedruckten Werke sind **gemeinfrei**.
- Transkriptionen, strukturierte Daten, Wortzuordnung und Prüflisten: **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de)**, siehe [LICENSE.md](LICENSE.md). Die hebräische Wortzählung bezieht sich auf die Open Scriptures Hebrew Bible (CC BY 4.0).

## Zitieren

Siehe [CITATION.cff](CITATION.cff). Jede Version wird auf Zenodo mit eigener DOI archiviert.
