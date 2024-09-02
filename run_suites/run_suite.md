# ACCESS-NRI Workshop rose cylc examples
<p>A simple suite to test that things are working.</p>

#  Running the example suite

Start a terminal in the VDI session (from icon at top left).

Note that pasting externally copied text into the VDI terminal is quite awkward. See https://github.com/ACCESS-NRI/workshop-training-2023/issues/22 for a workaround.

```
module use /g/data/hr22/modulefiles
module load cylc7
```

NCI persistent sessions allow a cylc server to keep running after your login session (e.g. for long running climate suites).
https://opus.nci.org.au/display/DAE/Persistent+Sessions+For+Cylc+Jobs

```
persistent-sessions start cylc
```

If you have a MOSRS account

```
mosrs-auth
rosie co u-dg767
rosie co u-dg768
```
This checks out a copies of the ancillary and nesting suites to `~/roses/u-dg767` and .`~/roses/u-dg768`

In this tutorial we will not run the u-dg767 suite due to timing constraints, but lets view the suite together.

```
cd ~/roses/u-dg767
rose edit
```

We will run the nesting suite.  To view the nesting suite

```
cd ~/roses/u-dg768
rose edit
```

To run the nesting suite do the following:
```
cd ~/roses/u-dg768
rose suite-run
```

The suite will take about 1 hour per +24 hours using 18 by 16 CPUs at a cost of roughly 1000SU

## Suite output
The model output and log files can be checked directly on the file system. E.g.

Note that the whole `cylc-run/SUITE` directory is on `/scratch` and linked to `$HOME`.

## Model run directory
Tasks run in a `/scratch/PROJECT/USER/cycle-run/SUITE/share/cycle/CYCLE_TIME/` subdirectory and by default input and output files will be there. 
