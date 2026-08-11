---
layout: default
title: "About the translations"
description: "How the translations are made, how their quality is measured, the distinction between reading-grade and citation-grade texts, and the editorial standards for fidelity and readability."
seo:
  type: WebPage
permalink: /about/
---

# About the translations

Translations are produced with an automated, AI-assisted pipeline that takes each text through a multi-stage workflow before final collation. For technical details, see the translator's [translation-pipeline](https://github.com/sweisman/translation-pipeline) repo.

The translations available here are prepublication texts: substantially complete and nearly publication-ready, with diagrams and illustrations still in progress.

## Reading grade, not citation grade

It is useful to distinguish between two standards for this kind of work.

**Reading grade** means a complete and substantially accurate English text: faithful to the author's argument, suitable for serious study, and readable as a book in its own right. For many works in this collection, it is the first complete English translation available. The translations here meet that standard.

**Citation grade** is stricter. It means that every line has been independently checked against the printed or manuscript page and that the remaining uncertainties are known and explicitly recorded. That is the standard required before a translation can be treated as a critical scholarly text.

No work in this corpus is currently offered as citation grade. Where a passage carries substantial scholarly weight, it should be checked against the original source, which is linked from every work's page.

The distinction matters because errors in machine-assisted translation are not necessarily visible in the finished prose. A system that misreads a word may still produce fluent English, and a bad reading can look just as natural as a good one. Fluency therefore says little by itself about reliability. The more important question is how the translation was checked.

## How the quality is measured

Skepticism about machine translation of historical books is reasonable. The useful answer is measurement.

Quality is tested adversarially. An independent reader works from the page images without seeing the existing translation, determines what the source says, and only then compares that reading against the committed text. For each substantive divergence, the printed reading and the translation are examined together. Consequential disagreements receive a third check.

That final check is important. Roughly one criticism in six has failed to survive it. Errors occur in both directions: in one particularly instructive case, the translation was correct and the criticism was wrong, something that became clear only after the original page was re-examined at high magnification.

Verification therefore has to be verified as well.

## What the measurements show

| Material | Defects per 1,000 words |
| --- | --- |
| Latin printed prose, institutional greyscale scans | about 1 |
| Hebrew printed prose, one-bit thresholded scans | about 10 |

Much of the difference between those figures appears to come from the scans rather than the languages themselves. A greyscale scan can preserve a faint impression; a one-bit scan may erase it entirely. Once information has disappeared from the source image, later processing cannot recover it. The Hebrew figure therefore reflects the quality of the available digitization as much as the difficulty of the text.

Where the source material is clean and regular, the results can be considerably better. Five sets of Clavius's numerical tables were checked exhaustively -- roughly nine thousand numerals -- with essentially no transcription errors. The few apparent exceptions turned out to be places where the translation had correctly repaired errors made by the original printer.

The intuitive concern about Hebrew numerals and *gematria*, where numbers appear as letters embedded in running prose, has also proved less serious than expected. Across the most date-dense passages examined, numerical readings have been highly reliable, including Hebrew-calendar years.

One book has been tested much more extensively than the rest. It was translated twice, independently, from two different digitizations, with neither translation having access to the other. The resulting English texts were then collated across about two hundred thousand words of parallel text.

That comparison located several hundred genuine disagreements that had survived both translations' internal review. It also revealed the limit of the technique: sometimes both translations make the same mistake. Comparison between independent translations can find many errors, but it cannot replace checking the original page.

## Where it fails

Testing has revealed several limitations that are important when using these editions.

**The machine's own confidence is a poor guide.** Translations mark passages where the system is uncertain, but those marks tend to reflect linguistic difficulty rather than actual output quality. Many heavily marked passages are perfectly legible, while serious errors may appear in passages with no warning at all. The `[?]` marks in these texts should therefore not be read as a map of where the errors are.

**Sampling finds defects without proving that unchecked material is clean.** One damaged passage of tables was reviewed twice, first by sampling and then cell by cell. The complete review found several times as many defects, including corrupted material in a block the sample had never examined. A clean sample means only that the material actually checked was clean.

**Arithmetic cannot safely verify the text.** Astronomical tables are highly regular, which makes automatic consistency checking tempting. In practice, that regularity creates a danger: when a value is unreadable, a system may supply the value that the mathematical pattern predicts. A fabricated reading can therefore fit the table more neatly than the number actually printed on the page. Automatic checks were tested for this purpose and discarded.

For final verification, the page itself has to be read.

## What is possible

Citation-grade verification has not yet been completed across the corpus, but it has been demonstrated on a smaller scale.

One shorter work received complete rather than sampled treatment, with every batch checked line by line against the original. That pass found something to correct in every batch, including a systematic problem with inline Greek that sampling had failed to expose.

The result was a text in which the remaining uncertainties were known and could be listed explicitly rather than simply assumed to be absent.

Bringing an entire book to that standard requires reading the full translation against the source page by page. The automated pipeline makes the production of the initial English text inexpensive enough that this final verification becomes practical. That is the standard toward which these editions can ultimately be developed.

## Fidelity and readability

The goal is fluent, readable modern English: a text an educated reader can follow without constantly reaching for the Latin or Hebrew.

The syntax of the original is therefore not reproduced mechanically. A long Latin period whose main verb appears only after several nested clauses may become two or three English sentences. The structure changes where necessary; the argument does not.

Nothing is intentionally omitted, summarized, or invented. Negations, numbers, technical terms, distinctions, examples, and analogies are preserved. Readability matters, but it does not take precedence over what the source actually says.

## Technical vocabulary

Technical vocabulary is translated consistently and, where useful, connected with its modern equivalent.

A significant Latin or Hebrew term of art may be glossed at its first appearance, with the original shown alongside the English rendering, and then carried consistently thereafter. Historical names, star names, and specialized vocabulary are identified where doing so helps the reader.

Tycho's "Lucida Vulturis volantis," for example, is identified as Altair in Aquila, while Gersonides' medieval Hebrew astronomical terminology is related to the corresponding concepts of the Ptolemaic system.

## Mathematical and astronomical content

Mathematical and astronomical material -- sexagesimal values, spherical-triangle calculations, calendar arithmetic, and tabular data -- is treated as part of the text rather than as incidental content.

Tables are reproduced cell by cell and degree by degree. Apparent compositor errors in the original are corrected explicitly with `[recte: ...]` notation rather than silently emended.

Where damaged ink, worn type, or an ambiguous letterform prevents a secure reading, the translator's best reading is retained and marked `[?]`.

Those marks indicate uncertainty in the source reading. They should be treated as an invitation to consult the original, not as a comprehensive indication of where translation errors are likely to occur.

## Illustrations and diagrams

The publicly available PDFs are currently text-only.

Geometric figures, instrument schematics, concentric-sphere charts, and other diagrams from the source works are extracted and represented with structured descriptions identifying the labels, arcs, points, and geometric relationships visible in the original woodcut or engraving.

Tycho's _De Mundi Aetherei_, for example, contains 93 such figures, ranging from constructions in spherical astronomy to diagrams of the comet's proposed eccentric orbit within the solar sphere.

For inquiries about producing a high-quality illustrated print edition of any of these works, please get in touch using the contact details on the front page.

<p><a href="/">&larr; Ars Astronomica</a></p>
