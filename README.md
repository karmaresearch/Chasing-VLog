# Chasing VLog

This directory contains some datasets for __VLog__ exercising the chase procedure, and, on installation,
installs some more. Installing this package allows one to run chases on either __VLog__ or __RDFox__, on
either MacOS or Linux.

## Installation instructions

Installation is quite simple:

```
sh setup
```

should do the trick.
This will get the chasebench repository and unzip its data files.
It will also get and install VLog.
Now you are ready to run either VLog or RDFox on these data sets.

## Running VLog or RDFox

There are scripts _run-vlog_ and _run-rdfox_. Names are self-explanatory.
These scripts take two parameters:
the first one describes the chase type, either __restricted__ or __skolem__,
the second one contains a dataset name.
For each dataset, the directory _params-datasets_ contains a file, whose name represents the dataset.
For instance,

```
sh run-vlog skolem LUBM-001
```

will run vlog, skolem chase, on the LUBM-001 dataset.
Output will appear on a file _vlog-LUBM-001.skolem.out_.
In addition, a summary will be printed on standard output: program used (VLog or RDFox), the chase type, the dataset, the date, what kind of processor, the runtime of the chase itself, the memory used, and the number of derivations.

## Notes

During setup, the chasebench repository is downloaded. It is available from
https://github.com/dbunibas/chasebench.git.
It is described in:
_Michael Benedikt, George Konstantinidis, Giansalvatore Mecca, Boris Motik, Paolo Papotti, Donatello Santoro, and Efthymia Tsamoura. 2017. Benchmarking the Chase. In Proceedings of the 36th ACM SIGMOD-SIGACT-SIGAI Symposium on Principles of Database Systems (PODS '17). ACM, New York, NY, USA, 37-52._ DOI: https://doi.org/10.1145/3034786.3034796

VLog is available from https://github.com/karmaresearch/vlog.git.

The original database for Uniprot is available from http://www.uniprot.org. Reactome is available from http://reactome.org.
