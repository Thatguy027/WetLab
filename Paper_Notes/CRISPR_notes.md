# Co-CRISPR Strategy for Efficient Genome Editing in Caenorhabditis elegans

[Here is the paper](http://www.genetics.org/content/197/4/1069.long)

## Goal of paper is to streamline CRISPR/Cas9 mediated genome editing

#### First used _rol-6_ as coinjection marker to to mediate mutation in _pie-1_
  1. _rol-6_ has a dominant rolling phenotype
  1. 5/93 F1 rollers produced maternal embryonic lethality (homozygous)
  2. 17/93 were heterozygous
      * likely due to Cas9 targeting of one parental allele.

_Found half of sgRNAs to not be effective_
  * Decided to use known sgRNAs that work well

#### Use sgRNA that targets _unc-22_ as co-CRISPR

##### Setup
  1. _unc-22_ gives a visible twitching phenotype
  2. attempt to target _avr-14_ _avr-15_ with sgRNAs known to work.
  3. included _rol-6_ as dominant coinjection marker
##### Results
    Selecting for both twitchers and rollers greatly increased the occurence of _avr-14_ and _avr-15_ deletions


#### Next attempt to do homologous recombination

_found it necessary to alter sgRNA target sequence in the donor DNA when trying to introduce point mutations or epitope tagging by mutating the PAM region or by introducing mismathes in the seed region (target recognition seq?)_

**want to avoid recutting**

##### Setup
  1. attempt to introduce GFP at _pie-1_
  2. plasmid contains the following:
      * used 1kb homology arms
      * silent mutation at PAM that disrupts the ssequence
  3. generated 3 plasmids
      * _pie-1-GFP_ **WT**
      * _pie-1-GFP_ **K88A**
      * _pie-1-GFP_ **K68R**
  4. each donor plasmid was injected with vectors to express:
      * sgRNA
      * Cas9
      * _rol-6_
##### Results
9/92 wt pie
1/69 K88
1/72 K68
Only tested F1 rollers
Each of the GFP positive strains were heterozygotes

#### Homologous recombination with coCRISPR
##### Setup
  1. _unc-22_
  2. attempt to tag _vet-2 pie-1 smo-1_ with gfp
  3. ID F1 rollers and F2 twitchers and tested for HR

#### Selection/Counter Selection based screening methods
save cost associated with sequencing
##### Setup
  1. _unc-119_ in combination with new BSD worm antibiotic as selectable marker
  2. _avr-15(+)_ plasmid acts as counter selection. This is used to remove _Cbr-unc-119(+)_ or BSD(+) extrachromosomal arrays
  3. sgRNA
  4. need to start with ivermectin resistant animals

##### Summary
Utilization of coCRISPR can decrease screening time required for identification of CRISPR events of interest. This didn't seem to have as pronounced an effect in the HR, though there was still improvement. IDentifying HR events works Selection/counterselection methods. **I am not sure what the counterselection is for - is it just to drop the extrachromosomal array when you no longer need it?** _Things to keep in mind_ There needs to be optimization of donor plasmid when performing HR with CRISPR. **Need** to mutate the PAM site or introduce mismatches on your target sequence when perfect.

# Heritable/conditional genome editing in C. elegans using a CRISPR-Cas9 feeding system

[Here is the paper](http://www.nature.com/cr/journal/v24/n7/full/cr201473a.html)
