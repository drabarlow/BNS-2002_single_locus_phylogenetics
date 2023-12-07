---
title       : "Phylogenetics and population genetics"
subtitle    : "BNS-2002: Genes, Development, and Evolution"
author      : Dr Axel Barlow
job         : "email: a.barlow@bangor.ac.uk"
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # {zenburn, tomorrow, solarized-dark, ...}
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {selfcontained, standalone, draft}
knit        : slidify::knit2slides
logo        : LA_Full_colour_reversed.svg
biglogo     : A1_FullColour.svg
assets      : {assets: ../../assets}
license     : by-nc-sa

---



<!-- adding bold and italic options -->
<style>
em {
  font-style: italic
}
strong {
  font-weight: bold;
}
</style>

## Phylogenetics and population genetics lectures

- **Key concepts and Single locus phylogenetics**
  - Theory
  - Methods
  - Discoveries
- Multi-locus phylogenetics
- Population structure
- Conservation genetics

--- 

## MEEB

**Molecular Ecology and Evolution at Bangor**

<img src="./assets/img/mb.svg" width="100%" style="display: block; margin: auto;" />

- 3rd year module "Molecular ecology and evolution"
- Dissertation and MSc projects

--- &twocol

## The link between evolution and genetics

*** =left

<img src="./assets/img/Charles_Darwin_by_Julia_Margaret_Cameron_2.jpg" width="80%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/800px-Gregor_Mendel_2.jpg" width="75%" />

---

<q>Nothing in biology makes sense, except in the light of evolution</q> (Dobzhansky 1973)

<q>Nothing in evolution makes sense, except in the light of population genetics</q> (Lynch 2007)

--- .segue .dark 

## Key concepts

---

## Your genome

- Size in base-pairs?
- Size in cm?
- Mass in picograms?
- Number autosomes?
- Number of sex chromosomes?
- Number of genes?
- % that is protein coding?
- % that is functional?

---

## Your genome

<img src="./assets/img/human_genome_dip.svg" width="90%" />

--- &twocol

## Genetic locus (plural loci)

*** =left

- Working definition: "a single position on a chromosome"
- Different variants at a locus are called **alleles**
- Difficult to determine in practise
- Simplistically a single nucleotide
- Extending beyond that depends on recombination
- Recombination results in independent evolutionary histories for unlinked loci

*** =right

<img src="./assets/img/recom.svg" width="90%" style="display: block; margin: auto;" />

--- &twocol

## Examples

*** =left

- Single copy genes/exons (at least practically)
- SNPs
- Microsatellites
- Mitochondrial DNA is a single locus
- Y chromosome (more or less) a single locus

*** =right

<img src="./assets/img/1280px-Mitochondrial_DNA_en.svg.png" width="100%" style="display: block; margin: auto;" />

--- &thirds

## Neutral evolution

*** =left

- Often people think about evolution in terms of natural selection
- What if there is no selection?
- Motoo Kimura: Neutral theory of molecular evolution, 1968
- Loci evolve by genetic drift
- Drift is determined by the population (size and gene flow)
- Basis of population genetics and phylogenetics
- "Null hypothesis" of molecular evolution

*** =right

<img src="./assets/img/Motoo_Kimura.jpg" width="90%" style="display: block; margin: auto;" />

---

## Genetic drift

<embed src="./assets/img/Practical2_handout_2023.pdf" width="100%" height="500" type="application/pdf" />

---

## Simulator

<iframe src = 'https://www.whfreeman.com/BrainHoney/Resource/6716/SitebuilderUploads/Hillis2e/Student%20Resources/Animated%20Tutorials/pol2e_at_1502_genetic_drift_simulation/pol2e_at_1502_genetic_drift_simulation.html' height='600px'></iframe>

--- .segue .dark 

## Single locus phylogenetics - theory

---

## Molecular dating of sabretooth cats

<img src="./assets/img/sabre_tree.svg" width="85%" style="display: block; margin: auto;" />

---

## Single locus tree (AKA gene tree)

- Evolutionary history of a genetic locus, represented as a tree
- (not always an actual gene)
- Can be used to infer species or population histories*
- Any recombining genome has multiple loci, each with its own gene tree
- Easy to calculate using genetic data (often sequences)

---

## Example: mitochondrial tree

<img src="./assets/img/mtDNA_tree.svg" width="80%" style="display: block; margin: auto;" />

---

## Gene tree terminology

<img src="./assets/img/term.png" width="90%" style="display: block; margin: auto;" />

--- &twocol

## Clades

*** =left

<img src="./assets/img/clade_eg.svg" width="50%" style="display: block; margin: auto;" />

*** =right

- A clade contains one ancestor and all its descendents
- It is a monophyletic group
- Modern taxonomy (generally) tries to align with clades

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort1.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort2.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort3.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort4.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort5.svg" width="100%" style="display: block; margin: auto;" />

---

## Lineage sorting summary

- Drift sorts the lineages into clades
- This takes time, we can't detect the divergence immediately
- We go through stages of complete/incomplete monophyly
- incomplete to complete lineage sorting
- lineage sorting is faster when the population size is small (= more drift)
- Mutation builds upon the clades, monophyly is retained [unless there is gene flow]
- ILS can be a real problem for inferring relationships, especially in large populaitons with recent divergence events

--- .segue .dark 

## Single locus phylogenetics - methods

--- &twocol

## PCR and Sanger sequencing

*** =left

<img src="./assets/img/abi_3130.svg" width="100%" style="display: block; margin: auto;" />

*** =right

- 700-1000 bp reads
- High accuracy
- 384 samples
- 1 day
- Dominated for 3 decades

---

## PCR and Sanger sequencing

<embed src="./assets/img/Practical2_handout_2023.pdf" width="100%" height="500" type="application/pdf" />

---

## Next generation sequencing

<img src="./assets/img/aDNA_seq.svg" width="95%" style="display: block; margin: auto;" />

---

## NGS: ancient DNA

- Fragmented ancient DNA is challenging for PCR
- NGS allows whole DNA molecules to be sequenced
- High levels of contamination
- Hybridisation capture often used
- Especially for complete mitochondrial genome sequences

<img src="./assets/img/hybr.svg" width="70%" style="display: block; margin: auto;" />

---

## NGS: metabarcoding

<img src="./assets/img/DNA_(meta)barcoding_differences.svg" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## Single locus phylogenetics - discoveries

--- &twocol

## Macrauchenia

*** =left

- Native South American mammal, in order Liptoterna
- Appeared 7 Ma
- Last species, *M. patachonica*, extinct ~10 Ka
- First collected 1834 in Argentina by Charles Darwin, on HMS Beagle. Identified as "some large animal, I fancy a Mastodon".
- Divergence time from extant mammals unknown

*** =right

<img src="./assets/img/WWB_Macrauchenia_render.webp" width="100%" style="display: block; margin: auto;" />

---

## Macrauchenia mitogenome phylogeny

<img src="./assets/img/macrauch.svg" width="100%" style="display: block; margin: auto;" />

---

## Macrauchenia mitogenome phylogeny

<embed src="./assets/img/Westbury et al. - 2017 - A mitogenomic timetree for Darwin’s enigmatic South American mammal Macrauchenia patachonica.pdf" width="100%" height="500" type="application/pdf" />

--- &twocol

## Giant beaver (*Castoroides*)

*** =left

- 2 m long, up to 125 kg, 15 cm incisors
- Extinct ~12 Ka, coinciding with arrival of Clovis people
- Several derived adapatations for wood cutting and aquatic life
- Information on evolution of "ecosystem engineers"?

*** =right

<img src="./assets/img/castoroides-size.jpg" width="85%" style="display: block; margin: auto;" />

<img src="./assets/img/Giant-beaver-fieldmuseum.jpg" width="85%" style="display: block; margin: auto;" />

---

## Giant beaver mitogenome phylogeny

<img src="./assets/img/castor_tree.svg" width="80%" style="display: block; margin: auto;" />

---

## Giant beaver mitogenome phylogeny

<embed src="./assets/img/Xenikoudakis et al. - 2020 - Ancient DNA reveals twenty million years of aquatic life in beavers.pdf" width="100%" height="500" type="application/pdf" />

--- &twocol

## Mediterranean Dwarf elephants

*** =left

- Multiple Mediterranean islands
- 1.5 to 2.3 m at shoulder
- Direct ancestor is *Palaeoloxodon antiquus*
- Example of insular dwarfism
- Phylogeny could provide information on the dwarfing rate


*** =right

<img src="./assets/img/Elephas mnaidriensis Grotta Puntali di notte.jpg" width="60%" style="display: block; margin: auto;" />

<img src="./assets/img/Palaeoloxodon_falconeri_Size_Comparison.svg.png" width="100%" style="display: block; margin: auto;" />

---

## Dwarfing rate

<img src="./assets/img/dwarf.svg" width="100%" style="display: block; margin: auto;" />

---

## Dwarfing rate

<embed src="./assets/img/Baleka et al. - 2021 - Estimating the dwarfing rate of an extinct Sicilian elephant.pdf" width="100%" height="500" type="application/pdf" />

---

## Background reading

- Any phylogenetics chapters in the course text book, especially:
- Avise (2004) Molecular markers, natural history, and evolution
- Page & Holmes (1998) Molecular evolution: a phylogenetic approach
- Papers for case studies

--- &thankyou

## Next time

**Multilocus phylogenetics**
