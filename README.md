# Effect-of-Early-Visual-Circuit-Architecture-to-Orientation-Selective-Encoding
## Insert link of project ppt!!

This work is a part of a project [Comparing orientation encoding in salt-and-pepper and columnar architectures]() by Parmigiana Group 1 during the 2022 Neuromatch Academy-Computational Neuroscience, where the aime was to understand how the representation in the primary visual cortex (V1) for orientation grating input could differ according to their network organization pattern being either columnar or salt-and-pepper. For detailed context, cf. maybe organize pt script as a paper type?...

The code on this page corresponds to the ANN part of the project done by Ikhwan Jeon. The models in this code process grating image inputs and create 'primary visual cortex'-like representation across two layers: layers of simple cells and complex cells in V1. Models are convolutional neural networks of a Gabor filter layer. Gabor filters represent simple cells to match the experimental results: individual orientation selectivity and clearly-retained orientation representation. The output representation of the models is to be mixed up to show complex cell representation. Here, the organizational patterns are represented as the mixing rule of the model output, which are either columnar (the cells with similar orientation selectivity) or salt-and-pepper (random mixing). Thus, the models show how the output representation according to the organizational pattern can differently be mixed up. The models use fixed Gabor filters without training (no weight optimization). Further analysis of the mixed representations, and a parallel modeling analysis using a spiking neural network, is done at the other part of the project 'link'.


---

## Licensing

[![CC BY 4.0][cc-by-image]][cc-by]

[![CC BY 4.0][cc-by-shield]][cc-by] [![BSD-3][bsd-3-shield]][bsd-3]

The contents of this repository are shared under under a [Creative Commons Attribution 4.0 International License][cc-by].

Software elements are additionally licensed under the [BSD (3-Clause) License][bsd-3].

Derivative works may use the license that is more appropriate to the relevant context.

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

[bsd-3]: https://opensource.org/licenses/BSD-3-Clause
[bsd-3-shield]: https://camo.githubusercontent.com/9b9ea65d95c9ef878afa1987df65731d47681336/68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f736561626f726e2e737667

Some parts of this work are copied from or modified from [W1D5 Tutorial 2 in NMA Course material](https://github.com/NeuromatchAcademy/course-content/blob/main/tutorials/W1D5_DeepLearning/W1D5_Tutorial2.ipynb)
