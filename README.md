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
