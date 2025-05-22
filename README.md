# Coloring Les Mis
This repository contains some of the code that was created for my master's thesis in engineering at Uppsala university. The thesis is called "Coloring Les Mis-A Multilayer Network Approach for Modeling and Characterizing Interpersonal Relationships".
## Setup
1. install requirements listed in requirements.txt
2. 'tendimension' is a NLP-tool called by the file 'ttn_to_mttn'. Instruction to set up the tool: https://github.com/lajello/tendimensions.
## Files and Folders
'Data/les_mis_dataset.csv' contains the subtitle, speaker, recipients, and time of every utterance in the movie Les Misérables(1998).

'Data/ttn_nets' contains temporal text networks created from 'les_mis_dataset.csv'

'Data/multilayer_message_networks' contains various multilayer message networks derived from 'Data/ttn_nets/mttn.txt'

'Data/multilayer_cosial_networks' contains various multilayer social networks derived from 'Data/ttn_nets/mttn.txt'

The notebooks contains the code that was used to create the different networks.

## Author
Erik Blomsterberg
