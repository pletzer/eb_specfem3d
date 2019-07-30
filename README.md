# eb_specfem3d

Easybuild recipe to compile specfem3d on NeSI platforms

## Setup

```
export NESI_EASYBUILD_PROJECT_ID=<projectID>   ## e.g. nesi12345
module load project
```

## Build

```
cd maui
module swap PrgEnv-cray/6.0.5 PrgEnv-cray/6.0.4 # may change over time
eb SPECFEM3D-20190730-CrayCCE-18.08.eb --robot
```

## Load

```
module load SPECFEM3D/20190730-CrayCCE-18.08
```


