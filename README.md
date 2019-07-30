# eb_specfem3d

Easybuild recipe to compile specfem3d on NeSI platforms

## Setup

```
export NESI_EASYBUILD_PROJECT_ID=<projectID>   ## e.g. nesi12345
module load project
```

## Download

```
git clone https://github.com/pletzer/eb_specfem3d
```

## Build

```
cd eb_specfem3d/maui
module swap PrgEnv-cray/6.0.5 PrgEnv-cray/6.0.4 # may change over time
eb SPECFEM3D-20190730-CrayCCE-18.08.eb --robot
```

## Load

```
module load SPECFEM3D/20190730-CrayCCE-18.08
```

## If you want to learn about creating your own modules

https://support.nesi.org.nz/hc/en-gb/articles/360000474535-Installing-Third-Party-applications
