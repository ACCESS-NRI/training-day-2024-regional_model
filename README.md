# ACCESS-NRI Training Day 4 September 2023

This repository includes the material for the <a href="https://www.access-nri.org.au" target="_black">ACCESS-NRI</a> <a href="https://www.access-nri.org.au/event/access-training-day-2023/" target="_black">Training Day</a> on 4 September 2023.  
You can find a general overview of the ACCESS-NRI documentation on the <a href="https://access-hive.org.au" target="_blank">ACCESS-Hive</a>.  

We value your feedback on this training, in-person or via the <a href="https://forum.access-hive.org.au/" target="_blank">ACCESS-Hive Forum</a>, as it will help us to provide better training and documentation for the ACCESS community on our documentation portal, <a href="https://access-hive.org.au" target="_blank">ACCESS-Hive</a>.

## Structure of this repository (see <a href="https://www.access-nri.org.au/access-training-day-program/" target="_blank">Training Day program</a>)

Instructions on which NCI project you need to be part of and how to launch the <a href="https://are.nci.org.au" target="_blank">ARE</a> (Australian Research Environment) are provided at the beginning of each exercise:

1. ACCESS Models:  
   a) [Exercise: Running ACCESS in ARE](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/access_rose_cylc/rose_cylc_example.md)  
   b) [Exercise: Working with an ACCESS suite](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/access_rose_cylc/ex1_runlength.md)  
   c) [Exercise: How to modify suites](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/access_rose_cylc/ex2_co2.md) <br>
   d) [Exercise: Troubleshooting example](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/access_rose_cylc/ex3_troubleshooting.md)
3. ACCESS-NRI Intake Catalog:  
   a) [Exercise: Getting set up on the ARE](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/intake/ARE_setup_guide.md)  
   b) [Exercise: Using the ACCESS-NRI Intake catalog](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/intake/Intake_tutorial_p1.ipynb)  
   c) [Exercise: Indexing a new model run](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/intake/Intake_tutorial_p2.ipynb)
4. [Exercise: Working with ILAMB](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/ilamb/ILAMB_training.md)
5. [Exercise: Working with ESMValTool](https://github.com/ACCESS-NRI/workshop-training-2023/blob/main/esmvaltool/ESMValTool_training_VDI.md)

Remember that you have to be part of the projects that are listed at the beginning of each exercise.

Please <a href="https://my.nci.org.au/mancini/" target="_blank">join</a> them before the workshop - most importantly `nf33` - and list them in the storage instructions of your ARE session, as per exercise instructions.

## Cloning this repository

For the training on Intake, ILAMB and ESMValTool, you will need to clone a local copy of this repo to <i>Gadi</i> as follows: 

1. Log in to <i>Gadi</i> via the command line of your preferred terminal using your NCI username and password.

   ```bash
   ssh <your_nci_username>@gadi.nci.org.au
   ```

   For example, you could use the **Gadi Terminal** app provided after logging in to the <a href="https://are.nci.org.au" target="_blank">ARE</a>.
   
2. Clone this Github repo to your user directory within `/scratch/nf33` on <i>Gadi</i>. Depending on whether or not you've used the nf33 project before, your user directory may or may not already exist.

   ```bash
   mkdir -p /scratch/nf33/$USER
   cd /scratch/nf33/$USER
   git clone https://github.com/ACCESS-NRI/workshop-training-2023.git
   ```
