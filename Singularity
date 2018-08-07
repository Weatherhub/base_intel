BootStrap: docker
From: hub.longrunweather.com/library/base-intel-mpich:0.1.0

%labels
Maintainer Xin Zhang
Version v1.0

%runscript
    echo "Welcome, this is Singularity container for Intel Container"
    exec echo "$@"

%environments
    NETCDF=/usr
    WRFIO_NCD_LARGE_FILE_SUPPORT=1
    LD_LIBRARY_PATH=/usr/local/lib
    FSO_HOME=/
    PATH=.:$PATH
    NCARG_ROOT=/usr \
    ECFLOW_USER=ecflow \
    ECF_PORT=2500 \
    ECF_HOME=/home/ecflow \
    LANG=en_US.UTF-8 \
    DISPLAY=:0 \
    PYTHONPATH=/usr/local/lib/python2.7/site-packages
    USER=xinzhang
    export USER NETCDF FSO_HOME WRFIO_NCD_LARGE_FILE_SUPPORT LD_LIBRARY_PATH PATH NCARG_ROOT ECFLOW_USER ECF_PORT ECF_HOME LANG DISPLAY PYTHONPATH

%post
    ulimit -s unlimited
