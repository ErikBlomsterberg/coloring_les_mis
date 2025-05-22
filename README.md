# Coloring Les Mis
This repository contains some of the code that was created in relation to my master's thesis in engineering at Uppsala university. The thesis is called "Coloring Les Mis-A Multilayer Network Approach for Modeling and Characterizing Interpersonal Relationships".

## Files and Folders
'Data/les_mis_dataset.csv' contains the subtitle, speaker, recipients, and time of every utterance in the movie Les Misérables(1998).

'Data/ttn_nets' contains temporal text networks created from 'les_mis_dataset.csv'.

'Data/multilayer_message_networks' contains various multilayer message networks derived from 'Data/ttn_nets/mttn.txt'.

'Data/multilayer_cosial_networks' contains various multilayer social networks derived from 'Data/ttn_nets/mttn.txt'.

The notebooks contains the code that was used to create the different networks.

## Setup
1. Unzip data.rar to access networks and Les Misérables(1998) dataset. 
2. pip install -r requirements.txt (may contain packages that are not needed).
3. Set up the NLP-tool 'tendimension'(called in 'ttn_to_mttn.ipynb') by following the instructions provided here: https://github.com/lajello/tendimensions.
4. Replace "print("Vocab size: %d" %len(self.model.vocab))" on line 76 in 'tendimensions/features/embedding_features.py' with "print("Vocab size: %d" %len(self.model.key_to_index))" to make 'tendimensions' work. 

## Author
Erik Blomsterberg
