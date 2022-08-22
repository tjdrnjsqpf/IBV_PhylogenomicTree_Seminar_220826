---
## 01 Multiple sequence alignment

mafft   	--auto	   --thread	20	   sequence.fa  >  sequence.fa.mafft

---

## 02 Alignment / site filtering

trimal	   -automated1	  -in	  sequence.fa.mafft 	   -out	   sequence.fa.mafft.trimAl

---

## 03 Concatenation

phyutility      -concat    -in     *.trimAl       -out      IBV.supermatrix

---

## 04 Format change

readal      -in     IBV.supermatrix   -out    IBV.supermatrix.phy   -phylip

---

## 05 Phylogenomic tree reconstruction

iqtree    -s   IBV.supermatrix.phy   -m  MFP   -bb  1000   -nt  AUTO
