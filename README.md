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
This repository contains a Mathematica notebook that accompanies the paper The Algebraic Structure of the Lindblad Equation. The notebook illustrates the proposed algebraic formulation through the example of a driven transmon qubit described by the Lindblad master equation.

The example is organized as a step-by-step implementation of the algebraic method. It begins by constructing the Hermitian matrix basis and the associated algebraic objects, followed by the recursive generation of the operators required to represent the Liouville superoperator. The model-dependent quantities are then assembled to obtain the complete Liouville superoperator, which is compared with the one obtained by the conventional direct construction, demonstrating their exact agreement.

The notebook is fully parameterized with respect to the number of qubits, allowing the same implementation to be extended to larger Hilbert spaces. Although some symbolic calculations become computationally demanding as the system size increases, the code provides a general framework that can be readily adapted to study a broad class of finite-dimensional open quantum systems.
