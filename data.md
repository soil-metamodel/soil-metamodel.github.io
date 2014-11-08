---
layout: page
title: "Data"
description: "How to format and contribute data"
group: navigation
---
{% include JB/setup %}

[edit this page](https://github.com/soil-metamodel/soil-metamodel.github.com/edit/master/data.md)


### Datasets

In defining the scope of the workshop, we have chosen to focus on microcosm and litterbag studies. By excluding the 'input' term for a carbon models, and by having less diverse substrate (in the case of litter), these should enable development and testing of new approaches. This will place emphasis on decomposition rather than plant productivity. 

* Microcosm data in the SoilR package (`data(eCO2)`)
* Microcosm data from a experimenatal test of litter type x species number effects on decomposition rate (LeBauer 2010)
* Litter data from LIDET - an outstanding cross-site evaluation of litter decomposition that has been widely used in modeling
* Litter data from a Tropical cross site study (Powers et al 2009).
* Litter data from Charlotte Riggs (unpublished)

### Variable names and units

The key feature with variable names is to use terminology that makes it easy to cross-reference equations.

The most important reason to standardize names and units is to make it easier to program against.


| variable | units | definition |
|:----|:----:|:----|
| `time` | days | |
| `temperature` | C | |
| `moisture` | g/g | mass fraction of water |
| `c` | g | total mass of carbon |
| `eCO2` | | cumulative evolved CO2 (for microcosm studies)|
| `dc_dt` | g/d | rate of change of total carbon pool |
| `c_<fraction>` | g | total mass of a fraction (e.g. 'light', 'cellulose', etc)|
| `n` | g | total mass of nitrogen |
| `n_percent` | g/g | mass percent nitrogen |
|-----

These are just a start, please suggest updates and changes in [a new issue in github](https://github.com/soil-metamodel/soil-metamodel.github.com/issues/new).

### Where to put data

Add a new folder to the [decomposition\_datasets](https://github.com/soil-metamodel/decomposition_datasets) repository. Add a README file with a license, dataset description, meta-data (variable names and units), and citation if applicable. Ideally, an exploratory / demonstration with the dataset.

A CC-BY license allows reuse with attribution. See [Creative Commons Licenses](http://creativecommons.org/licenses/) for more details about this and other alternative licenses for open data.

#### Archiving Data: 

**Extra Credit:** Archive your data so that it can be accessed programatically - within and beyond the scope of the workshop.

 * First, use standard variable names above.
 * Then use Dash to upload your data, either to the [DataOne Dash](https://oneshare.cdlib.org/xtf/search) instance or for UC affiliates to one of the [UC campus Dash sites](http://www.cdlib.org/cdlinfo/2014/11/03/announcing-the-dash-tool-data-sharing-made-easy/). The web interface guides you through creating metadata and uploading to OneShare, which is a DataOne membernode
 * Create a folder in the decomposition\_datasets repository with information about the dataset as above
