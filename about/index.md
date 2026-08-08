---
layout: default
title: "About the translations"
description: "How the translations are made, and how good they are -- the reading-grade standard, measured defect rates from adversarial verification, the editorial standards for fidelity and readability, and what is not being claimed."
seo:
  type: WebPage
permalink: /about/
---

# About the translations

Translations are produced with an automated, AI-assisted pipeline that runs each text through a multi-stage workflow before final collation. For technical details, see the translator's [translation-pipeline](https://github.com/sweisman/translation-pipeline) repo.

These translations are prepublication texts -- nearly publication-ready, pending the diagrams and illustrations still in progress.

## Reading grade, not citation grade

There are two standards this kind of work can be held to, and it is worth being explicit about which one these texts meet.

**Reading grade** means a complete English text of a book that has never had one: accurate in substance, faithful to the author's argument, good enough to work from and to read for pleasure. That is what these translations are, and it is achieved now.

**Citation grade** is stricter. It means every line has been independently read against the printed page, with the remaining uncertainties enumerated rather than unknown -- the standard a critical edition must meet before a scholar quotes it as evidence in print. No work in this corpus is citation grade, and none is offered as one. Where a passage carries real weight, check it against the source; the source is linked from every work's page.

The distinction is not modesty. It follows from how this kind of translation fails, which is quietly. A machine that cannot read a word does not stop -- it produces a word, in fluent English, indistinguishable from the words around it. Nothing in the finished prose marks the difference between a good reading and a bad one, which is why the only meaningful question about a translation like this is not how it reads but how it was checked.

## How the quality is measured

Skepticism about machine translation of historical books is reasonable, and the answer to it is measurement rather than assurance.

Quality here is measured adversarially. An independent reader, denied the existing translation, works from the page images, forms its own understanding, and only then compares against the committed text -- quoting the printed reading beside the translated one for every divergence. Anything consequential is checked a third time.

That third step is not a formality. Roughly one criticism in six does not survive it, and the errors run in both directions: the most instructive case on record is one where the machine was right and the criticism wrong, resolved only by re-examining the page at high magnification. Verification that is not itself verified manufactures false accusations.

## What the measurements show

| Material | Defects per 1,000 words |
| --- | --- |
| Latin printed prose, institutional greyscale scans | about 1 |
| Hebrew printed prose, one-bit thresholded scans | about 10 |

The gap between those two rows is mostly the scan rather than the language. A one-bit scan deletes a light impression rather than merely dimming it, and no later processing recovers it; source quality is settled before a word is translated and cannot be revisited afterwards. Those Hebrew figures are a floor, not a verdict on Hebrew.

Where the material is regular, the results are better than one would expect. Five sets of Clavius's numeric tables were verified exhaustively -- roughly nine thousand numerals, with essentially no misreadings. The handful of exceptions were not misreadings at all, but places where the translation had quietly corrected the printer, and correctly.

The intuitive worry about Hebrew -- *gematria*, where numbers are written as letters embedded in running prose -- is not what fails. Across the most date-dense passages examined, the numerals came through very nearly perfect, Hebrew-calendar years included.

One book has been carried further than the rest as a test of the ceiling: translated twice, independently, from two different digitisations, neither translation aware of the other, and the two English texts then collated against each other across about two hundred thousand words of parallel text. That located several hundred points of genuine disagreement, every one of which had passed both translations' own internal review. It also established the limit of the technique: the two independent translations are wrong *together* perhaps a sixth of the time, and no amount of comparison finds those. Only reading the page finds those.

## Where it fails

Three findings are worth stating plainly, because they govern what this method can be trusted to do.

**The machine's own confidence inverts.** Translations mark the passages they are unsure of. Those marks measure the difficulty of the language, not the quality of the output, and they are anti-correlated with real defects -- across the worst-marked passages examined, the large majority of marks sat on text that was simply legible and hedged, while the worst passage found anywhere was among the least-marked. Nothing should be triaged by the machine's own confidence, and the `[?]` marks in these texts should not be read as a map of where the errors are.

**Sampling locates defects without measuring them.** One damaged passage of tables was checked twice, once by sampling and once by reading every cell; the complete reading found several times more, including corrupted material in a block the sample had never opened. Every clean verdict anywhere should be read as clean *where read*.

**Arithmetic cannot check this work.** Astronomical tables are highly regular, which makes it tempting to verify them automatically. It cannot be done: asked for a value it cannot read, a machine supplies the one the pattern predicts, so a fabricated cell satisfies the table's own symmetries *better* than the true value. Automatic checks were built for this and discarded. The page has to be read.

## What is possible

Citation grade has not been reached in this corpus, but it has been shown reachable rather than merely asserted. One shorter work received complete rather than sampled treatment -- every batch of it verified line by line -- and the result was a text whose remaining defects are enumerated rather than unknown. That pass also found a systematic fault in the inline Greek that no amount of sampling had surfaced, and found something to correct in every single batch.

That is the honest shape of it. The failures are bounded, locatable and quotable, and a book can be brought to a state where what is uncertain about it is written down. What that takes is reading all of it against the page -- which is affordable in a way that producing the first draft never was, and which is exactly the work these editions have not yet had.

## Fidelity and readability

The goal is fluent, readable modern English -- a text an educated reader can follow without reaching for the Latin or Hebrew, not one written only for specialists. Rather than reproduce the long periodic sentences and deferred verbs of the originals, the translations carry the author's meaning, argument, and tone into natural contemporary prose: where Tycho builds a single sentence whose main verb arrives only after four nested clauses, the translation breaks it into the two or three a modern writer would use. Fidelity comes first, though -- nothing is dropped, summarized, or invented, and negations, numbers, technical terms, and the author's own examples and analogies are preserved exactly. Readability never comes at the cost of changing what the source says.

## Technical vocabulary

Technical vocabulary stays precise and is anchored to its modern equivalents. A key Latin or Hebrew term of art is glossed on its first occurrence -- the original shown alongside the English rendering -- and thereafter carried in settled English. Historical names, star names, and specialized vocabulary carry inline identifications: Tycho's "Lucida Vulturis volantis" is identified as Altair in Aquila; Gersonides' medieval Hebrew astronomical terminology is mapped to the Ptolemaic system it describes.

## Mathematical and astronomical content

Mathematical and astronomical content -- sexagesimal values, spherical triangle computations, calendar arithmetic, tabular data -- is reproduced with the precision of the originals, cell by cell and degree by degree. Compositor errors in the source are corrected inline with `[recte: ...]` notation rather than silently emended. Uncertain readings due to ink damage, worn type, or ambiguous letterforms are marked with `[?]`, preserving the translator's best reading rather than dropping it. This page used to describe those marks as flagging a passage for editorial review, which implied more than they can carry: measurement showed that most of them sit on text that is perfectly legible, and that the genuinely bad passages are often unmarked. Read them as an invitation to check the source, not as an index of where the errors are.

## Illustrations and diagrams

The publicly available PDFs are text-only. Geometric figures, instrument schematics, concentric-sphere charts, and other diagrams from the source works are extracted and replaced with structured descriptions identifying every label, arc, point, and geometric relationship visible in the original woodcut or engraving. Tycho's _De Mundi Aetherei_, for example, carries 93 such figures, from spherical-astronomy constructions to the two-circle hypothesis of the comet's eccentric orbit within the solar sphere. For a high-quality illustrated print edition of any of these works, please get in touch using the contact details on the front page.

<p><a href="/">&larr; Ars Astronomica</a></p>
