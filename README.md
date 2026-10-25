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
This repository contains the Mathematica notebook accompanying the paper Algebraic Structures of the Lindblad Equation. It provides a step-by-step implementation of the algebraic formulation, from the construction of orthonormal Hermitian operator bases and their structure constants to the Liouville superoperator and the differential equations governing the dynamical map.

The notebook contains five worked examples. Examples 1, 3, and 5 verify the main algebraic relations for one-, two-, and three-qubit operator bases. Examples 2 and 4 numerically solve the evolution equations for transmon models, construct the dynamical map, and plot the energy-level populations. An additional application illustrates the implementation of an approximate X gate.

The numerical examples also construct the unnormalized Choi matrix to check Hermiticity preservation, complete positivity, and trace preservation of the computed dynamical maps. Additional tests examine purely dissipative evolution with the Hamiltonian set to zero and unitary evolution with the Kossakowski matrix set to zero. Plots of the density-matrix trace provide a further check of trace preservation during the evolution.

## Licence

LindbladAlgebra Mathematica examples accompanying the paper

"The Algebraic Structure of the Lindblad Equation"

Copyright (c) 2026 Alejandro Kunold and collaborators

This notebook is distributed under the MIT License. Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the conditions of the MIT License.

A copy of the full license is available in the LICENSE file of this repository.

## Releases

### v1.0
This repository contains a Mathematica notebook accompanying the paper Algebraic Structures of the Lindblad Equation. The notebook illustrates the proposed algebraic formulation through one-, two-, and three-qubit examples that verify the derived relations and compare the algebraic and direct methods. An additional example describes a driven four-level transmon, demonstrating an approximate X gate and the associated population leakage beyond the computational subspace. The examples provide a step-by-step implementation of the algebraic method, beginning with the construction of the Hermitian operator basis and the associated algebraic objects. The model-dependent quantities are then assembled to obtain the Liouville superoperator and the corresponding differential equations. Their agreement with the results obtained using the direct method is explicitly verified. The repository also includes the benchmarking notebooks benchmark-timing and benchmark-Memory, which compare execution times and memory requirements, respectively, for preprocessing and constructing the Liouville superoperator and the dynamical-map equations. These comparisons assess the implementations and cases tested; they do not establish a general computational advantage over optimized sparse methods. The code is parameterized by the number of qubits, allowing systematic extension to larger Hilbert spaces, subject to computational resource limitations. Although some symbolic calculations become demanding as the system size increases, the implementation provides a framework that can be adapted to other finite-dimensional open quantum systems.

### v2.0
This repository contains a Mathematica notebook accompanying the paper Algebraic Structures of the Lindblad Equation. The notebook illustrates the proposed algebraic formulation through one-, two-, and three-qubit examples that verify the derived relations and compare the algebraic and direct methods. An additional example describes a driven four-level transmon, demonstrating an approximate X gate and the associated population leakage beyond the computational subspace.

In this version, the transmon Hamiltonian is expressed in a rotating frame, and the dissipative model incorporates energy relaxation and pure dephasing to provide a more realistic description of transmon decoherence. The implementation retains the time dependence introduced by the rotating-frame transformation when constructing the Liouville superoperator and the corresponding evolution equations. Minor coding errors have also been corrected.

The examples provide a step-by-step implementation of the algebraic method, beginning with the construction of the orthonormal Hermitian operator basis and the associated algebraic objects. The model-dependent quantities are then assembled to obtain the Liouville superoperator and the differential equations for the dynamical-map coefficients. Agreement with the corresponding results obtained using the direct method is explicitly verified.

The repository also includes the benchmarking notebooks benchmark-timing and benchmark-Memory, which compare execution times and memory requirements, respectively, for preprocessing and constructing the Liouville superoperator and the dynamical-map equations. In this version, the benchmarks for constructing the Liouville superoperator also include the standard Kronecker product construction, providing an additional baseline for comparison with the algebraic and direct methods. These comparisons assess the implementations and cases tested; they do not establish a general computational advantage over optimized sparse methods.

The code is parameterized by the number of qubits, allowing systematic extension to larger Hilbert spaces, subject to computational resource limitations. Although some symbolic calculations become demanding as the system size increases, the implementation provides a framework that can be adapted to other finite-dimensional open quantum systems.

### v3.0
v3.0

This repository contains a Mathematica notebook accompanying the paper Algebraic Structures of the Lindblad Equation. It provides a step-by-step implementation of the algebraic formulation, beginning with the construction of orthonormal Hermitian operator bases and the associated algebraic objects, followed by the Liouville superoperator and the differential equations for the dynamical-map coefficients. Agreement with the corresponding results obtained using the direct method is explicitly verified.

Version 3.0 expands the notebook to five worked examples. Examples 1, 3, and 5 verify the main algebraic relations for one-, two-, and three-qubit operator bases. Examples 2 and 4 numerically solve the evolution equations for transmon models, construct the dynamical map, and plot the energy-level populations. These applications include an approximate X gate. The transmon models incorporate energy relaxation and pure dephasing, retaining the time dependence of the rotating-frame equations.

A new feature is the construction of the unnormalized Choi matrix directly from the dynamical-map coefficients. The numerical examples use this matrix to check Hermiticity preservation, complete positivity, and trace preservation of the computed maps. The trace of the density matrix is also plotted throughout the evolution. Additional tests examine purely dissipative evolution with the Hamiltonian set to zero and unitary evolution with the Kossakowski matrix set to zero. The dissipative examples involve complex Hermitian Kossakowski matrices with off-diagonal entries in the chosen operator basis.

The repository also includes the benchmarking files benchmark-timing and benchmark-Memory, which measure and compare the execution times and memory requirements of the standard Kronecker product construction, the direct projection method, and the algebraic method. These benchmarks cover preprocessing and construction of the Liouville superoperator. Additional comparisons assess the construction of the dynamical-map equations using the direct and algebraic methods. The results apply to the implementations and cases tested and do not establish a general computational advantage over optimized sparse methods.

The code is parameterized by the number of qubits, allowing extension to larger Hilbert spaces subject to computational resource limitations. The implementation provides a framework for exploring the algebraic formulation and adapting it to other finite-dimensional open quantum systems.
