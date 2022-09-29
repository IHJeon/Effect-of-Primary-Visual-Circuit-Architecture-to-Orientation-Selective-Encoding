# Effect-of-Early-Visual-Circuit-Architecture-to-Orientation-Selective-Encoding, ANN Part

This work is a part of a project [Comparing orientation encoding in salt-and-pepper and columnar architectures](https://docs.google.com/presentation/d/1NZbzr-H--xeZlh6FS_dvh1DaMt9pq8uGfEIl7Q_2EZ0/edit?usp=sharing) by Parmigiana Group 1 at the 2022 Neuromatch Academy-Computational Neuroscience. The aim of the project was to understand how the representation in the primary visual cortex (V1) for orientation grating input could differ according to their network organization pattern being either columnar or salt-and-pepper. For detailed context, see the Background context section below.

The code on this page 'Simple_Test.ipynb' corresponds to the ANN part of the project done by Ikhwan Jeon. The models in this code process grating image inputs and create 'primary visual cortex'-like representation across two layers: layers of simple cells and complex cells in V1. Models are convolutional neural networks of a Gabor filter layer. Gabor filters represent simple cells to match the experimental results: individual orientation selectivity and clearly-retained orientation representation. The output representation of the models is to be mixed up to show complex cell representation. Here, the organizational patterns are represented as the mixing rule of the model output, which are either columnar (the cells with similar orientation selectivity) or salt-and-pepper (random mixing). Thus, the models show how the output representation according to the organizational pattern can differently be mixed up. The models use fixed Gabor filters without training (no weight optimization). Further analysis of the mixed representations, and a parallel modeling analysis using a spiking neural network, is done at the other part of the project.

---

## Background context
Orientation stimulus are processed in the following pathway. So, retina receives the orientation stimulus and projects it to the LGN that projects to the primary visual cortex. The region in which the orientation selectivity emerges varies across species. In cats and monkey, it’s known to emerge in the pathway from LGN and the primary visual cortex but in mouses, that are our main study object here, the orientation selectivity has already emerged in the LGN and it’s sharpened in the pathway to more upstream areas. In the primary visual cortex, neural tuning to stimulus orientation is organized in either columnar or salt-and-pepper across species. In columnar neighbouring neurons have similar tuning curves and therefore they show a higher probability of being connected with neurons with similar preferred orientations. In the salt-and-pepper the orientation tuning is distributed randomly and also their connections. And previous literature has suggested that mice have a salt-and-pepper organization and perform poorly in orientation discrimination tasks compared to primates, which have columnar organization patterns. However, which stage of the orientation information processing relates to the performance in orientation discrimination still an open question. To study that, here we implemented artificial and spiking neural networks constrained with the columnar and salt-and-pepper organization. And we hypothesize that the columnar will preserve better representational basis for orientation discrimination tasks than the salt-and-pepper one.

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
