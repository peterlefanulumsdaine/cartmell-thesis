cartmell-thesis
===============

A collaborative project to TeXify Cartmell's PhD thesis “Generalised Algebraic Theories and Contextual Categories” — an important paper that’s currently not very accessible.

The scanned original is available from http://peterlefanulumsdaine.com/files/cartmell-1978-phd-thesis.pdf.

# General project notes

## Contributing 

- Please read and adhere to the conventions agreed on below! But feel free to make judgment calls as needed.
- Use the [status file](signup.md) to monitor + record progress, and reserve sections you’re currently working on.
- New contributors: please fork and issue pull requests to contribute.

# Conventions

## Faithfulness to original

- General layout + formatting: stick roughly to original, but no need to bend over bakcwards.
- Typos: correct unambiguous typos; if in doubt, leave unchanged but add comment for proofreaders.
- Punctuation etc: stick closely to Cartmell's (sometimes idiosyncratic), except when inconsistent to the extent of being a typo.
- Accents: add where missing. (Notably `Martin-L\"o{}f`).
- Bibliography: probably modernise bibliography style; for now keep citation style unchanged (i.e. numeric), possibly change to a more reader-friendly style (e.g. alphabetical).

## General LaTeX style

- Within a paragraph, separate sentences by blank-except-percent lines, e.g.

    This makes diffs clearer.
    %
    I learned this style from Andrej Bauer.

- Mark page breaks of the source like follows:

    The source pdf is not searchable.
    %
    % source p2.17
    %
    Page numbers thus help navigation.

- Labels/references: not fully decided yet, template `\ref{sec:source-1-8}` seems robust in this situation, and means one can input them from the link text without having to break flow and flip ahead to the linked section.  Possibly change later to more semantic text though?

- Cartmell often uses un-bulleted but line-broken lists (e.g. bottom of source p 1.4).  For now, do as `itemize`?

- Cartmell often uses inline numbered lists: do these with environment `enumerate*`

## Macros

- ALWAYS use semantic macros!  (How far to take this, though?)

- Commands denoting syntax of object theories: all begin `\syn`, eg `\synHom` in discussing the theory of categories

- single letter commands: undecided, but at least for now, keep descriptive, eg `\catC` for a *C* denoting a category, `\varV` for *V* denoting a set of variables, etc.

 
