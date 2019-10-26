## Batch processing CTD data
### R/V John H. Martin
### Moss Landing Marine Labs

Tom Connolly - tconnolly@mlml.calstate.edu
October 26, 2019

Template for batch processing Seabird CTD data from the R/V John H. Martin. Includes example data from survey conducted near the head of Monterey Submarine Canyon conducted on September 24, 2019 (Physical Oceanography class cruise). 

Runs on Windows. Seabird Data Processing must be installed.

The setup files are for a configuration with a DeepSUNA sensor on voltage channel 4, and nitrate calculated in a user polynomial variable. This repository could be updated in the future with additional configurations.

#### Instructions

Open the Windows command prompt, navigate to the main directory that contains batch.txt. Run:

`SBEbatch batch.txt DATA_DIR CON_FILE`

* Replace DATA_DIR with the path to the directory that contains the raw .hex files.
* Replace CON_FILE with the path to the configuration file to be used. Include both the path and the file name.

#### Example

To process the example data, open the Windows command prompt, navigate to the main directory that contains batch.txt, and run:

`SBEbatch batch.txt CTD_example_data CTD_example_data\C1.xmlcon`