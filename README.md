# qstm
This repository contains the public release of QSTM, a persistent STM for byte-addressable NVM.

## Building
Compile ralloc by running make libralloc.a in ralloc/test and then run 'make' in qstm/qstm

## Running
To run STAMP Vacation:
./bin/main -T2 -dcont=0 -t[number of threads]

To run STAMP Intruder:
./bin/main -T3 -dcont=0 -t[number of threads]

## Configuration
qstm/config.hpp contains several configuration options including Bloom filter size and persistence operations.
