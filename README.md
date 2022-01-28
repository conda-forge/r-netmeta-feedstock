About r-netmeta
===============

Home: https://github.com/guido-s/netmeta https://link.springer.com/book/10.1007/978-3-319-21416-0

Package license: GPL-2.0-or-later

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-netmeta-feedstock/blob/master/LICENSE.txt)

Summary: A comprehensive set of functions providing frequentist methods for network meta-analysis and supporting Schwarzer et al. (2015) <DOI:10.1007/978-3-319-21416-0>, Chapter 8 "Network Meta-Analysis": - frequentist network meta-analysis following Rücker (2012) <DOI:10.1002/jrsm.1058>; - net heat plot and design-based decomposition of Cochran's Q according to Krahn et al. (2013) <DOI:10.1186/1471-2288-13-35>; - measures characterizing the flow of evidence between two treatments by König et al. (2013) <DOI:10.1002/sim.6001>; - ranking of treatments (frequentist analogue of SUCRA) according to Rücker & Schwarzer (2015) <DOI:10.1186/s12874-015-0060-8>; - partial order of treatment rankings ('poset') and Hasse diagram for 'poset' (Carlsen & Bruggemann, 2014) <DOI:10.1002/cem.2569>; (Rücker & Schwarzer, 2017) <DOI:10.1002/jrsm.1270>; - split direct and indirect evidence to check consistency (Dias et al., 2010) <DOI:10.1002/sim.3767>, (Efthimiou et al., 2019) <DOI:10.1002/sim.8158>; - league table with network meta-analysis results; - additive network meta-analysis for combinations of treatments (Rücker et al., 2020) <DOI:10.1002/bimj.201800167>; - network meta-analysis of binary data using the Mantel-Haenszel or non-central hypergeometric distribution method (Efthimiou et al., 2019) <DOI:10.1002/sim.8158>; - 'comparison-adjusted' funnel plot (Chaimani & Salanti, 2012) <DOI:10.1002/jrsm.57>; - automated drawing of network graphs described in Rücker & Schwarzer (2016) <DOI:10.1002/jrsm.1143>; - rankograms and ranking by SUCRA; - contribution matrix as described in Papakonstantinou et al. (2018) <DOI:10.12688/f1000research.14770.3> and Davies et al. (2021) <arXiv:2107.02886>.

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15163&branchName=master">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-netmeta-feedstock?branchName=master">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--netmeta-green.svg)](https://anaconda.org/conda-forge/r-netmeta) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-netmeta.svg)](https://anaconda.org/conda-forge/r-netmeta) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-netmeta.svg)](https://anaconda.org/conda-forge/r-netmeta) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-netmeta.svg)](https://anaconda.org/conda-forge/r-netmeta) |

Installing r-netmeta
====================

Installing `r-netmeta` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-netmeta` can be installed with:

```
conda install r-netmeta
```

It is possible to list all of the versions of `r-netmeta` available on your platform with:

```
conda search r-netmeta --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-netmeta-feedstock
============================

If you would like to improve the r-netmeta recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-netmeta-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/conda-forge/r/)
* [@nsandau](https://github.com/nsandau/)

