# classical-greek-nlp-resources

# 🚧 🙏 This is currently a work in progress 🙏 🚧

This repository contains a list of publicly available resources that might come in handy while performing NLP tasks for
Classical Greek

## LSJ + derivatives

- https://archive.org/details/Lsj--LiddellScott
- https://github.com/gcelano/Thesaurus_Morphologicus_Linguae_Graecae
- https://github.com/gcelano/LSJ_additions
- https://github.com/gcelano/LSJ_GreekUnicode
- https://github.com/gcelano/lexica
- https://github.com/PerseusDL/lexica/
- http://www.perseus.tufts.edu/hopper/opensource/download

Comments on each below.

#### Plaintext LSJ

Link: https://archive.org/details/Lsj--LiddellScott

- 12M gzip, 36M unpacked.
- A single txt file, plaintext version of Greek-English LSJ.
- There's also an html version but it's essentially the same txt file within a single `<pre></pre>` block.
- Unicode, not Betacode.
- Easy to separate definitions (divided by a series of "*")
- No out-of-the-box way of parsing within a definition.
- Some entries contain extra chars such as '-', e.g. `ἀγαθο-γονία`

Snippet:

<details>
<summary>Snippet</summary>

```text
************************************************************

ἀβᾰθής, ές, (βάθος) not deep, φάλαγξ Arr.Tact.5.6; in
single rank, ἡ ἐφ’ ἑνὸς ἀ. τάξις ib.17.5, ἕλκεα
Aret.SA1.9, Gal.11.127.

2.  Geom., without depth, ἐπιφάνεια S.E.P.3.43, cf.
Simp.in Ph.572.25.

************************************************************

ἄβαθρος, ον, without foundation, Cyr.
```

</details>

