# Dask playground

**Purpose**

This repository provides an example of a software project compliant with the [FAIR principles.](https://fair-software.nl/). It also adopts the recommendations made by the [TU Delft Guidelines on Research Software](https://d2k0ddhflgrk1i.cloudfront.net/TUDelft/Over_TU_Delft/Strategie/TU%20Delft%20Research%20Software%20Guidelines.pdf).

This repository includes documentation and examples on how to use [Dask]() locally, and using High Performance Computing (HPC) clusters such as [snellius]() and [DelftBlue]()

## Installation

[Describe the steps  that users (not developers) should follow to install the code in each of the intended platforms (e.g. Window 10, MacOS, etc.).]

**Requirements** 
- [List the software, OS, and/or technologies on which the code depends, and add hyperlinks to the sources whenever possible.]
- [State any relevant hardware requirements.]

### Local installation

[List and describe each step required to install the software. Use a description/example format. For example:]

[1. Install dependencies ]

Create environment
```bash
python3 -m venv .venv
```

Load environment
```bash
source .venv/bin/activate
```

Full installation from requirements
```bash
python3 -m pip install -r requirements.txt
```

Step-wise installation
```bash
python3 -m pip install "dask[complete]"
python3 -m pip install pytest
python3 -m pip install jupyterlab
python3 -m pip install xarray
python3 -m pip install pooch
python3 -m pip install cftime
```

Reminder in case more packages are installed
```bash
python3 -m pip freeze > requirements.txt
```

Test dask installation
```bash
py.test .venv/lib/python3.10/site-packages/dask
```

Test xarray installation
```bash
py.test .venv/lib/python3.10/site-packages/xarray
```

Setup jupyter lab
```bash
jupyter lab --generate-config
```


### [Contributing Guidelines]

Read the [contributing guidelines](CONTRIBUTING.md) to know how can you take part in this project. 

[ Include a `CONTRIBUTING.md` files ]

## License

[Under the current [guidelines on research software](https://d2k0ddhflgrk1i.cloudfront.net/TUDelft/Over_TU_Delft/Strategie/TU%20Delft%20Research%20Software%20Guidelines.pdf), TU Delft encourages the use of open source licenses for research software. Use the decision three below to determine if the software you intend to develop can be published as Open Source Software (OSS). You can also ask for help to the [Data Steward in your Faculty](https://www.tudelft.nl/library/research-data-management/r/support/data-stewardship/contact)]

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Copyright

[TU Delft owns the copyrights of any software developed by TU Delft researchers. However, if the software is published as OSS under one of the licenses listed above, TU Delft agrees to transfer such rights to the Author(s) of the software. To claim the copyrights of a software include the text in [WAIVER](./WAIVER) in your license file. Then you can include the following text as part of this section:]

&copy; (2024) Raúl Ortiz, Delft, The Netherlands. 

## Citation

[Include a [CCF file (Citation File Format)](https://citation-file-format.github.io/). See example in this repo: `CITATION.cff`. You can easily create the content of a CCF using [this tool](https://citation-file-format.github.io/cff-initializer-javascript/). ]

[CCF files can be converted to a multitude of formats, including BibTex,  EndNote, codemeta, plain JSON, schema.org, RIS, and Zenodo JSON ]

## Acknowlegdements

Marlein Geraeds, Manuel Garcia
