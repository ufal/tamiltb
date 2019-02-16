# This Makefile describes how to update the CoNLL-X files when the master Treex file changes.
conll:
	treex -Lta Read::Treex from=tamiltb.treex Write::CoNLLX is_member_within_afun=1 to=tamiltb.conll
	split_conll.pl < tamiltb.conll -head 480 traindev.conll test.conll
	split_conll.pl < traindev.conll -head 400 train.conll dev.conll
	rm traindev.conll
