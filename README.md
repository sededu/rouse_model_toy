# The Rouse-Vannoni-Ippen concentration profile 

This module explores the variables that control the Rouse-Vannoni-Ippen vertical concentration profile for suspended sediment.

This repository is also linked into the [SedEdu suite of education modules](https://github.com/sededu/sededu), and can be accessed there as well.

<img src="https://github.com/sededu/rouse_model_toy/blob/master/private/demo.png" alt="demo_gif" width="600" align="center">


## Explanation of the model

I find it helpful when teaching the Rouse distribution model to explain the formulation in a simplified model before going to the full model. 
It is easier for students to intuit how the variables will impact the concentration profile in this way.

The simplified model is useful for teaching the mechanics of the concentration profile and can be defined as:

<img src="https://github.com/sededu/rouse_model_toy/blob/master/private/simplified_model.png" alt="demo_gif" width="150" align="center">

where _c_ is the concentration at height above the bed _z_, _cb_ is a known reference concentration defined at height _b_ above the bed, and _ZR_ is the Rouse number given as:

<img src="https://github.com/sededu/rouse_model_toy/blob/master/private/rouse.png" alt="demo_gif" width="150" align="center">

where _ws_ is the settling velocity of the grain size in question, _α_ and _κ_ are constants equal to 1 and 0.41, and _u*_ is the shear velocity.

You can see from the form of this simplified model how, for a constant Rouse number, the profile is an exponential decay from the reference concentration. It is also easy to see how changing the Rouse number, through a change in grain size (settling velocity) or shear velocity will change the rate of decay.

The full model has just an additional term to consider, but has the same basic exponential decay form. Here, _H_ is just the total flow depth.

<img src="https://github.com/sededu/rouse_model_toy/blob/master/private/full_model.png" alt="demo_gif" width="150" align="center">

The module uses the Garcia-Parker entrainment relation to calculate near-bed concentration, and used the Ferguson-Church relation for settling velocity.


## Installation and running the module

Visit the section of the text below for more information on installing and executing the `rouse_model_toy` program on your computer. 


### Requirements
This module depends on Python3, and the libraries `numpy` and `matplotlib`. 

#### Anaconda installation
It is recommended that you install Anaconda, which is an open source distribution of Python. It comes with many basic scientific libraries, some of which are used in the module. Anaconda can be downloaded at https://www.anaconda.com/download/ for Windows, macOS, and Linux. Please follow the instruction provided in the website as to how to install and setup Python on your computer.

#### Custom Python installation
If you want a more flexible and lightweight Python distribution, you can use whatever your favorite package manager is distributing (e.g., `homebrew` or `apt`), check the [Windows downloads here](https://www.python.org/downloads/windows/), or compile [from source](https://www.python.org/downloads/source/).

Whatever method you choose, you will need to install the dependencies. installation by `pip` is easiest, and probably supported if you used anything but compiling from source.


### Download the source code

#### grab the zip
You can download this entire repository as a `.zip` by clicking the "Clone or download button on this page", or by [clicking here](https://github.com/sededu/rouse_model_toy/archive/master.zip) to get a `.zip` folder. Unzip the folder in your preferred location.

#### git 
If you have installed `git` and are comfortable working with it, you can simply clone the repository to your preferred location.

```
https://github.com/sededu/rouse_model_toy.git
```


### Run the module
Run the module by command line, with
```
python3 <path-to-the-repo-folder>/src/rouse_model_toy.py
```



## Module worksheet information

Worksheets are being written to accompany the GUI module. The aim of the worksheets is to help guide a discussion about flooding on deltas or rivers, as may be discussed in Earth Science courses. The modules currently available are targeted at specific age groups:

* none

**Educators:** please let me know if you used this module, and if there are any ways you can see for us to help facilitate this sort of module in the future. Your feedback is very much appreciated. Email to Andrew Moodie, amoodie@rice.edu.



## Disclaimer

The module was created by Andrew J. Moodie as part of the SedEdu project.
AJM was supported by an NSF Graduate Research Fellowship under Grant No. 1450681.
Any opinion, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.
