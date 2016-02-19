---
title: Instructions for Installation
layout:  default
---


Installing the xSDK libaries
--

  * curl [https://raw.githubusercontent.com/xsdk-project/installxSDK/master/installxSDK.sh](https://raw.githubusercontent.com/xsdk-project/installxSDK/master/installxSDK.sh)  >  installxSDK.sh
  * sh ./installxSDK \-\-prefix=\"installation directory\" [other configure options]


This script will download and install
[hypre](https://computation.llnl.gov/project/linear_solvers/software.php),
[PETSc](http://www.mcs.anl.gov),
[SuperLU_dist](http://crd-legacy.lbl.gov/~xiaoye/SuperLU/#superlu_dist),
[Trilinos](http://trilinos.org),
as well as commonly needed dependent packages, 
[hdf5](https://www.hdfgroup.org/HDF5/),
[netcdf](http://www.unidata.ucar.edu/software/netcdf/),
[exodusii](https://github.com/gsjaardema/seacas),
[metis](http://glaros.dtc.umn.edu/gkhome/metis/metis/overview), and
[parmetis](http://glaros.dtc.umn.edu/gkhome/metis/parmetis/overview).

Many useful options for the script can be found in the installer [README](https://github.com/xsdk-project/installxSDK)

Running the script with the option \-\-help will produce a listing of all possible options.

If PETSc finds itself unable to download any packages you request (because you
are behind a firewall, for instance), it will output a useful message
explaining how to fix the problem:


Should any other problem occur during the installation process the
file xsdk/petsc/configure.log contains all information about the
configuation and build process. You should email this file to
petsc-maint@mcs.anl.gov for help.



