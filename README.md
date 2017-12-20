[![DOI](https://zenodo.org/badge/114890430.svg)](https://zenodo.org/badge/latestdoi/114890430)


# Multiple list learning task
PsychoPy implementation of a multiple wordlist learning task for demonstrating the backward and forward effects of testing (testing effects).

# Author
Marc Beardsley, Pompeu Fabra University, Barcelona, Spain

Contact marc.beardsley@upf.edu with any comments or questions

# Task Description
This is a PsychoPy (Peirce, 2009) implementation of a multiple-list learning task described in Pastötter et al. (2011) and Szpunar et al. (2008). The number of lists in the implementation is three rather than five of the original studies.

The multiple-list learning study assesses working memory performance and is used to demonstrate both the backward and forward effects of testing.

Participants are asked to study a list of words, presented one-by-one, in preparation for a final cumulative test. There are three lists and sixty words in total. Each list has twenty words and is followed by two activities - a backwards counting activity and either a restudy or retrieval activity. After the third list activities, a 3-back task is completed prior to the taking of the final cumulative test. Participants type as many of the sixty words they can remember, in any order, during the final cumulative test (e.g. a free recall test).

In the retrieval condition, participants complete a recall activity after each backwards counting activity. For 60s, participants are instructed to type as many words they can recall, in any order, from the list preceding the activity.

In the restudy condition, participants complete a restudy activity after list 1 and list 2, and then a recall activity after list 3. For the restudy activity, participants are shown all 20 words from the preceding list for 60s and are instructed to study the list in preparation for the final test. After list 3, the recall activity is the same free recall test as in the retrieval condition.

Spanish version: The target material consisted of three lists of 20 Spanish words that were drawn from the free EsPal online repository (Duchon et al., 2013).

# Usage Notes
The task uses the keyboard for participant input. 

Once started, a prompt will appear to input a participant ID, which is used for naming the output files. The output files (log files and .csv files) include L3 and final recall test answers. PsychoPy will create a Data/ directory in the current directory to store participant responses. Responses will be stored in a file whose name includes the participant ID entered and the data and time the experiment was started.

The experiment runs automatically with each screen having a time limit - facilitating the syncing of physiological measures (e.g. EEG, EDA).

A Spanish and an English version of the experiment are included in the files. 

# License
Licensed under the GNU General Public License v3.0.
https://www.gnu.org/licenses/gpl.txt 

This project is licensed under the GNU General Public License v3.0.
Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.

# Getting Started
These instructions will get you a copy of the experiment up and running on your local machine.

### Prerequisites
PsychoPy 1.85.4 (http://psychopy.org/installation.html)

### Installing
Download the experimental files and open the .psyexp files in PsychoPy.
Trial_A is the retrieval condition
Trial_B is the restudy condition

### To edit the word lists
1. Edit the words shown in the encoding periods (e.g. display of words one by one). Open and edit files memory_test_a.csv, memory_test_b.csv, memory_test_c.csv

2. Edit the review activity after L1 and L2. Open Trial_B.psyexp. Go to Review1 and Review2 boxes. Edit Review_Words component to input the new words. 

### Getting the data
Trial data is written to a .csv file and log file in the /data directory of the experimental folder.

# References
Duchon, A., Perea, M., Sebastián-Gallés, N., Martí, A., & Carreiras, M. (2013). EsPal: One-stop shopping for Spanish word properties. Behavior research methods, 45(4), 1246-1258.

Pastötter, B., Schicker, S., Niedernhuber, J., and Bäuml, K.-H. T. (2011). Retrieval during learning facilitates subsequent memory encoding. J. Exp. Psychol. Learn. Mem. Cogn. 37, 287–297. doi: 10.1037/a0021801

Peirce JW (2009) Generating stimuli for neuroscience using PsychoPy. Front. Neuroinform. 2:10. doi:10.3389/neuro.11.010.2008

Szpunar, K. K., McDermott, K. B., and Roediger, H. L. III (2008). Testing during study insulates against the buildup of proactive interference. J. Exp. Psychol. Learn. Mem. Cogn. 34, 1392–1399. doi: 10.1037/a0013082

# Citing these materials
Beardsley, M. (2017). Multiple-list learning task PsychoPy implementation. doi: 10.5281/zenodo.1120260
