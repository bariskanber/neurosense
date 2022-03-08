Neurosense is a trained neural network for identifying full or near-full coverage head/brain scans in large human magnetic resonance image datasets.

# Quick Start Guide
 
## Preamble

Neurosense comes in the form of an Ubuntu Virtual Machine, which has FSL pre-installed. Therefore, its use is conditional on your agreement of the FSL software license available at https://fsl.fmrib.ox.ac.uk/fsldownloads_registration. You do not need to download FSL itself as it has been pre-installed. However, make sure you read and agree to the terms of the FSL software license before using Neurosense.
 
## Requirements

You will need VirtualBox to run the Neurosense virtual machine. If you do not already have VirtualBox, download and install it for your platform from https://www.virtualbox.org/wiki/Downloads
 
## Installation and Use

* Download *Neurosense_v0.3.ova* from [this link](https://liveuclac-my.sharepoint.com/:u:/g/personal/rmapkan_ucl_ac_uk/ET1xs2mw7-lMt3OFa6cNlnQBjYfpzWaWSbfxk_hBD5yx0w?download=1) (password: `neurosense`) and save it in an appropriate location. **It is recommended that all work is carried out in an encrypted, safe environment if you will be using Neurosense on sensitive data.**
 
* Start VirtualBox, and choose `File/Import Appliance` to import *Neurosense.ova*
 
* Once imported, `right click` on Neurosense in VirtualBox and choose `Settings`.
​
* Within `Neurosense – Settings` click on `Shared Folders` and click the small add icon on the right.
 
* Within the `Add Share` dialog, choose the folder where the NIFTI volumes you would like to run through Neurosense are located. 

* Put `myfolder` for `Folder Name` and check `Auto-mount`.

* Start the virtual machine and login as user `neurosense` (password: `neurosense`)
 
* Type the following commands to make sure you can see your files/folders: `ls /media/sf_myfolder`
​
* Type the following commands to run Neurosense on your files/folders: `neurosense /media/sf_myfolder`
​
## Notes
* You can add `--pdf` as a parameter if you would like Neurosense to produce a Pdf report. 
* You may wish to check your VirtualBox settings to ensure you have enough computing resources available to Neurosense.
* Neurosense has been trained primarily using T1-weighted MRI volumes, performance on MR volumes of other contrasts and non-MRI volumes will be degraded.
* Any queries can be sent to [b.kanber@ucl.ac.uk](mailto:b.kanber@ucl.ac.uk).

## Sample Output
<img width="556" alt="SampleOutput" src="https://user-images.githubusercontent.com/12815964/157304777-d7a9b85d-8224-4165-9003-4da43edbfe76.png">

## Acknowledgements
If you use Neurosense for your research, please acknowledge our publication below:

Kanber, B., Ruffle, J., Cardoso, J. et al. Neurosense: deep sensing of full or near-full coverage head/brain scans in human magnetic resonance imaging. Neuroinform (2019) doi:10.1007/s12021-019-09442-x

## Notices
Commercial use is not allowed without explicit permission.
