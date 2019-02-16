# TamilTB

This package contains a morphologically and syntactically (dependency) annotated corpus for Tamil. There are 600 sentences (trees) and 9581 tokens (non-root nodes).

The static copy in /net/data/TamilTB has not been touched since 2013. It apparently corresponds to the release 0.1. Since then, the Universal Dependencies conversion has been the more visible version of the corpus. However, we should be able to fix errors in the original Prague-style annotation.

Loganathan Ramasamy, the author of the original treebank, is no longer a member of ÚFAL. This repository has been started by Dan Zeman, based on the release 0.1.


## Contents of this package

    data/
	./TamilTB.v0.1.tmt - Dependency treebank in TMT format
	./TamilTB.v0.1.conll - Dependency treebank in CoNLL-X format
	./TamilTB.v0.1.tt - Words, POS tags and lemmas from the treebank in the vertical format expected by the TnT tagger
    doc/
	./index.html - Documentation for the treebank data
	...
    README.md - This file


## TMT Format

Dependency trees can be viewed/modified using tree editor [TrEd](https://ufal.mff.cuni.cz/tred).
Use tmttred for viewing TamilTB.v0.1.tmt.


## CoNLL Format

CoNLL format is provided mainly to use machine learning parsers to train the parsing models for Tamil


## POS Tagged Corpora

The POS tagged corpora can be used to train the machine learning taggers. The data follows the TnT format.

The first column contains the wordform.
The second column contains the POS tag.
The third column contains the lemma.


## License

TamilTB.v0.1 by Institute of Formal and Applied Linguistics (ÚFAL) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/).
