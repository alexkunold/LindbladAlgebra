# LindbladAlgebra
Mathematica notebooks implementing the algebraic formulation of the Lindblad equation for finite-dimensional open quantum systems.

## Authors
Leonel Bixano,
Guillermo López-Alvarez,
Victor Alberto Cruz-Barriguete,
Victor Guadalupe Ibarra-Sierra,
José Luis Cardoso,
Juan Carlos Sandoval-Santana,
Alejandro Kunold

## Abstract
This repository contains a Mathematica notebook accompanying the paper Algebraic Structures of the Lindblad Equation. The notebook illustrates the proposed algebraic formulation through one-, two-, and three-qubit examples that verify the derived relations and compare the algebraic and direct methods. An additional example describes a driven four-level transmon, demonstrating an approximate \(X\) gate and the associated population leakage beyond the computational subspace.
The examples provide a step-by-step implementation of the algebraic method, beginning with the construction of the Hermitian operator basis and the associated algebraic objects. The model-dependent quantities are then assembled to obtain the Liouville superoperator and the corresponding differential equations. Their agreement with the results obtained using the direct method is explicitly verified.
The repository also includes the benchmarking notebooks benchmark-timing and benchmark-memory, which compare execution times and memory requirements, respectively, for preprocessing and constructing the Liouville superoperator and the dynamical-map equations. These comparisons assess the implementations and cases tested; they do not establish a general computational advantage over optimized sparse methods.
The code is parameterized by the number of qubits, allowing systematic extension to larger Hilbert spaces, subject to computational resource limitations. Although some symbolic calculations become demanding as the system size increases, the implementation provides a framework that can be adapted to other finite-dimensional open quantum systems.

## Licence

LindbladAlgebra Mathematica examples accompanying the paper

"The Algebraic Structure of the Lindblad Equation"

Copyright (c) 2026 Alejandro Kunold and collaborators

This notebook is distributed under the MIT License. Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the conditions of the MIT License.

A copy of the full license is available in the LICENSE file of this repository.
