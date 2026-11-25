# Moses Mendelssohn's Pentateuch – translation and Biur

<p align="center">
  <img src="portraits/mendelssohn.jpg" alt="Moses Mendelssohn" title="Moses Mendelssohn" height="180">
  <br>
  <sub>Moses Mendelssohn</sub>
</p>

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24466528.svg)](https://doi.org/10.5281/zenodo.24466528)

**English** · [Deutsch](README.de.md)

Moses Mendelssohn's German translation of the Five Books of Moses and the Hebrew commentary that accompanied it, the **Biur**, transcribed from the printed editions:

| Part | Edition | Verses | Characters |
| --- | --- | ---: | ---: |
| **Biur** (`biur/`) – Hebrew commentary | *Sefer Netivot ha-Shalom*, Vienna 1795 | 4,126 verses with comment | 3.2 million |
| **Taitsch** (`taitsch/`) – the German translation in Hebrew letters, as Mendelssohn printed it | same edition, Vienna 1795 | 5,847 | 0.8 million |
| **German translation in Latin script** (`dessau-1815/`) | *Die fünf Bücher Mose*, ed. D. Fränkel and M. H. Bock, Dessau 1815 | 5,846 | 0.8 million |
| **Word alignment** (`dessau-1815/alignment/`) – the Dessau text word by word against the Hebrew | Westminster Leningrad Codex | 5,846 | 81,190 segments |

The Biur is a joint work: following the usual attribution, Genesis is mostly by Solomon Dubno, Exodus by Mendelssohn himself, Leviticus by Naphtali Herz Wessely, Numbers by Aaron Jaroslaw and Deuteronomy by Herz Homberg, with Mendelssohn's revisions throughout. The introduction *Or li-Netivah* is not included.

The data were prepared for the free desktop library [Safran](https://github.com/mitkin89/Safran), where the translation can be shown under every Hebrew word (interlinear) and the Biur appears as a commentary next to the text.

## Format

- `biur/<Book>.json`, `taitsch/<Book>.json`, `dessau-1815/<Book>.json`: `{"book", "title", "verses": {"1:1": "…", …}}`. Verses follow the Hebrew numbering; verses without text are omitted.
- In the Biur, `<b>…</b>` marks the lemma and other words printed in square script (as against the Rashi script of the commentary), and `<br>` a paragraph break of the print.
- `dessau-1815/alignment/<Book>.json`: `{"verses": {"1:2": [[[1], "Die Erde aber"], [[2], "war"], …]}}` – the German segments in German order, each with the Hebrew words it renders (word numbers 1-based within the verse of the Westminster Leningrad Codex as in the [Open Scriptures Hebrew Bible](https://github.com/openscriptures/morphhb)). `[]` marks German words without a Hebrew counterpart; a Hebrew word rendered twice carries the same number twice.
- `docs/`: the review and correction lists of the Dessau text (German): misplaced sentence continuations returned to their verses, OCR candidates, possible omissions, and the printing appendix of Deuteronomy.

## Method and reliability

- The Vienna 1795 volumes (Taitsch and Biur) were transcribed page by page with Claude (Anthropic, 2026) from page images in eScriptorium; uncertain places were checked a second time. The Dessau 1815 text was corrected against the print where the review lists say so; the word alignment was made with Claude and reviewed.
- This is a working transcription, **not a critical edition**; it has not been proofread completely against the print. Please report errors as an issue, with book, verse and part.

## License

- Moses Mendelssohn (†1786) and his collaborators: the printed works are in the **public domain**.
- Transcriptions, structured data, word alignment and review lists: **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)**, see [LICENSE.md](LICENSE.md). The Hebrew word numbering refers to the Open Scriptures Hebrew Bible (CC BY 4.0).

## Citation

Itkin, Igor Mendel (ed.): *Moses Mendelssohn's Pentateuch – translation and Biur*, version 1.0.0, 2026. https://doi.org/10.5281/zenodo.24466528

See [CITATION.cff](CITATION.cff). Each release is archived on Zenodo with its own DOI.
