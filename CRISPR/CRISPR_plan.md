## Starting off CRISPR

**11/10/14**

1. Confirm plasmid sequences(**pECA061,060,059,058,057**)
  * ALl of the above plasmids were generated by Bryn using the Goldstein plasmid _pDD162_
  * Use **GGTGTGAAATACCGCACAGA** to verify sequences
    * Bryn made some primers for checking as well
      * F - oECA486
      * R - oECA484

2. Make sure there is enough co-injection plasmid
  * pECA43 - pBCN27-Pmyo-2::GFP::unc-54_3‘UTR
  * pECA49 - pDD04neo pmyo2::gfp

3. Inject worms in order to visualize GFP in F1


## While figuring out the above

1. Making new sgRNA plasmid constructs (2 options)
  * **A:** Use sgRNA vector from Calarco lab (this is method for coCRISPR)
    * Primers : **oECA547** & **oECA553**
  * **B:** Use sgRNA-Cas9 vector from Goldstein lab
    * Forward primer  5’-(N19-25)GTTTTAGAGCTAGAAATAGCAAGT-3’
    * Reverse Primer 5’-CAAGACATCTCGCAATAGG-3’
    * **NOTE** This doesn't seem to be the recommended protocol on the [NEB Q5 protocol](https://www.neb.com/products/e0554-q5-site-directed-mutagenesis-kit)
      * They suggest using primers with two tail for large insertions. However, Bryn and the Goldstein lab apparently got it working using only one primer with a tail containing the sgRNA


#### Summary of A - Calarco / Church / coCRISPR method

Things to include in injection:
1. Cas9 (**pECA51** - Peft-3::cas9-SV40_NLS::tbb-2 3'UTR) [from paper](http://www.nature.com/nmeth/journal/v10/n8/full/nmeth.2532.html)
2. co-injection marker (pECA43 or pECA49 (?))
3. Target sgRNA plasmid (we make)
4. coCRISPR target (_unc-22, ben-1, GFP_)

***constructs 3-4 can be derived from pECA52***

pECA52 - PU6::unc-119_sgRNA

Use Q5 kit to generate these plasmids

**FOR EXAMPLE** (from Bryn)

The below primers were used to generate an sgRNA plasmid that targets GFP (**pECA069**)

The forward primer seems to have the **PAM** site in it which is **NOT** recommended when designing target sequences of the sgRNA. Apparently Mostafa says it is cool because the second G starts the "universal" scaffold RNA

Fwd primer:

oECA548 5' - GGGCGAGGAGCTGTTCAC **CGG** TTTTAGAGCTAGAAATAGCAAGT - 3'

Reverse primer:

oECA547 5' - AAACATTTAGATTTGCAATT - 3'

#### Summary of B - Goldstein Method

1. Cas9 - sgRNA plasmid
  * if we go this route we should use coCRISPR sgRNA on the Cas9 plasmid
2. co-injection marker (pECA43 or pECA49 (?))
3. Target sgRNA plasmid (we make)


Figure 2 from [coCRISPR Paper:](http://www.genetics.org/content/197/4/1069.long)

![alt text](http://www.genetics.org/content/197/4/1069/F2.large.jpg)

#### sgRNA structure

From [PAPER](http://www.nature.com/nprot/journal/v8/n11/full/nprot.2013.132.html)

![alt text](http://www.nature.com/nprot/journal/v8/n11/images/nprot.2013.132-F3.jpg)
