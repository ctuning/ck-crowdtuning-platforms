[![logo](https://github.com/ctuning/ck-guide-images/blob/master/logo-powered-by-ck.png)](http://cKnowledge.org)
[![logo](https://github.com/ctuning/ck-guide-images/blob/master/logo-validated-by-the-community-simple.png)](http://cTuning.org)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)

This repository contains JSON meta information in the [open CK format](http://github.com/ctuning/ck)
about platforms participating in CK-powered experiment crowdsourcing across diverse
hardware provided by volunteers. For example, it is used to crowdsource performance
analysis and optimization of realistic workloads across mobile devices and IoT. 

Entries are first automatically created at cknowledge.org/repo ,
then synced with this repository. More importantly, they can be 
manually updated by the community to add important
properties (such as platform topology, info about caches, etc)
or scripts to set frequency, etc useful for collaborative and
reproducible research scenarios!

The community also provides notes about setting up various hardware
using this [wiki](https://github.com/ctuning/ck-crowdtuning-platforms/wiki).

Contributors
=======
* [Grigori Fursin](http://fursin.net/research.html), cTuning foundation/dividiti
* [Anton Lokhmotov](https://www.hipeac.net/~anton), dividiti
* [Flavio Vella](http://dividiti.com), dividiti
* The community participated in the [CK-powered experiment crowdsourcing](http://cKnowledge.org/repo)

Prerequisites
=============
* Collective Knowledge Framework: http://github.com/ctuning/ck

Installation
============

```
 > ck pull repo:ck-crowdtuning-platforms

 > ck list platform --print_name | sort
 > ck list platform.cpu --print_name | sort
 > ck list platform.gpgpu --print_name | sort
 > ck list platform.gpu --print_name | sort
 > ck list platform.nn --print_name | sort
 > ck list platform.npu --print_name | sort
 > ck list platform.os --print_name  | sort

 > ck load platform.cpu:40bc4c800b3f8e3d --min
 > ck load platform.cpu:40bc4c800b3f8e3d
 > ck info platform.cpu:40bc4c800b3f8e3d

```

Publications
============

```
@inproceedings{cm:29db2248aba45e59:cd11e3a188574d80,
    title = {{Collective Mind, Part II}: Towards Performance- and Cost-Aware Software Engineering as a Natural Science},
    author = {Fursin, Grigori and Memon, Abdul and Guillon, Christophe and Lokhmotov, Anton},
    booktitle = {18th International Workshop on Compilers for Parallel Computing (CPC'15)},
    year = {2015},
    url = {https://arxiv.org/abs/1506.06256},
    month = {January}
}
```

```
@inproceedings{ck-date16,
    title = {{Collective Knowledge}: towards {R\&D} sustainability},
    author = {Fursin, Grigori and Lokhmotov, Anton and Plowman, Ed},
    booktitle = {Proceedings of the Conference on Design, Automation and Test in Europe (DATE'16)},
    year = {2016},
    month = {March},
    url = {https://www.researchgate.net/publication/304010295_Collective_Knowledge_Towards_RD_Sustainability}
}
```

The concepts have been described in the following publications:

* http://tinyurl.com/zyupd5v (DATE'16)
* http://arxiv.org/abs/1506.06256 (CPC'15)
* http://hal.inria.fr/hal-01054763 (Journal of Scientific Programming'14)
* https://hal.inria.fr/inria-00436029 (GCC Summit'09)

Public results
==============

Public benchmarking and optimization results are continuously
aggregated in the [live CK repository](http://cKnowledge.org/repo)

Public discussions
==================
* [CK mailing list](http://groups.google.com/group/collective-knowledge)
