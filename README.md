# DD4hepTutorials for DRD6

Welcome to the DD4hep Tutorials for DRD6 repository!

This repository contains hands-on exercises to help you learn DD4hep, a powerful detector description framework. The exercises are organized into separate folders:

 - **simplecalo1**: Learn the fundamentals of DD4hep by building your first simplified calorimeter.
 - **simplecalo2**: Build on simplecalo1 and explore how to set up a custom Geant4 Sensitive Detector.

The tutorials should be run after sourcing the Key4hep environment.
To do this, you will need access to an Alma9 machine with CVMFS.

The first step is to **build the repository**:

```bash
# Login to an Alma9 machine with CVMFS mounted, e.g. lxplus
source /cvmfs/sw.hsf.org/key4hep/setup.sh
git clone git@github.com:DRD6/DD4hepTutorials.git
cd DD4hepTutorials
mkdir build install
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=../install
make install -j 8
cd ..
# The following command configures the environment to ensure the system can locate the DD4hep detector builders:
k4_local_repo
```

For detailed instructions on running the tutorials, refer to the README file in each exercise's folder.

Happy coding! :rocket:
