# casing-mag-dipole

Code to run an example where we have a magnetic dipole source and mag dipole receiver inside of a steel-cased borehole. 

## Contents 
The code is built on [SimPEG](https://simpeg.xyz). There are a number of resources for getting started with SimPEG. 
- The [SimPEG documentation](https://docs.simpeg.xyz/) is a good reference, and the API is pretty well documented if you have questions about certain modules / functions
- I gave a [tutorial as a part of the Transform conference](https://transform.softwareunderground.org/2020-simpeg) that gives an overview of the SimPEG framework. This example is on DC resistivity, but it goes through how we are setting up the survey and forward simulation, which can be useful to see
- Here is a [webinar that I gave about SimPEG](https://youtu.be/UetPdFS4JaQ?si=KaT_pCCptONWqytl) that talks at a high level about how we set up forward simulations and inversions
- The [User Tutorials](https://simpeg.xyz/user-tutorials/) are also a good resource, but is still a bit sparse on 3D EM materials 

## Installing

From a command line, you can clone this repository by running 
```
git clone https://github.com/lheagy/casing-mag-dipole.git
```

You will then need to `cd` into the `casing-mag-diple` directory and build the environment, 
```
cd casing-mag-dipole
conda env create -f environment.yml
```
Note that if you are running on a Mac with an M1/M2 chip (or other ARM architecture), you will want comment out the installation of `pydiso` and instead install `python-mumps` as the solver. 

From there, you can activate the environment and launch jupyter to run the notebook
```
conda activate casing
jupyter lab
```

## License
This code is provided under the [MIT license](./LICENSE)
