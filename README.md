# BIDS Extension Proposal 028: Provenance in BIDS (BEP028)
This repository contains **BIDS Extension Proposal 028 : BIDS-prov, a provenance framework for BIDS**

## Our goal
**Interpreting and comparing scientific results** and enabling reusable data and analysis output require understanding provenance, i.e. how the data were generated and processed. To be useful, the provenance must be understandable, easily communicated, and captured automatically in machine accessible form. Provenance records are thus used to encode transformations between digital objects

## Who is building BEP 028
Camille Maumet ([@cmaumet](https://github.com/cmaumet)) and Satrajit Ghosh ([@satra](https://github.com/satra)) are the BEP co-moderators. 

Rémi Adon ([@remiadon](https://github.com/remiadon)) is currently working on the definition of this BEP, as well as providing real-world examples.

### BIDS-prov in the NIDM project
The Neuroimaging Data Model (NIDM) is a collection of specification documents that define extensions the `W3C PROV` standard for the domain of human brain mapping

<p align="center">
  <img width="50%" src="img/nidm-layer-cake.png">
</p>


BIDS-prov takes effect at level 1 in the set of layers presented above. It follows semantics web practices (level 0) to allow for expression of arbitrary interactions between Agents, Entities and Activites, as defined in the W3C documentation.


## How to help
[Our goal](#our-goal) is to extends BIDS to be able to track provenance at every stage of an experiment.

For this purpose we have to **propose changes to the BIDS specification**


The BIDS specification is *rendered* as a webpage at https://bids-specification.readthedocs.io.

The website is built from a GitHub repository that consists of mostly markdown files at https://github.com/bids-standard/bids-specification.
If you don't know much about markdown, here's a [good intro guide](https://guides.github.com/features/mastering-markdown/)

The file that you are most likely to propose changes to is [src/03-modality-agnostic-files.md](https://github.com/bids-standard/bids-specification/blob/master/src/03-modality-agnostic-files.md), although there may be additional changes that have to happen in other pars of the repository

### Avoiding great big pull requests

We could do all our work in a branch of the main [bids-specification](https://github.com/bids-standard/bids-specification) repository.
We would be able to see how our proposed changes affected the current version of the specification by opening a [pull request](https://help.github.com/articles/about-pull-requests/).

However, there are quite a few changes to make, and quite a lot of conversation to have around each of them, so our proposed way of working is to **break up the individual changes into manageable chunks**.

Each conceptual update to the specification should have a *``proposal file``*.
This file should explain what change it is proposing and provide a justification for the change.

Once the proposal is ready, the developer should **open a pull request** to the master branch of the BEP028 repository (this one).
If everyone agrees on the proposal, the file will be merged to master.

(There will then be some wrangling to make the one big pull request to the bids-specification.
We'll cross that bridge when we come to it! :sparkles:)


## Finding information and getting in touch

### Google doc
The BEP028 started as a [google doc](https://docs.google.com/document/d/1vw3VNDof5cecv2PkFp7Lw_pNUTUo8-m8V4SIdtGJVKs/edit?usp=sharing)


### NIDM weekly calls
We meet every week by videoconference on Mondays at 8-9am PDT / 11am-12pm EDT / 4-5pm BST. The group is always open to new contributors interested in neuroimaging data sharing. To join the call or to ask any question, please email us at incf-nidash-nidm@googlegroups.com.  

---------------
## Additional resources
Mature building blocks of NIDM:
* [NIDM-terms](https://github.com/incf-nidash/nidm-terms)
* [NIDM-results](http://nidm.nidash.org/specs/nidm-results_130.html)


[New features (to be included)](new_features.md)
