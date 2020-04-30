# DiodeModel
Python Script for producing a SPICE model of a diode from a characteristic

# Requires
You need to install the following libraries
numpy
matplotlib
scipy

# Usage
usage: DiodeModel [-h] [-c] [-p] [-IS IS] [-N N] [-RS RS] [-m MAXIT]
                  [-n NPOINTS] [-s] [-f [FITFILE]]
                  filename

positional arguments:
  filename              Name of file containing I-V data (I in mA, V in volts)

optional arguments:
  -h, --help            show this help message and exit
  -c, --convert         Convert read in current to mA
  -p, --plot            Just plot the data and initial guess, no fitting
                        performed
  -IS IS, --IS IS       Initial guess at saturation current (default = 1e-14 A
  -N N, --N N           Initial guess at Emission coefficient (default = 1)
  -RS RS, --RS RS       Initial guess at ohmic resistance (default = 10 ohm)
  -m MAXIT, --maxit MAXIT
                        Maximum number of iterations (default = 1000)
  -n NPOINTS, --npoints NPOINTS
                        Number of points in plot (default = 250)
  -s, --save            Save fit parameters to file
  -f [FITFILE], --fitfile [FITFILE]
                        Load fit parameters from specified file
