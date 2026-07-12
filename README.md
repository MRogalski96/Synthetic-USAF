# Synthetic-USAF
Matlab code for generating synthetic USAF targets - it maintains the realistic dimensions of different USAF elements in relation to the selected pixel sampling

# How to use
Run the: <br>
[USAF, USAF_upsampled] = USAFgenerator(S, dx, upsmpl, usaf_groups, add_numbers); <br>
and it will generata a 'USAF' mask of the 'S' dimensions (e.g., S = [1000,1000] px) with a 'dx' pixel sampling (e.g., dx = 2 um). 'upsmpl' defines the accuracy with which each usaf element is generated. E.g., for upsmpl = 10, the USAF will be firstly generated as binary mask of the dimensions S*10 and pixel size dx/10, and in the final step downsampled to 'S' dimensions with 'dx' sampling - it means that the usaf elements will be generated with dx/upsmpl [um] (and 1/upsampl [px]) accuracy. 'usaf_groups' defines which usaf groups will be generated (e.g., usaf_groups = 4:9) and 'add_numbers' determines whether the group and elements numbers will be shown in the generated image (1 - yes, 0 - no)

# Demo
![](https://github.com/MRogalski96/Synthetic-USAF/blob/main/Synthetic_usaf_gif.gif) 


# Created by
Mikołaj Rogalski, <br>
mikolaj.rogalski@pw.edu.pl <br>
QCI lab, <br>
Warsaw University of Technology, Poland <br>
