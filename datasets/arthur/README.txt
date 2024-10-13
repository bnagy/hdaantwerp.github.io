# Arthur

## Provenance
The table `manuscripts.csv` is a comma-separated file encoded as UTF-8. It features metadata on the medieval manuscripts containing Arthurian narrative fiction. The data is based on the following online resource: "Arthurian Fiction in Medieval Europe: Narratives and Manuscripts" [[http://www.arthurianfiction.org/]] (courtesy of Prof. Dr. Bart Besamusca, University of Utrecht). The curators of this resource put the underlying database for the website at our disposal (d.d. 02 October 2020) in JSON, which we preprocessed into CSV (and which we simplified somewhat for pedagogical purposes).

## Columns
In the data, each row represents a single manuscript (or the remnants of it). More detailed information is provided in Dutch [on the website](http://www.arthurianfiction.org/Teaching%20Module%20CLARIN%20ArthurianFiction.pdf) but we summarize the nature of each column here:
- signature (`str`): the current signature (e.g. in a library) of the object
- repository (`str`): the institution where the book is currently kept
- script (`str`): the type of letter ("font") used; e.g. `"textualis"` for a traditional Gothic letter
- text-height (`int`): height (in milimeters) of the text area (i.e. written surface)
- text-width (`int`): width (in milimeters) of the text area (i.e. written surface)
- illustrations (`int`): the number of illustrations in the manuscript
- date_min (`int`): date *after* which the manuscript was produced (can be identical to `date_min`)
- date_max (`int`): date *before* which the manuscript was produced (can be identical to `date_max`)
- leaf-height (`int`): height (in milimeters) of the full page
- leaf-width (`int`): width (in milimeters) of the full page
- number-lines (`int`): the number of lines on a page
- material (`str`): the material of the pages (mainly parchment or vellum)
- physical-type (`str`): the physical integrity of the book (a fully surviving codex versus a fragment)
- country (`str`): the country where the manuscript originated from
- region (`str`): the region where the manuscript originated from
- columns (`int`): the number of text columns on each page

The data contains `NA`s in various cells where information is lacking or simply hasn't been entered yet.