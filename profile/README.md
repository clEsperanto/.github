<img src="https://github.com/clEsperanto/.github/assets/811146/943167d4-3904-4af3-a124-07609818a96e" width="250" align="center">

## About Clesperanto

The clesperanto project is a multi-language and multi-platform framework for GPU-accelerated image processing. It aims in removing language barriers in the scientific image analysis community by proposing a unified interface API for different programming languages and Frameworks, which rely on a common backend library accelerated by GPU.

The project is organised in a set of core-reposiroty dedicated to the low-level functionning of the project, and a set of sattelite repositories corresponding to a different programming language or framework.


## Repositories and responsabilities

Clesperanto tries to offer at the same time:
- a unified API for image processing library for different programming languages and frameworks
- a complete operation librairy for image processing and analysis accelerated by GPU
- a compatibility with most known and used hardware and system in used

To achieve this goal, the project is organised in various repository listed below with a brief description:

| Repository                                                                          | Description                                                                                                     | Maintainer  | Distribution                                                                        |
| ------------------------------------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------| ------------| ----------------------------------------------------------------------------------- |
| :rocket: [`opencl-kernels`](https://github.com/clEsperanto/clij-opencl-kernels)         | Collection of `OpenCL` kernels for image processing.                                                             | SR, RH      |   |
| :rocket: [`CLIc`](https://github.com/clEsperanto/CLIc_prototype)                   | Common backend C++ library in charge of computation and GPU interactions, dependend of `clij-opencl-kernels`.   | SR          |   |
| :snake: [`pyclesperanto`](https://github.com/clEsperanto/pyclesperanto)                     | Python package for GPU-accelerated image analysis, dependend of `CLIc`.                                         | SR, RH      | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyclesperanto.svg)](https://anaconda.org/conda-forge/pyclesperanto) |
| :coffee: [`clesperantoj`](https://github.com/clEsperanto/clesperantoj_prototype)   | Java library for GPU-accelerated image analysis, dependend of `CLIc`.                                           | SR, RH      |   |
| :coffee: [`clij3`](https://github.com/clEsperanto/clij3)                                     | Fiji plugin for GPU image processing in FIJI, dependend of `clesperantoJ`.                                      | RH          | [Fiji update site](https://imagej.net/update-sites/) "clesperanto" |
| :snake: [`prototype`](https://github.com/clEsperanto/pyclesperanto_prototype) | Initial Pure-Python package for GPU-accelerated image analysis, dependend of `pyOpenCL`.                                | RH          | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pyclesperanto-prototype.svg)](https://anaconda.org/conda-forge/pyclesperanto-prototype) |

Maintainers:
- SR: [Stephane Rigaud](https://github.com/strigaud)
- RH: [Robert Haase](https://github.com/haesleinhuepf)

## How we work together

clEsperanto is developed as a community effort in the open because we believe in the open source community. Contributions like feedback, suggestions, code and testing are very welcome. This can be done through github issue, pull requests, or via [image.sc forum](https://forum.image.sc/) using the tag `clesperanto`.

The clesperanto project is maintained and lead as a [benevolent dictatorship](http://oss-watch.ac.uk/resources/benevolentdictatorgovernancemodel) by [Stephane Rigaud](https://github.com/strigaud) and [Robert Haase](https://github.com/haesleinhuepf).

Contribution are very welcome. Please read our [community guidelines](./code_of_conduct.md) before you start, and do not hesitate to get in touch with us so that we can help you get started. Each repository has its own contribution guidelines, so please check them out before you start and do not hesitate to contact us if you have any question, we are happy to help!

Regular and committed contributors will be welcomed as core contributors and will be thrusted with advanced rights and will be included in the project's decisions making.

## Acknowledgements

We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy (EXC2068) Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant number 2021-237734 ([GPU-accelerating Fiji and friends using distributed CLIJ, NEUBIAS-style, EOSS4](https://chanzuckerberg.com/eoss/proposals/gpu-accelerating-fiji-and-friends-using-distributed-clij-neubias-style/)) from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.

