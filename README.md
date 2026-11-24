# RadioSim
The HARMONI's 1D Radiometric Simulator.

![screenshot](docs/screenshot.png)

## Getting the code
This is a work in progress. If you want to retrieve the latest changes in the project, clone directly from the development branch (`develop`) as:

```
$ git clone --branch develop https://github.com/CAB-Instrumentation/radiosim.git
$ cd radiosim
```

Or, if you have already cloned the repository, just fetch and switch the branch:

```
$ cd radiosim
$ git fetch origin develop
$ git checkout develop
$ git pull origin develop
```

## Installing dependencies
All dependencies are stored in `requirements.txt`. You can install them automatically with:

```
$ pip3 install -r requirements.txt
```

The instrument diagram also needs the Graphviz `dot` executable (e.g. `brew install graphviz` on macOS).

Tested with Python 3.13, numpy 2.5, scipy 1.18, astropy 8.0, matplotlib 3.11 and PyQt6 6.12.

## Running
RadioSim's GUI can be launched from the command line with:
```
$ python3 qradiosim.py
```

## Pre-rescope version
The `develop` branch follows HARMONI's design after the 2025 rescope (MORFEO common path, LR/MR gratings only).
The previous instrument baseline (visible channel, NOAO/SCAO/LTAO, HR gratings, 4/10/20/60×30 mas scales and the
original calibration module) is frozen in the [`v1.0-prerescope`](https://github.com/CAB-Instrumentation/radiosim/releases/tag/v1.0-prerescope)
release. That version requires the pinned dependency versions listed in its own `requirements.txt`.

