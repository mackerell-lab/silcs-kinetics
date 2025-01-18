# silcs-kinetics
This is the repository for SILCS-Kinetics ML models that are described in our paper:

"High Throughput Ligand Dissociation Kinetics Predictions using Site-Identification by Ligand Competitive Saturation"

For a new protein, the SILCS simulations need to be performed and the FragMaps calculated to initialize the protocol. 
The SILCS software to perform the simulations and calculate the FragMaps is available the SilcsBio LLC (https://silcsbio.com/).
After production of the SILCS FragMaps, SILCS-Pathway is used to generate ligand dissociation pathways. SILCS-Pathway workflow and executables are available at: https://github.com/mackerell-lab/silcs-pathway. Then for each pathway cluster, SILCS-MC sampling for each ligand can be conducted using the SILCS-MC code available through SilcsBio LLC.
Upon acquisition of LGFE and IE energy profiles for a ligand, the SILCS-Kinetics ML models can be used to predict its -logkoff value.
Two types of ML models are present in two subdirectories: "tree" and "rnnmlp". Please check the "README" file in each subdirectory for more details.
