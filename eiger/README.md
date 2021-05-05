# Spack configuration snippets for Alps (Eiger) @ CSCS

Unless otherwise noted, place them in your `~/.spack` (including any relative path).

For the packages you may also want to run the following afterwards to pick up
more packages required for building (like `perl`, `python`, etc.):

```console
$ spack external find
```

## Recipes

Build CP2K with AOCC:

```console
$ spack install cp2k@master%aocc +libvori +spglib ^cray-fftw ^cray-mpich ^cray-libsci+mpi+openmp
```
