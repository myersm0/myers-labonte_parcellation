## Supplementary materials for "Functional parcellation of the neonatal brain"
### by Michael Myers, Alyssa Labonte et al

The main object, the parcellation file in FSLR 32k space, is `elabe_parcels_n131_height0.5.dlabel.nii`, a [CIFTI](https://www.nitrc.org/projects/cifti/) dense label file containing 283 parcels on the cortical surface.

Several files included here complement the dlabel file above:
- `parcel_assignments.txt` is a list of functional network assignments for each of the 283 parcels in ascending numerical order
- `parcel_centroids.csv` is a tabular file containing the vertex number of the centroid for each parcel, along with the xyz coordinates of that vertex (with respect to the Conte69 32k surface atlas)
- `network_info.csv` is a tabular file listing the distinct integer network assignments, along with supplementary information such as RGB color values

The parcellation code is available [here](https://github.com/myersm0/WatershedParcellation.jl), a Julia adaptation of the original MATLAB code from Evan Gordon and Tim Laumann.

![Parcels](https://github.com/myersm0/myers-labonte_parcellation/blob/main/consensus_modified_very-inflated.png "Parcels colored by network assignment")
