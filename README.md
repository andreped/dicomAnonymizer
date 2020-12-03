# dicomAnonymizer
Simple program (.exe) for anonymizing DICOMs.

## To use:
Simply run the executable. A file dialog will open. Choose the patient folder of interest. Click "Open". The program will start to run immediately. There will be created an anonymized folder at the same level as the selected patient folder. Thus, the original data will be kept untouched. While the program is running, a console should output prints for which scan it is currently working on. When the program is finished, the console will close.

## Expected Patient Folder Structure:
+-- {PATIENT_FOLDER}/
|   +-- Patient 1/
|   |   +-- Some_scans_folder/
|   |   |   +-- Scan 1/
|   |   |   |   +-- File 1
|   |   |   |   +-- File 2
|   |   |   |   +-- [...]
|   |   |   |   +-- File K

## Expected Directory Setup (excluding scans folder structure):
```
+-- {PATIENT_FOLDER}/
|   +-- Patient 1/
|   |   +-- Some_scans_folder/
|   |   +-- Images/
|   |   +-- Some_files_and_folder_to_be_neglected
|   |   +-- [...]
|   +-- Patient 2/
|   |   +-- Some_scans_folder/
|   |   +-- Images/
|   |   +-- Some_files_and_folder_to_be_neglected
|   |   +-- [...]
[...]
|   +-- Patient N/
|   |   +-- Some_scans_folder/
|   |   +-- Images/
|   |   +-- Some_files_and_folder_to_be_neglected
|   |   +-- [...]
``` 
