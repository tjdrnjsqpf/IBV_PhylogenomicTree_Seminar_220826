# IBV_PhylogenomicTree_Seminar_220826


## 01 Mafft download 
https://mafft.cbrc.jp/alignment/software/source.html


wget https://mafft.cbrc.jp/alignment/software/mafft-7.505-with-extensions-src.tgz

tar -xf mafft-7.505-with-extensions-src.tgz

cd mafft-7.505-with-extensions

cd core

vi Makefile

---------------------------
From:

PREFIX = /usr/local

To:

PREFIX = /home/your_home/somewhere (must be absolute path)

---------------------------

---------------------------
From:

BINDIR = $(PREFIX)/bin

To:

BINDIR = /home/your_home/bin (or elsewhere in your command-search path)

---------------------------

make clean

make

make install


cd 

vi .profile

---

[Write] 

export PATH="$PATH:/home/lsg/lsg/bin"

ESC + : + wq

---
source .profile

---

## 02 trimAl download

wget http://trimal.cgenomics.org/_media/trimal.v1.2rev59.tar.gz

tar -xf trimal.v1.2rev59.tar.gz

cd trimAl

cd source

make

---

## 03 phyutility download

wget https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/phyutility/phyutility_2_2_6.tar.gz

tar -xf phyutility_2_2_6.tar.gz

cd phyutility

./phyutility


---


## 04 iqTree download

wget https://github.com/Cibiv/IQ-TREE/releases/download/v1.6.12/iqtree-1.6.12-Linux.tar.gz

tar -xf iqtree-1.6.12-Linux.tar.gz 

cd iqtree-1.6.12-Linux

cd bin

./iqtree







