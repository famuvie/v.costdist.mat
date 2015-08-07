[![DOI](https://zenodo.org/badge/4357/famuvie/v.costdist.mat.svg)](https://zenodo.org/badge/latestdoi/4357/famuvie/v.costdist.mat)

![GRASS logo](http://grass.osgeo.org/uploads/images/logo/grass.smlogo.gif)

* * * * *

`v.costdist.mat` is a [GRASS](http://grass.osgeo.org/) script (i.e., a bash script to be executed under a GRASS console, or from a GRASS GUI) for computing cost-based distance matrices.

Uses GRASS' `r.cost` iteratively to compute minimum-cost distances between two or more sets of points.


NAME
----

***v.costdist.mat*** - Cost-based distances between points

KEYWORDS
--------

SYNOPSIS
--------

**v.costdist.mat**\

**v.costdist.mat help**\

**v.costdist.mat** [-**k**] **from**=*filename* **to**=*filename*[,*filename*,...] **cost**=*filename* [--**verbose**]
[--**quiet**]

### Flags:

**-k**
:   Use the 'Knight's move'. Forwarded to r.cost (see r.cost).

**--verbose**
:   Verbose module output

**--quiet**
:   Quiet module output

### Parameters:

**from**=*filename*
:   Name of existing vector points map

**to**=*filename[,*filename*,...]*
:   Name(s) of existing vector points map(s) where cost-distances to
    "from" points are to be stored

**cost**=*filename*
:   Name of existing raster file containing cost information

