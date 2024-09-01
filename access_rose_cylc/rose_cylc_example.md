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
persistent-sessions start cylc-test
```

[Running Example Suite](https://opus.nci.org.au/display/DAE/Cylc+7+suite+run+example%3A++u-cq161)

This is a simple suite that runs a couple of short jobs to test connectivity

If you have a MOSRS account

```
mosrs-auth
rosie co u-cq161
```
This checks out a copy of the suite to `~/roses/u-cq161`.

If you do not have a MOSRS account but are a member of the `ki32_mosrs` project
```
mkdir -p ~/roses
cd roses
svn co file:///g/data/ki32/mosrs//roses-u/c/q/1/6/1/trunk u-cq161
```

If all else fails
```
mkdir -p ~/roses
cp -r /g/data/access/nri_training/u-cq161 ~/roses
```

```
cd ~/roses/u-cq161
rose suite-run
```

You should now see something like this
<p align="center"><img src="../assets/access_rose_cylc/vdi_cylc_run.png" alt="drawing" width="80%"/></p>

This should only take a few minutes to complete. Note that tasks disappear from the GUI after they and their successors complete, so at the end of a successful run you'll be left with an empty GUI.
<p align="center"><img src="../assets/access_rose_cylc/cylc_complete.png" alt="drawing" width="80%"/></p>

## Suite output
The model output and log files can be checked directly on the file system. E.g.
<p align="center"><img src="../assets/access_rose_cylc/suite_output_files.png" alt="drawing" width="80%"/></p>

Note that for suites launched from ARE, the whole `cylc-run/SUITE` directory is on `/scratch`, not just the `work` and `share` subdirectories.

## Model run directory
Tasks run in a `work/CYCLE_TIME/TASK_NAME` subdirectory and by default input and output files will be there.
