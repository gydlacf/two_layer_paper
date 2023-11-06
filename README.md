# two_layer_paper 

The repository of data for the paper titled _A
kinetic transition network model reveals the diversity of protein
dimer formation mechanisms_.

There are two folders in the repository, one containing the
description of the microstates (/states) and another containing the
description of the transition matrices. 

The file names follows the {pdbid}_{dissociation entropy} pattern. For
example, 1arr_87.0 contains the data for the 1arr PDB structure
calculated at $87\ \mathrm{\frac{J}{mol \cdot K}$.

## Microstates

Microstate files contain nine columns:
- the first column specifies the serial numbers of states
- the `fromA` and `toA` columns specify the start and end points of the
native section in the chain A
- the `fromB` and `toB` columns specify the start and end points of the
native section in the chain B
- the `inter` column specifies the numbers of interchain contacts
- the `weight` column specifies the Boltzmann weight of the states
- the `ass` column specifies whether the chains are associated
- the `native` column specifies whether the microstates belong to the
native state

## Transition matrices

Transition matrix files contain three columns:
- the `fr` column specifies the serial numbers of the tail nodes in the
transition graph
- the `to` column specifies the serial numbers of the head nodes in
the transition graph
- the `w` column specifies the weights of directed edges in the
transition graph
