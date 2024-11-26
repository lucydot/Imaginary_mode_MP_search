# Searching the Materials Project for Imaginary Phonon Modes

This repository contains the lab notebooks used to search and analyse the [Materials Project](https://next-gen.materialsproject.org/) for structures with imaginary phonon modes. 
The notebooks make heavy use of the [Materials Project API](https://next-gen.materialsproject.org/api).

The result is 153 structures listed in `Analysis_two.ipynb`.

Each of these structures also meets the following criteria:

- contains five or more atoms in the primitive cell, as we are targeting complex materials for thermoelectric applications
- it is marked as experimentally observed on the [ICSD](https://www.psds.ac.uk/icsd), as we want materials which are synthesisable
- it is the lowest energy structure on Materials Project, to exclude structures with known lower energy polymorphs
- the imaginary mode has a frequency $<-0.25$ THz, to exclude imaginary modes as a result of noise / numerical limitations
- the imaginary mode is at a high symmetry point in reciprocal space


