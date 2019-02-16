# TamilTB

This package contains a morphologically and syntactically (dependency) annotated corpus for Tamil. There are 600 sentences (trees) and 9581 tokens (non-root nodes).

The static copy in /net/data/TamilTB has not been touched since 2013. It apparently corresponds to the release 0.1. Since then, the Universal Dependencies conversion has been the more visible version of the corpus. However, we should be able to fix errors in the original Prague-style annotation.

Loganathan Ramasamy, the author of the original treebank, is no longer a member of ÚFAL. This repository has been started by Dan Zeman, based on the release 0.1.


## Contents of this package

    data/
	./TamilTB.v0.1.treex - Dependency treebank in Treex format
	./TamilTB.v0.1.conll - Dependency treebank in CoNLL-X format
	./train.conll - First 480 sentences / 7592 tokens of the treebank, intended for training of models
	./test.conll - Last 120 sentences / 1989 tokens of the treebank, intended for testing of models
    doc/
	./index.html - Documentation for the treebank data
	...
    README.md - This file


## Treex Format

Dependency trees can be viewed/modified using tree editor [TrEd](https://ufal.mff.cuni.cz/tred) with the EasyTreex extension.


## CoNLL Format

CoNLL format is provided mainly to use machine learning tools to train and test tagging and parsing models. It is created automatically from the Treex version, which is the master file.


## License

TamilTB.v0.1 by Institute of Formal and Applied Linguistics (ÚFAL) is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/).
