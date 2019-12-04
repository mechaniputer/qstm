# qstm
This repository contains the public release of QSTM, a persistent STM for byte-addressable NVM.

## Building
Compile ralloc by running make libralloc.a in ralloc/test and then run 'make' in qstm/qstm

## Running
Note: You should always delete the files created in /dev/shm prior to rerunning these tests, as these STAMP benchmarks are not real persistent applications and do not know how to reuse an old persistent segment.

To run STAMP Vacation:
./bin/main -T2 -dcont=0 -t[number of threads]

To run STAMP Intruder:
./bin/main -T3 -dcont=0 -t[number of threads]

## Configuration
qstm/config.hpp contains several configuration options including Bloom filter size and persistence operations.

## Misc/TODO
At some point I plan to add several microbenchmarks to this repo as well but this will require additional cleanup.
