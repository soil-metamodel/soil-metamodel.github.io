---
layout: page
title: "Data"
description: "How to format and contribute data"
group: navigation
---
{% include JB/setup %}


### Where to put data

Add a new folder to the [decomposition\_datasets](https://github.com/soil-metamodel/decomposition_datasets) repository. Add a README file with dataset description, meta-data (variable names and units), and citation if applicable.

### Variable names and units

The key feature with variable names is to use terminology that makes it easy to cross-reference equations.

The most important reason to standardize names and units is to make it easier to program against.


| variable | units | definition |
|:----|:----:|:----|
| `time` | days | |
| `temperature` | C | |
| `moisture` | g/g | mass fraction of water |
| `c` | g | total mass of carbon |
| `dc_dt` | g/d | rate of change of total carbon pool |
| `c_<fraction>` | g | total mass of a fraction (e.g. 'light', 'cellulose', etc)|
| `n` | g | total mass of nitrogen |
| `n_percent` | g/g | mass percent nitrogen |
|-----

These are just a start, please suggest updates and changes in [a new issue in github](https://github.com/soil-metamodel/soil-metamodel.github.com/issues/new).

### Archiving Data: 

It would be a great idea to archive your data so that it can be accessed programatically - within and beyond the scope of the workshop.

 * First, use standard variable names above.
 * Then use [DataUp](https://web.dataup.org/) web interface, DataUp will guide you through creating metadata and uploading to OneShare, which is a DataOne membernode
 * Post your dataset on the Data Wiki page

## Available Datasets

For the purposes of the workshop, we have chosen to focus on microcosm and litterbag studies. By excluding the 'input' term for a carbon models, and by having relatively controlled substrate, these should enable development and testing of new approaches.

###  In the [decomposition\_datasets](https://github.com/soil-metamodel/decomposition_datasets) repository.

* LeBauer, D. S. (2010). Litter degradation rate and β-glucosidase activity increase with fungal diversity. Canadian journal of forest research, 40(6), 1076-1085. 
([pdf](https://github.com/soil-metamodel/decomposition_datasets/blob/master/lebauer_2010_micrcosm/lebauer2010ldr.pdf?raw=true))

* Powers, J. S., et al. (2009). Decomposition in tropical forests: a pan‐tropical study of the effects of litter type, litter placement and mesofaunal exclusion across a precipitation gradient. Journal of Ecology, 97(4), 801-811. ([pdf](https://github.com/soil-metamodel/decomposition_datasets/blob/master/powers_2009_litterbags/powers2009%20J%20Ecology.pdf?raw=true))

###  Publicly available, not yet placed in GitHub

* LIDET
* ... list yours here
