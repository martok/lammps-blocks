LAMMPS Building Blocks
======================

About
-----
A collection of input files for [LAMMPS](http://lammps.sandia.gov/), modularized
as much as possible to allow for easy setup of new simulations.

Maintained by [Sebastian Hütter](mailto:sebastian.huetter@st.ovgu.de).


Structure
---------
Since LAMMPS does not support search paths, all files are located in one flat directory.
Instead of using subfolders, they follow a namespace-style naming scheme. For easier
access in job scripts, it is recommended to either clone this repository to a subdirectory
of your work folder, or create a symlink to a working copy shared between multiple
simulations. For instance, if this repository is accessible in a subdirectory called
`blocks`, one might call up a potential as follows:

    include    blocks/potential.feal.lmp


Groups
------

* lattice: general lattice setup
* utl: utilities, not operation-specific
* atoms: modify atoms in simulation box
* potential: potentials for various uses with correct `pair_style` etc.
* mm: molecular mechanics (T=0K simulations)
* md: molecular dynamics (T>0K simulations)



License
=======
```
Copyright (c) 2014-15, Sebastian Hütter (sebastian.huetter@st.ovgu.de)
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```