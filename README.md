# IBV_PhylogenomicTree_Seminar_220826


### Mafft download 
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


make clean

make

make install
