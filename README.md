
"He Said She Said" classification challenge (2nd edition)
=========================================================

Give the probability that a text in Polish was written by a man.

This challenge is based on the "He Said She Said" corpus for Polish.
The corpus was created by grepping gender-specific first person
expressions (e.g. "zrobiłem/zrobiłam", "jestem zadowolony/zadowolona",
"będę robił/robiła") in the Common Crawl corpus. Such expressions were
normalised here into masculine forms.

Classes
-------

* `0` — text written by a woman
* `1` — text written by a man

Directory structure
-------------------

* `README.md` — this file
* `config.txt` — configuration file
* `train/` — directory with training data
* `train/train.tsv.gz` — train set (gzipped), the class is given in the first column,
  a text fragment in the second one
* `train/meta.tsv.gz` — metadata (do not use during training)
* `dev-0/` — directory with dev (test) data
* `dev-0/in.tsv` — input data for the dev set (text fragments)
* `dev-0/expected.tsv` — expected (reference) data for the dev set
* `dev-0/meta.tsv` — metadata (not used during testing)
* `dev-1/` — directory with extra dev (test) data
* `dev-1/in.tsv` — input data for the extra dev set (text fragments)
* `dev-1/expected.tsv` — expected (reference) data for the extra dev set
* `dev-1/meta.tsv` — metadata (not used during testing)
* `test-A` — directory with test data
* `test-A/in.tsv` — input data for the test set (text fragments)
* `test-A/expected.tsv` — expected (reference) data for the test set (hidden)
