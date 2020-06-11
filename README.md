# Useful scripts
Here are some useful scripts shared within THGLab

## vmd.rc
This is the VMD configuration file that supports some enhanced functionality
### Install
* For Windows systems, copy the configuration file to the VMD installation path (Default position should be `C:\Program Files (x86)\University of Illinois\VMD`)
* For Linux and Mac systems, rename the file as `.vmdrc` and save the file in the home folder

### Functionality
After putting this run commands file into the correct position, you will have the following functionalities and key bindings:
* Newly loaded files will by default show with NewCartoon representation and colored by secondary structure
* q: quit VMD
* x: delete the last molecule
* m: remove last representation on the last molecule
* n: open new file menu
* s: open save structure menu
* p: open representation menu
* d: open render menu
* u: open RMSD Trajectory Tool menu
* v: open Sequence Viewer menu
* w: show representation for non-protein molecules (i.e. water and ligand) using CPK and color by elements for the last molecule
* i: show structure in CPK representation and color by elements for the last molecule
* a: show protein as a single backbone line colored by index for the last molecule

## LRC_scripts
These are some scripts for easily submitting jobs or run jobs interactively on LAWRENCIUM cluster
### Install
1. Copy the folder to your LAWRENCIUM home folder
2. Add this folder to the bash run script: i.e. run `echo "export PATH=$HOME/LRC_scripts:$PATH" >> ~/.bashrc`
3. To make this work for the current shell, run `source ~/.bashrc`
4. Go into the folder and add execution permissions for the files `chmod u+x *`

### Functionality
* These scripts allow you to type `comp` to get into a computing node (under NinjaOne cluster) and `comp gpu` to get into a GPU computing node with 2080Ti GPUs. The default time limit for interactive jobs are set to 4 hours.
* You can use `submit` to submit jobs on LAWRENCIUMs with some pre-defined parameters, or `submit gpu` to submit GPU jobs. You will be prompted to enter a one-line command for running the job (when you leave it empty, the job command will be the same as last command). You can then specify the resources needed for the job or leave it as default. Type "y" or "yes" to submit the job to the queue.
