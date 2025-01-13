# LIGGGHTS

LIGGGHTS® - LAMMPS Improved for General Granular and Granular Heat Transfer Simulations - is a discrete element method (DEM) particle simulation software.
LIGGGHTS® is part of the [CFDEM®project](https://www.cfdem.com) and is based on the molecular dynamics simulation code [LAMMPS](https://lammps.sandia.gov/).

[![CircleCI](https://circleci.com/gh/ParticulateFlow/LIGGGHTS.svg?style=shield&circle-token=4ca67fb317cf07f8794efaa7b37438f4886d5da3)](https://circleci.com/gh/ParticulateFlow/LIGGGHTS)
[![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

## Disclaimer

> This is an adaptation of particulate flow modelling department LIGGGHTS.

## Installation

This is a short summary of how to install LIGGGHTS on Linux. A more comprehensive guide can be found in the documentation.

### Install prerequisites

```bash
sudo apt-get install build-essential cmake openmpi-bin libopenmpi-dev python-dev
```

We recommend installing LIGGGHTS to a directory named `CFDEM`, especially when used with CFDEMcoupling.

```bash
cd
mkdir -p CFDEM
cd CFDEM
```

Clone or download the LIGGGHTS source from the repository.

### Build LIGGGHTS with CMake

```bash
cd LIGGGHTS_BE
mkdir -p src-build
cd src-build
cmake ../src/
make
```

### Add an alias

You may want to create a permanent alias for the executable.

```bash
gedit ~/.bashrc &
alias liggghts='~/CFDEM/LIGGGHTS_BE/src-build/liggghts'
source ~/.bashrc
```

## License

[![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

- This software is distributed under the [GNU General Public License](https://opensource.org/licenses/GPL-2.0).
- Copyright © 2003      Sandia Corporation. Under the terms of Contract DE-AC04-94AL85000 with Sandia Corporation, the U.S. Government retains certain rights in this software.

