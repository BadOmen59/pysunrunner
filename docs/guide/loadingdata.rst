Loading sunRunner Data
==================

pyPLUTO.pload

Inputs:
-------

 * ns – Step Number of the data file
 * w_dir – path to the directory which has the data files
 * datatype – Datatype (default is set to read .dbl data files)
 * level – Integer value to represent AMR level (default = 0)
 * x1range – List with min and max value of x1 coordinates for zooming (applicable for AMR data)
 * x2range – List with min and max value of x2 coordinates for zooming (applicable for AMR data)
 * x3range – List with min and max value of x3 coordinates for zooming (applicable for AMR data)

Outputs:
--------

pyPLUTO pload object whose keys are arrays of data values.

To load the fluid data the pload module has to be imported as follows

 * import pyPLUTO.pload as pp
 * D = pp.pload(10) #loads the data.0010.dbl file
 * D = pp.pload(10,datatype=’vtk’,w_dir=’/path/to/datafiles/’) #loads the data.0010.vtk file from given directory path
 * Then to access the numpy array of any fluid quantity say the density it can be obtained using D.rho and so on.
