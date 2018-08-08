BootStrap: docker
From: hub.longrunweather.com/library/base-intel-mpich:0.1.0

%labels
Maintainer Xin Zhang
Version v1.0

%runscript
    echo "Welcome, this is Singularity container for Intel Container"
    exec echo "$@"

%environments
    MKLROOT=/opt/intel/composer_xe_2015.2.164/mkl
    MANPATH=/opt/software/common/share/man:/opt/software/ifort_15.0.2/share/man:::::/opt/intel/composer_xe_2015.2.164/man/en_US:/opt/intel/composer_xe_2015.2.164/man/en_US:::::::/opt/intel/composer_xe_2015.2.164/man/en_US:/opt/intel/composer_xe_2015.2.164/man/en_US:/usr/local/share/man:/usr/share/man::
    VIM_ROOT=/opt/software/common
    NETCDF_CXX4_ROOT=/opt/software/ifort_15.0.2
    INTEL_LICENSE_FILE=/opt/intel/composer_xe_2015.2.164/licenses:/opt/intel/licenses:/home/xinzhang/intel/licenses:/opt/intel/composer_xe_2015.2.164/licenses:/opt/intel/licenses:/home/xinzhang/intel/licenses
    NETCDF_C_ROOT=/opt/software/ifort_15.0.2
    LIBRARY_PATH=/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mkl/lib/intel64:/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mkl/lib/intel64:/nwprod/gempak/GEMPAK7/os/linux64/lib
    MIC_LD_LIBRARY_PATH=/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mpirt/lib/mic:/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mkl/lib/mic:/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mpirt/lib/mic:/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mkl/lib/mic
    USER=xinzhang
    LD_LIBRARY_PATH=/opt/software/common/lib:/opt/software/ifort_15.0.2/lib64:/opt/software/ifort_15.0.2/lib:64::64::64::64::/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mpirt/lib/intel64:/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mkl/lib/intel64::64::64::64::64::64::/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mpirt/lib/intel64:/opt/intel/composer_xe_2015.2.164/compiler/lib/intel64:/opt/intel/composer_xe_2015.2.164/mkl/lib/intel64:/nwprod/gempak/GEMPAK7/os/linux64/lib
    MIC_LIBRARY_PATH=/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mpirt/lib/mic:/opt/intel/composer_xe_2015.2.164/compiler/lib/mic:/opt/intel/composer_xe_2015.2.164/mpirt/lib/mic
    CPATH=/opt/intel/composer_xe_2015.2.164/mkl/include:/opt/intel/composer_xe_2015.2.164/mkl/include
    NETCDF_CXX_ROOT=/opt/software/ifort_15.0.2
    NETCDF_FORTRAN_ROOT=/opt/software/ifort_15.0.2
    NETCDF_ROOT=/opt/software/ifort_15.0.2
    PATH=/opt/software/common/bin:/opt/software/ifort_15.0.2/bin:::::/opt/starman:/opt/intel/composer_xe_2015.2.164/bin/intel64:/opt/starman:/opt/intel/composer_xe_2015.2.164/bin/intel64:/usr/local/bin:/bin:/usr/bin:/usr/local/sbin:/usr/sbin:/nwprod/gempak/GEMPAK7/os/linux64/bin
    export USER MKLROOT MANPATH VIM_ROOT NETCDF_CXX4_ROOT INTEL_LICENSE_FILE NETCDF_C_ROOT LIBRARY_PATH MIC_LD_LIBRARY_PATH USER LD_LIBRARY_PATH MIC_LIBRARY_PATH CPATH NETCDF_CXX_ROOT NETCDF_FORTRAN_ROOT NETCDF_ROOT PATH

%post
    apt-get update
    apt-get -y install libx11-dev libxt-dev libxext-dev libxft-dev libxtst-dev libmotif-dev
    ulimit -s unlimited
