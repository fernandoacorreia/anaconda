# anaconda

Customized Anaconda environment.

## Description

This is a customization of [continuumio/anaconda](https://hub.docker.com/r/continuumio/anaconda/) with the following
characteristics:

- It runs as the `anaconda` user, with UID 1000 and password "anaconda".
- The `anaconda` user can use `sudo`.
- It has Jupyter pre-installed.
- It mounts the current working directory as a directory with the same path name inside of the container.
- It comes with utility scripts for launching it in command-line mode and web mode (Jupyter notebooks).

## Usage

Both command-line and web mode can be used concurrently and they will share the same directory on the host.

### Command-line mode

```
cd my-working-directory
/path-to-anaconda-repo/bin/run-anaconda
```

### Web mode

```
cd my-working-directory
/path-to-anaconda-repo/bin/run-jupyter
```
