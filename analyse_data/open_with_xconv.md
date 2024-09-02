# ACCESS-NRI Workshop regional model examples
<p>Guide for the regional model ACCESS-NRI workshop exercises.</p>


# Exercise 1:  Open a FieldsFile with xconv
The standard output for the Unified Model is in FieldsFile format.

To open a FieldsFile file and inspect the contents visually, do the following


```
module use ~access/modules
module load xconv
```

go to an output directory of interest and list the files

```
cd /scratch/nf33/<user>/cylc-run/u-dg768/share/cycle/20220226T0000Z/Lismore/d0198/RAL3P2/um/
ls

```

then run

```
xconv umnsaa_pb000
```

A window will pop-up displaying the contents of the fieldsfile.

Double-click on "PRESSURE AT MEAN SEA LEVEL"

Click on the "t" (time) dimension.

Double-click on a single time.

Click on Apply.

Click on Plot Data.

A plot will appear on the screen showing the contents of the data selected.

## [Exercise 2:  List contents of a fields file](list_file_contents.md)
