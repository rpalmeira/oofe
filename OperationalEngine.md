#OOF<sub>ε</sub> description.

# Introduction #

This page describes the components and the python engine and the operational process.


# Details #

## operational engine ##

  * Analysis

> runs the ocean model forced with anlysis or real data (surface and boundary forcings)

  * Forecast

> runs the model froced with predictions


## operational cycle ##

  1. check/wait for the required forcing and initial conditions
  1. creation of model input files
  1. ocean simulation
  1. plot/manage model input/output

The cycle is repeated continuously. Ocean model initial conditions come from the restart file of the previous day analysis simulation


## modules ##

  * op\_main
> > maintenance of the analysis and forecast cycles

  * op\_vis
> > visualization of model input/output

  * op\_clean
> > delete/compress input/output files

  * op\_monitor
> > access the status of the model runs

the modules include text configuration files