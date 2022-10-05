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

#### Perseus LSJ - https://github.com/gcelano/lexica

- Perseus export of LSJ.
- XML. Well structured.
- Betacode.
- 40M zip-compressed, 345M unpacked.

<details>
<summary>Snippet</summary>

```xml

<entryFree id="n92041"
           key="r(abdouxe/w"
           type="main"
           opt="n"
           TEIform="entryFree">
    <orth extent="full" lang="greek" opt="n" TEIform="orth">r(abdoux-e/w</orth>,
    <sense id="n92041.0" n="A" level="1" opt="n" TEIform="sense">
        <tr opt="n" TEIform="tr">to be a</tr>
        <foreign lang="greek" TEIform="foreign">r(abdou=xos</foreign>, <tr opt="n" TEIform="tr">carry a rod</tr> or <tr
            opt="n" TEIform="tr">wand</tr>, esp. as a badge
        <pb n="1563" TEIform="pb"/>
        of office,
        <bibl default="NO" TEIform="bibl">
            <author TEIform="author">Hippias Erythr.</author>
        </bibl>
        ap.
        <bibl n="urn:cts:greekLit:tlg0008.tlg001.perseus-grc1:6:259d"
              default="NO"
              TEIform="bibl">
            <author TEIform="author">Ath.</author>
            <biblScope TEIform="biblScope">6.259d</biblScope>
        </bibl>
        ; of the Roman lictors, <tr opt="n" TEIform="tr">bear the fasces</tr>,
        <bibl n="urn:cts:greekLit:tlg0385.tlg001:48:43"
              default="NO"
              TEIform="bibl">
            <author TEIform="author">D.C.</author>
            <biblScope TEIform="biblScope">48.43</biblScope>
        </bibl>
        :—
        <gramGrp opt="n" TEIform="gramGrp">
            <gram type="voice" opt="n" TEIform="gram">Pass.</gram>
        </gramGrp>
        , <tr opt="n" TEIform="tr">have the fasces borne before one</tr>,
        <bibl n="urn:cts:greekLit:tlg0007.tlg005:10" default="NO" TEIform="bibl">
            <author TEIform="author">Plu.</author>
            <title TEIform="title">Num.</title>
            <biblScope TEIform="biblScope">10</biblScope>
        </bibl>
        .
    </sense>
</entryFree>
```

</details>

#### Unicode Perseus LSJ - https://github.com/gcelano/LSJ_GreekUnicode

- ^, but converted to Unicode.
- 26M zip-compressed, 228M unpacked.

<details>

<summary>Snippet</summary>

```xml

<entryFree id="n92041" key="ῥαβδουχέω" type="main" opt="n" TEIform="entryFree">
    <orth extent="full" lang="greek" opt="n" TEIform="orth">ῥαβδουχ-έω</orth>,
    <sense id="n92041.0" n="A" level="1" opt="n" TEIform="sense">
        <tr opt="n" TEIform="tr">to be a</tr>
        <foreign lang="greek" TEIform="foreign">ῥαβδοῦχος</foreign>,<tr opt="n" TEIform="tr">carry a rod</tr>or<tr
            opt="n" TEIform="tr">wand</tr>, esp. as a badge<pb n="1563" TEIform="pb"/>of office,
        <bibl default="NO" TEIform="bibl">
            <author TEIform="author">Hippias Erythr.</author>
        </bibl>
        ap.
        <bibl n="urn:cts:greekLit:tlg0008.tlg001.perseus-grc1:6:259d" default="NO" TEIform="bibl">
            <author TEIform="author">Ath.</author>
            <biblScope TEIform="biblScope">6.259d</biblScope>
        </bibl>
        ; of the Roman lictors,<tr opt="n" TEIform="tr">bear the fasces</tr>,
        <bibl n="urn:cts:greekLit:tlg0385.tlg001:48:43" default="NO" TEIform="bibl">
            <author TEIform="author">D.C.</author>
            <biblScope TEIform="biblScope">48.43</biblScope>
        </bibl>
        :—
        <gramGrp opt="n" TEIform="gramGrp">
            <gram type="voice" opt="n" TEIform="gram">Pass.</gram>
        </gramGrp>
        ,<tr opt="n" TEIform="tr">have the fasces borne before one</tr>,
        <bibl n="urn:cts:greekLit:tlg0007.tlg005:10" default="NO" TEIform="bibl">
            <author TEIform="author">Plu.</author>
            <title TEIform="title">Num.</title>
            <biblScope TEIform="biblScope">10</biblScope>
        </bibl>
        .
    </sense>
</entryFree>
```

</details>

#### Unicode Perseus LSJ + 2 extra tags - https://github.com/gcelano/LSJ_additions

- 27M zip-compressed, 233M unpacked.

- The extra tags are:
    - key2 = value of @key without U+0308 U+0304 U+0306,
    - key3 = value of @key without accents

<details>

<summary>Snippet</summary>

```xml

<entryFree key2="ῥαβδουχέω" key3="ραβδουχεω" id="n92041" key="ῥαβδουχέω" type="main" opt="n" TEIform="entryFree">
    <orth extent="full" lang="greek" opt="n" TEIform="orth">ῥαβδουχ-έω</orth>,
    <sense id="n92041.0" n="A" level="1" opt="n" TEIform="sense">
        <tr opt="n" TEIform="tr">to be a</tr>
        <foreign lang="greek" TEIform="foreign">ῥαβδοῦχος</foreign>,<tr opt="n" TEIform="tr">carry a rod</tr>or<tr
            opt="n" TEIform="tr">wand</tr>, esp. as a badge<pb n="1563" TEIform="pb"/>of office,
        <bibl default="NO" TEIform="bibl">
            <author TEIform="author">Hippias Erythr.</author>
        </bibl>
        ap.
        <bibl n="urn:cts:greekLit:tlg0008.tlg001.perseus-grc1:6:259d" default="NO" TEIform="bibl">
            <author TEIform="author">Ath.</author>
            <biblScope TEIform="biblScope">6.259d</biblScope>
        </bibl>
        ; of the Roman lictors,<tr opt="n" TEIform="tr">bear the fasces</tr>,
        <bibl n="urn:cts:greekLit:tlg0385.tlg001:48:43" default="NO" TEIform="bibl">
            <author TEIform="author">D.C.</author>
            <biblScope TEIform="biblScope">48.43</biblScope>
        </bibl>
        :—
        <gramGrp opt="n" TEIform="gramGrp">
            <gram type="voice" opt="n" TEIform="gram">Pass.</gram>
        </gramGrp>
        ,<tr opt="n" TEIform="tr">have the fasces borne before one</tr>,
        <bibl n="urn:cts:greekLit:tlg0007.tlg005:10" default="NO" TEIform="bibl">
            <author TEIform="author">Plu.</author>
            <title TEIform="title">Num.</title>
            <biblScope TEIform="biblScope">10</biblScope>
        </bibl>
        .
    </sense>
</entryFree>
```

</details>
