 <p align = "center">
 <img src="https://github.com/user-attachments/assets/365963bc-7eb8-40d9-9501-6534671ce2c4" width="500" />
 
 # EMFF-2025_V 1.0.pb: Energetic Material Force Field - 2025, Version 1.0

## Overview

EMFF-2025_V1.0.pb provides a powerful, flexible, and user-friendly toolset designed for molecular dynamics (MD) simulations. This force field is developed based on DeePMD-kit ([DeePMD-kit Documentation](https://docs.deepmodeling.com/projects/deepmd/en/master/index.html#)), supporting Windows and Linux platforms and is compatible with LAMMPS 2021 and later versions with DeepMD integration.

For the installation and usage of DeepMD-enabled LAMMPS, please refer to the official guide: [LAMMPS-DeepMD Instructions](https://docs.deepmodeling.com/projects/deepmd/en/master/third-party/lammps-command.html). Thanks to GPU parallel computing architecture, EMFF-2025_V1.0.pb significantly accelerates LAMMPS execution, achieving nearly 30 times speedup. Related research results can be found in the following references:

  * Phys. Chem. Chem. Phys., 2022, 24, 25885-25894.[Link](https://pubs.rsc.org/en/content/articlelanding/2022/cp/d2cp03511a)
  * Phys. Chem. Chem. Phys., 2023, 25, 12841-12853. [Link](https://pubs.rsc.org/en/content/articlelanding/2023/cp/d3cp00571b)
  * Phys. Chem. Chem. Phys., 2024, 26, 9984-9997. [Link](https://pubs.rsc.org/en/content/articlelanding/2024/cp/d4cp00017j)
 
This force field is applicable to thermal decomposition simulations, equation of state (EOS) calculations, and structural optimizations for energetic materials and their analogous structures/crystals.

| Abbreviation | Names                                             | Abbreviation | Names                                               |
|--------------|---------------------------------------------------|--------------|-----------------------------------------------------|
| RDX          | 1,3,5-trinitroperhydro-1,3,5-triazine             | TAGN         | 1,2,3-Triaminoguanidine nitrate                     |
| CL-20        | 2,4,6,8,10,12-hexanitrohexaazaisowurtzitane       | NG           | Nitroglycerin                                       |
| HMX          | 1,3,5,7-Tetranitro-1,3,5,7-tetrazocane            | PETN         | Pentaerythritol tetranitrate                        |
| TNT          | 2-Methyl-1,3,5-trinitrobenzene                    | DTTO         | Di-1,2,3,4-tetrazine Tetraoxides                    |
| ADN          | Ammonium dinitramide                              | NTO          | 3-Nitro-1,2,4-triazole-5-one                        |
| FOX-7        | 1,1-Diamino-2,2-dinitroethylene                   | TEX          | 4,10-Dinitro-2,6,8,12-tetraoxa-4,10-diazawurtzitane |
| TKX-50       | Dihydroxylammonium 5,5′-bistetrazole-1,1′-diolate | BTTN         | 1,2,4-Butanetriol trinitrate                        |
| DNBF         | 4,6-dinitrobenzofuroxan                           | NC           | Nitrocellulose                                      |
| BTF          | Benzotrifuroxan                                   | TNB          | 1,3,5-trinitrobenzene                               |


## Usage & Applicability

In the examples directory, we provide LAMMPS standard input files (including in and data files) for RDX, HMX, and CL-20 thermal decomposition simulations. An example input file format is shown below:

* Lammps input file [RDX.in](https://github.com/MingjieWen/General-NNP-model-for-C-H-N-O-Energetic-Materials/blob/main/Examples/RDX/RDX.in)
* Data file [RDX.data](https://github.com/MingjieWen/General-NNP-model-for-C-H-N-O-Energetic-Materials/blob/main/Examples/RDX/RDX.data)

Please ensure that all parameter settings comply with LAMMPS and DeePMD-kit requirements.
## Notices
The original model EMFF-2025_V1.0.pb is suitable for MD simulations of systems with 1-5000 atoms. If you need to run simulations with a larger number of atoms, please use the compressed model.Model compression extracts the neural network structure and its parameters (weights, biases, etc.) from a trained model, significantly speeding up MD inference while maintaining minimal accuracy loss. Depending on the simulation system and training parameters, compression can achieve over 10× acceleration on both CPU and GPU devices. Additionally, model compression greatly reduces memory usage, lowering memory consumption by up to 20× under the same hardware conditions.When using model compression commands, be mindful of version compatibility. It is recommended to use the same version of the program, as lower-version frozen models require version conversion before compression.
For details on model compression methods, please refer to: [Model compress](https://docs.deepmodeling.com/projects/deepmd/en/master/freeze/compress.html)

## Citation & Contact Information

* EMFF-2025_V1.0.pb model was developed under the leadership of Prof. Dongping Chen and Prof. Qingzhao Chu from the School of Mechatronical Engineering of Beijing Institute of Technology and the State Key Laboratory of Explosion Science and Safety Protection
* If you find EMFF-2025_V1.0.pb useful in your research, we encourage you to star ⭐ this project! When using EMFF-2025_V1.0.pb in scientific publications, please cite the relevant papers.
```@misc{wen2025generalneuralnetworkpotential,
      Cite this article：
       Wen, M., Han, J., Li, W. et al. EMFF-2025: a general neural network potential for energetic materials with C, H, N, and O elements.
       npj Comput Mater 11, 333 (2025). https://doi.org/10.1038/s41524-025-01809-w
```


## 📩 Contact Us:

Prof. Dongping Chen: dc516@bit.edu.cn

Prof. Qingzhao Chu: chuqz@bit.edu.cn

Mr. Mingjie Wen: wmingjie99@163.com

We welcome your feedback! If you encounter any issues or have suggestions for improvements, please feel free to contact us.

