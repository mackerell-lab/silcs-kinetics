# silcs-kinetics
This is the repository for SILCS-Kinetics ML models that are described in our paper:

"High Throughput Ligand Dissociation Kinetics Predictions using Site-Identification by Ligand Competitive Saturation"

For a new protein, SILCS simulation is required to initialize the protocol. 
The SILCS software to calculate the FragMaps is available free of charge to educational institutions through the SilcsBio LLC (https://silcsbio.com/).
After production of SILCS FragMaps, SILCS-Pathway is used to generate ligand dissociation pathways. SILCS-Pathway workflow and executables are available at: https://github.com/mackerell-lab/silcs-pathway.
Then for each pathway cluster, SILCS-MC samplings for each ligand can be conducted. Again, the SILCS-MC code is available free of charge to educational institutions through the SilcsBio LLC.
Upon acquisition of LGFE and IE energy profiles, the SILCS-Kinetics ML models can be used to predict -logkoff values.
Two types of ML models are present in two subdirectories: "tree" and "rnnmlp". Please check the "README" file in each subdirectory for more details.
