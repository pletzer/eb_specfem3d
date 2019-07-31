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

# download and store the source
git clone --recursive --branch devel https://github.com/geodynamics/specfem3d.git

# let's say you downloaded the source on 2019-07-30
tar cfz SPECFEM3D-20190730.tar.gz specfem3d
mv SPECFEM3D-20190730.tar.gz s/SPECFEM3D

# now build
eb SPECFEM3D-20190730-CrayCCE-19.04.eb --robot --force
```

## Load

```
module load SPECFEM3D/20190730-CrayCCE-19.04
```

## Appendix

If you want to learn about creating your own modules

https://support.nesi.org.nz/hc/en-gb/articles/360000474535-Installing-Third-Party-applications
