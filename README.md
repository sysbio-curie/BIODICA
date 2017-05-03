# BIODICA: Independent Component Analysis for BIg Omics Data

BIODICA is a user-friendly pipline for high-performant computation of independent components for omics data, 
using stability analysis and computing the optimal number of the components from their stabilities,
and performing analyses for interpreting the results of ICA application.

BIODICA can work as Graphical User Interface (GUI) or in the command line mode.

For installing BIODICA, clone the repository into a local folder, with all files, and check that the Java is installed.
It is recommended to update your Java installation to the latest version (Java 1.8 is required).

Current version of BIODICA requires MATLAB installed (will be changed to using MATLAB RunTime in the future).

For minimal configuration, edit the config file in the root folder, and change the 'MATLABFolder' parameter, specifying the path to MATLAB bin folder.
If you want to run the examples of the command line BIODICA uses ('cmdline_examples' folder), modify the 'cmdline_examples/config' file also.

To list all options for the command line use, execute

```
java -cp BIODICA_GUI.jar BIODICAPipeLine
```

Otherwise, launch the BIODICA GUI by executing

```
java -jar BIODICA_GUI.jar
```

##Tips and tricks:

It is not necessary to re-compute the ICA decomposition each time. Application of different procedures is possible for the results computed earlier, or even for the decompositions computed not with BIODICA.
For example, the toppgene analysis can be launched by executing
```
java -cp BIODICA_GUI.jar BIODICAPipeLine -config config -sfile [path_to_metagene_file] -dotoppgene
```





