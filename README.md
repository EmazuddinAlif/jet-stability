# jet-stability

## This repository contains all the files and codes pertaining to the paper "**Liquid jet stability through elastic planar nozzles**" (https://doi.org/10.1140/epjs/s11734-022-00656-w). Please contact Md. Emazuddin Alif (malif@vols.utk.edu) or Dr. Andrew Dickerson (adicker7@utk.edu) for further details and information. We request everyone using any portion of our code to appropriately cite the parent paper.



## CAD Models and Descriptions
- Base_plate.ipt : Base plate along which the linear stage connected to the relaxation chamber is held
- Connector_ring : 3D printed ring connecting the relaxation chamber to the membrane. On later iterations it was replaced with metallic flanges sourced from Home Depot
- encoder_coupler.ipt : Couples the encoder to the linear stage moving the relaxation chamber
- encoder_mount.ipt: Mounts the rotary encoder on the base plate
- Relaxation chamber holder.ipt : Connects the relaxation chamber to the linear stage
- Relaxation chamber outer holder.ipt : Clamps the relaxation chamber to the Relaxation Chamber Holder
- punch_holder.ipt : Holds the punch parallel to vertical in order to create clean circular nozzles
- laminizer.rld : Laminarizes the flow inside the relaxation chamber

## MATLAB Codes and Descriptions
- calibration.m : Calibrates the pixel distance in each video with real life physical units (here mm). The diameter of the relaxation chamber flange is taken as the refence for calibration
- calibration_looper.m : Loops through all the images taken of the flange in a particular folder for calibration

## BibTex

@article{alifLiquidJetStability2022a,
  title = {Liquid Jet Stability through Elastic Planar Nozzles},
  author = {Alif, Md Emazuddin and Veihdeffer, Julie and Alam, Md Erfanul and Dickerson, Andrew K.},
  year = {2022},
  month = sep,
  journal = {The European Physical Journal Special Topics},
  issn = {1951-6401},
  doi = {10.1140/epjs/s11734-022-00656-w},
  urldate = {2023-04-08},
  abstract = {An extensive number of processes require liquid jets such as cleaning, waterjet cutting, hydroentanglement, and atomization in combustion. The coherence and stability of the jet highly depend on the characteristics of the nozzle. Jet breakup lengths have been extensively studied for a multitude of nozzle characteristics and external stimuli, yet jets issuing from deformable, elastic nozzles have not been considered. In this study, we take the enduring topic of jet breakup into a new realm by introducing nozzles that passively deform when exposed to liquid flow by making an approximately 500 \$\$\textbackslash upmu \textbackslash hbox \{m\}\$\$orifice in thin sheets. We perform the experiments with nozzles of varying hardness and thickness, starting with a rigid BeCu nozzle, and continuing with shore hardness 70A, 65A, 35A and 20A. We observe nozzle dilation scales well with Reynolds number and that softer nozzles experiences greater dilation, as expected. We introduce a modification to linear stability theory to describe the break-up length of deformable nozzles to account for the dilation, a scaling which works best for our stiffer nozzles. The three softest materials provide the most stable jets through the range of flow rates in which they can operate before failure. For all nozzles, breakup is highly variable with time and jet velocity.},
  langid = {english},
  keywords = {Atomization,Deformable membrane,Linear stability,Nozzle dilation},
  file = {C:\Users\Emazuddin Alif\Zotero\storage\DV542TNR\Alif et al. - 2022 - Liquid jet stability through elastic planar nozzle.pdf}
}

- calibration_dia.m : Measures the diameter of the jet just as it is exiting the nozzle (in Pixels)
- calibration_dia_looper.m : Measures the diameter of the jet (in Pixels) for all the videos saved in the selected folder
- jet_breakup.m : Measures the breakup distance of the jet. (Optional) Recreates the video with jet breakup highl;ighted with a red line
- jet_breakup_looper.m : Measures the breakup distance of the jet of all the videos in the selected folder


