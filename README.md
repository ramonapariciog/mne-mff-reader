# mne-mff-reader  BETA

MNE Class and functions for loading the EGI '.mff' files from EGI Netstation EEG. 

# Install

Clone the package and copy the folder into your mne current folder:

.../mne/io/

# How to import

only with this line:

from mne.io.mff import read_egi_mff

and for create the raw instance:

raw = read_egi_mff(filepath, exclude, include, verbose)

All the pararameters are the same than for the read_raw_egi.


# Limitations:

1.- At this moment doesn't support multisubject records, but can be adapted for that.

2.- At the moment has been tested by comparing the results with the obtained by a single subject and notsegmented record raw file.

3.- At the moment all data is loaded to memory, using the preload=True mode.


# Thanks to PhD. Guillaume Dumas, PhD. Dennis A. Engeman & PhD. Sheraz Khan
