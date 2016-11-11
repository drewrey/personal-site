---
layout: page
title: learning journal
permalink: /learning_journal/
---

This page is a collection of small things I've learned over time. I find it useful to peruse to reinforce learning.


---

2016 Nov 8
===

- Java auto un boxing between primitive type and object type. For example: `double` to `Double`


2016 Nov 2
===

- EAV: entity attribute value (not just east Atlanta village)


2016 Oct 10
===

- used jvisualvm to connect to a running java app, make a heapdump, and then peruse it locally


2016 Oct 7
===

- check if rows 1 and 2 are exactly the same in excel:
    - `=AND(EXACT(1:1, 2:2))`


2016 Sept 27
===

- `git log - -grep`


2016 Sept 26
===

- you can edit `/etc/hosts` to map `127.0.0.1` to something other than localhost


2016 Sept 22
===

- frequent itemsets (e.g. buying diapers & beer at the same time)
    - aka association rules


2016 Sept 18
===

- “spoonerism”: the transposition of initial or other sounds of words, as in a blushing crow for a crushing blow.


2016 Sept 8
===

- ICA (Independent Component Analysis):
    - does not assume that components will be orthogonal, but relies on assumption of statistical independence. accordingly, it’s good for BSS (Blind Source Separation) — aka identifying the sources of multiple microphones.
    - scikit-learn has FastICA
    - vs. PCA:
        - PCA wants each component to be gaussian, ICA wants each component to be as far from gaussian as possible
        - PCA ranks components by how much each accounts for variance (so it can be used for dimensionality reduction), but ICA does not
    - see: sci-kit learn and pg. 561 of Hastie, Tibshirani, Friedman
- how could i use this to get the filenames as output?
    - `ls -lat *venues*.csv | awk '{print $10}' | xargs head -n 1 {} | grep "state"`


2016 Sept 7
===

- when printing with css media queries, use `position: absolute` instead of `fixed`;
- scikit-learn doesn’t have a 1-sided 2-sample kolmogorov-smirnov statistic. why?


2016 Sept 6
===

- Kleene Star: `/*` or `([0-9]*)` (regex for “0” or “98765” or “”)
- BNF: describe structure formally of, say, a postal e-mail address
- strace: debug kernel-level activities (the zine from julia — jvns.ca)
- use # in css to target media queries for accessing the screen element to determine display style
