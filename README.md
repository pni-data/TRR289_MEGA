# TRR289 MEGA Dataset

## ℹ️ Information
*This repository is the Github sibling of the corresponding [DataLad](https://www.datalad.org/) dataset, i.e. it **does not** contain the data itself.*
The GitHub sibling, nevertheless, provides insights into the general data structure (directory tree, filenames) and serves as a starting point to download, share and discuss the dataset.
Data follow the BIDS Extension proposal 35 (BEP035), BIDS-MEGA format and includes a collection of dataset from the TRR289 project for mega-analytic purposes.
The single BIDS datasets contained at the mega-analysis level are stored in [Coscine](https://coscine.rwth-aachen.de/) and can't be downloaded without the dataset specific secret token.
Token is available at project Z03 for members of TRR289 and collaborators upon reasonable request.

See `dataset_description.json` for project related meta-data and `bids_mapper.json` for mega-analysis level meta-data.

## ⬇️ How to download dataset

#### 1. Install it with DataLad based on the github handle
This does not download the actual data, only the gin-annex "skeleton".
```bash
datalad install -s git@github.com:pni-data/<dataset_name>.git <dataset_name>
```

#### 2. Change to the dataset directory and download the file(s) you want
You can selectively download what you need (e.g. derivatives only).
```bash
cd <dataset_name>
datalad get <path/to/file*>
```

For an explanation about how to get data from the single TRR289 datasets see our [documentation](https://github.com/pni-data/.github/blob/master/profile/README.md).

Comments added by the SFB289 Z03 project coordinators
====================================================================
General Comments
--------------------------------------------------------------------
ToDo link detailed information about the dataset.
eg: The sub-datasets were acquired by the teams of the TRR/SFB289. The whole mega-analysis dataset includes ?? subjects with the common sequences within the SFB289 project, namely a high resolution T1w, resting state fMRI, 133 direction multi shell DWI, and 2 fieldmaps for the functional data and one fieldmap for the DWI (reversed field encoding direction). An additional reference image of the resting state fMRI is included without multiband factor.

ToDo: Questionnaires data are also acquired and can be found in the ... folder.

The proposal can be found here: ToDo link

The BIDS conversion was done with heudiconv by the Z03 project coordinators.

Defacing
--------------------------------------------------------------------
Defacing was done by the Z03 coordinator.
Pydeface was used on all anatomical images to ensure de-identification of subjects. The code
can be found at https://github.com/poldracklab/pydeface


Known Issues
--------------------------------------------------------------------
N/A 

--------------------------------------------------------------------

## bids-validator
The bids-validator doesn't currently support the BIDS-MEGA format.
    