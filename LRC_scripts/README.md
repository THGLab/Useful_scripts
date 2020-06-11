# LRC_scripts
These are the scripts that help with submitting jobs or getting into the computing nodes on LAWRENCIUM cluster.

## Install
1. Copy the folder to your LAWRENCIUM home folder
2. Add this folder to the bash run script: i.e. run `echo "export PATH=$HOME/LRC_scripts:$PATH" >> ~/.bashrc`
3. To make this work for the current shell, run `source ~/.bashrc`
4. Go into the folder and add execution permissions for the files `chmod u+x *`

## Functionality
* These scripts allow you to type `comp` to get into a computing node (under NinjaOne cluster) and `comp gpu` to get into a GPU computing node with 2080Ti GPUs. The default time limit for interactive jobs are set to 4 hours.
* You can use `submit` to submit jobs on LAWRENCIUMs with some pre-defined parameters, or `submit gpu` to submit GPU jobs. You will be prompted to enter a one-line command for running the job (when you leave it empty, the job command will be the same as last command). You can then specify the resources needed for the job or leave it as default. Type "y" or "yes" to submit the job to the queue.
