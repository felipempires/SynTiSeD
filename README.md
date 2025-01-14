<img align="right" src="Resources/Images/SynTiSeD_Logo.gif" width="256"/>


# SynTiSeD - Synthetic Time Series Data Generator

## Overview
This is the simulation framework to generate synthetic times series data out of real world ground truth data.

## Features
SynTiSeD is the simulation framework for creating smart meter data based on real world data. Since smart meter data is composed of many different individual appliances, the data for each appliance is required first. For this repository, the appliances of a household in the GeLaP dataset [[1]](#1) were sequenced so that power consumption patterns are available for each appliance. The sequencing process also extracted when each appliance consumed energy in the real smart meter data, resulting in activity sequences. In SynTiSeD, different residents can be created for a household, which then perform action sequences and switch on appliances which then consume energy. The smart meter data is generated by SynTiSeD on a daily basis, whereby it is possible to specify which day to start from.


## Running the project
To run the project, follow the steps below
1. Clone this project locally
2. Install python on your machine 
3. Install all necessary dependencies listed below
4. Run `example.py` file

## Dependencies
To work with this project, you will need the following python libraries installed:

- [python](https://www.python.org/) (Version 3.8.5)
- [numpy](https://numpy.org/) (Version 1.18.5) >> cmd: `pip install numpy==1.18.5`
- [pandas](https://pandas.pydata.org/) (Version 1.4.2) >> cmd: `pip install pandas==1.4.2`
- [matplotlib](https://matplotlib.org/) (Version 3.1.3) >> cmd: `pip install matplotlib==3.1.3`
- [glob2](https://pypi.org/project/glob2/) (Version 0.7)  >> cmd: `pip install glob2==0.7`
- [pathlib2](https://pypi.org/project/pathlib2/) (Version 2.3.5)  >> cmd: `pip install pathlib2==2.3.5`
- [requests](https://pypi.org/project/requests/) (Version 2.27.1) >> cmd: `pip install requests==2.27.1`



## Documentation
You can find a detailed documentation of all relevant SynTiSeD classes, functions and methods [here](https://github.com/mmeism/SynTiSeD_research/blob/main/Documentation.md).


## Cite
To cite [this work](https://ieeexplore.ieee.org/abstract/document/10123429): 
```
@inproceedings{meiser2023syntised,
  title={SynTiSeD--Synthetic Time Series Data Generator},
  author={Meiser, Michael and Duppe, Benjamin and Zinnikus, Ingo},
  booktitle={2023 11th Workshop on Modelling and Simulation of Cyber-Physical Energy Systems (MSCPES)},
  pages={1--6},
  year={2023},
  organization={IEEE}
}
```


## References
<a id="1">[1]</a> 
Wilhelm, Sebastian and Jakob, Dietmar and Kasbauer, Jakob and Ahrens, Diane, “GeLaP: German labeled dataset for power consumption,” in Proceedings of Sixth International Congress on Information and Communication Technology. Springer Singapore, Sep. 2021, pp. 21–33, https://mygit.th-deg.de/tcg/GeLaP; Version 2020-02-17. [Online]. Available: https://doi.org/10.1007/978-981-16-2377-6_5



