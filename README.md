# Pre-CONN-fieldmap-and-fMRI-preparation
Everything that needs to be done with raw fieldmap and fMRI data from a SIEMENS scanner before inputting into CONN

This code was completed on a Windows machine using Ubuntu 22.04.5 LTS (GNU/Linux 6.6.87.2-microsoft-standard-WSL2 x86_64).
Code for Mac is unclear but using the none-script version line-by-line and making small adjustments should work. You may also need to run dos2unix this_script.sh before starting

PLEASE CHECK - This code assumes: NIFTI files, SIEMENS scanner, resting-state fMRI, DELTATE=2.46, DWELL=0.000689992, UNWARP_DIR="y-", total change in echo time=2.46.

To check change in echo time: "EchoTime" from the .json of XX_e2.ni.gz minus "EchoTime" from xx_e1.nii.gz. For example; 0.00738(e2)-0.00492(e1)=0.00246 seconds, or 2.46 milliseconds (command uses milliseconds).
