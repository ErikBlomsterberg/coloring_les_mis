# Coloring Les Mis
This repository contains a dataset, networks, and some of the code that was created in relation to my master's thesis in engineering at Uppsala university. The thesis is called "Coloring Les Mis - A Multilayer Network Approach for Modeling and Characterizing Interpersonal Relationships"(will be properly referenced once it is uploaded). I refer to the thesis for a detailed description of the process for creating the dataset.  

## Files and Folders
'data/les_mis_dataset.csv' contains the subtitle, speaker, recipients, and time of every utterance in the movie Les Misérables(1998).

'data/ttn_nets' contains temporal text networks created from 'les_mis_dataset.csv'.

'data/flat_ttn_nets' contains one flat ttn for each layer in 'data/ttn_nets/mttn.txt'.

'data/multilayer_message_networks' contains various multilayer message networks derived from 'data/ttn_nets/mttn.txt'.

'data/multilayer_social_networks' contains various multilayer social networks derived from 'data/ttn_nets/mttn.txt'.

'srt_to_csv_and_more.ipynd' contains the code that was used for constructing the Les Misérables(1998) dataset.

Notebooks(except 'srt_to_csv_and_more.ipynd') contains the code that was used to create the different networks.

## Setup
#### To run notebooks(except 'srt_to_csv_and_more.ipynd') :
1. Unzip 'data.rar' to access networks and Les Misérables(1998) dataset.
2. pip install -r requirements.txt (may contain packages that are not needed).
3. Set up the NLP-tool 'tendimension'(called in 'ttn_to_mttn.ipynb') by following the instructions provided here: https://github.com/lajello/tendimensions.
4. Replace "print("Vocab size: %d" %len(self.model.vocab))" on line 76 in 'tendimensions/features/embedding_features.py' with "print("Vocab size: %d" %len(self.model.key_to_index))" to make 'tendimensions' work. 
#### To run 'srt_to_csv_and_more.ipynd':
1. Download a SRT-file
2. Adjust path names in 'srt_to_csv_and_more.ipynd'.
## Author
Erik Blomsterberg
