[![Build Status](https://travis-ci.org/Pyomo/pyomo.svg?branch=master)](https://travis-ci.org/Pyomo/pyomo)
[![Build status](https://ci.appveyor.com/api/projects/status/km08tbkv05ik14n9/branch/master?svg=true)](https://ci.appveyor.com/project/WilliamHart/pyomo/branch/master)
[![codecov](https://codecov.io/gh/Pyomo/pyomo/branch/master/graph/badge.svg)](https://codecov.io/gh/Pyomo/pyomo)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/Pyomo/pyomo/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/Pyomo/pyomo/?branch=master)
[![Research software impact](http://depsy.org/api/package/pypi/Pyomo/badge.svg)](http://depsy.org/package/python/Pyomo)

## Overview

The '''pyomo.aux.simplemodel''' package is software for modeling
and solving optimization problems.  This package is derived from
[Pyomo](http://www.pyomo.org), and it provides functionality that
is comparable to [PuLP](https://github.com/coin-or/pulp).  This
software is available under the BSD License.

### Description

This software defines the '''SimpleModel''' class, which illustrates
how Pyomo can be used in a simple, less object-oriented manner.
Specifically, this class mimics the modeling style supported by
PuLP.

Here is a comparison of features between PuLP and SimpleModel:
    . LP/MILP:      PuLP=YES, SimpleModel=YES
    . NLP/MILNP:    PuLP=NO,  SimpleModel=YES
    . Column-wise:  PuLP=YES, SimpleModel=NO
    . Solvers:
        CPLEX       PuLP=YES, SimpleModel=YES
        Gurobi      PuLP=YES, SimpleModel=YES
        XPRESS      PuLP=YES, SimpleModel=YES
        GLPK        PuLP=YES, SimpleModel=YES
        CBC         PuLP=YES, SimpleModel=YES
        CoinMP      PuLP=YES, SimpleModel=NO
        Ipopt       PuLP=NO,  SimpleModel=YES
        ASL         PulP=NO,  SimpleModel=YES

NOTE:  The '''SimpleModel''' class illustrates the basic steps in
formulating and solving an optimization problem, but it is not meant
to serve as a replacement for Pyomo.  Pyomo models supports a much
richer set of modeling components than simple objectives and
constraints.  In particular, the Block component supports the
expression of hierarchical models with nested structure.  The
SimpleModel class only supports a simple, flat optimization problems.

### Installation

#### PyPI [![PyPI](https://img.shields.io/pypi/v/pyomo.svg?maxAge=2592000)]() [![PyPI](https://img.shields.io/pypi/dm/pyomo.svg?maxAge=2592000)]()

    pip install pyomo.aux.simplemodel
    
#### BinStar [![Binstar Badge](https://anaconda.org/conda-forge/pyomo/badges/version.svg)](https://anaconda.org/conda-forge/pyomo) [![Binstar Badge](https://anaconda.org/conda-forge/pyomo/badges/downloads.svg)](https://anaconda.org/conda-forge/pyomo)

    conda install -c https://conda.anaconda.org/conda-forge pyomo.aux.simplemodel

### Developers

By contributing to this software project, you are agreeing to the
following terms and conditions for your contributions:

1. You agree your contributions are submitted under the BSD license. 
2. You represent you are authorized to make the contributions and grant the license. If your employer has rights to intellectual property that includes your contributions, you represent that you have received permission to make contributions and grant the required license on behalf of that employer. 
