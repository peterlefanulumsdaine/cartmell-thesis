cartmell-thesis
===============

A (proposed) HoTT group project to TeXify Cartmell's PhD thesis “Generalised Algebraic Theories and Contextual Categories” — an important paper that’s currently not very accessible.

# General project notes

## Contributing 

- Please read adhere to the conventions agreed on below!
- To decide: fork/pull, or direct push?
- Signup sheet for sections?

# Conventions

## Faithfulness to original

- General layout, formatting: to be discussed.
- Punctuation etc: stick closely to Cartmell's (sometimes idiosyncratic), except when inconsistent, in which case go with his most frequent usage.
- Typos: correct unambiguous typos.  Add flag for proofreaders?
- Accents: add where missing. (Notably `Martin-L\"o{}f`).
- Italics/emphasis not used in original.  Add anywhere, e.g. for definienda?
- 

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

## Macros

- ALWAYS use semantic macros!  (How far to take this, though?)

- Commands denoting syntax of object theories: all begin `\syn`, eg `\synHom` in discussing the theory of categories

- single letter commands: undecided, but at least for now, keep descriptive, eg `\catC` for a *C* denoting a category, `\varV` for *V* denoting a set of variables, etc.

 
