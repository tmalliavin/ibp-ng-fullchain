# ibp-ng-fullchain
ibp-ng for calculation with variable stereochemistry

An extension of the ibp-ng implementation of the interval Branch-and-Prune (iBP) structure determination algorithm.

Introduction

The iBP algorithm enumerates the set of molecular structures that conform to a user-specified set of distance, angle and dihedral constraints. For a proof of principle in biomolecules, the reader is referred to:

    Worley, et al. Tuning interval Branch-and-Prune for protein structure determination. Journal of Global Optimization 2018, 72, 109–127.

    Cassioli, et al., An algorithm to enumerate all possible protein conformations verifying a set of distance constraints, BMC Bioinformatics, 2015, 16: 23.

The mathematics used to embed each atom into three-dimensional space are discussed in:

    Lavor et al., Clifford algebra and the discretizable molecular distance geometry problem, Advances in Applied Clifford Algebras, 2015, 25: 925.

A recursive description of the iBP algorithm is published in:

    Lavor et al., The interval Branch-and-Prune algorithm for the discretizable molecular distance geometry problem with inexact distances, Journal of Global Optimization, 2013, 56: 855.

The current implementation uses both breadth-first and depth-first iterative tree searches based on a multidimensional index data structure, but this may change in future versions.
Compilation

The iBP source code should be compilable on any decently modern GNU/Linux distribution. The development configuration is:

    Linux 2.6.18
    Binutils 2.17.50
    GCC 4.1.2
    Flex 2.5.4
    Bison 2.3

ibp-ng may be compiled like so:

make

The data directory contains an example (fullchain) of a run on a protein chain with variable stereochemistry. 

Licensing
This project is released under the MIT license. See the LICENSE.md file for the complete license terms.
