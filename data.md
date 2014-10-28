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
