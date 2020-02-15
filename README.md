# SFND_Radar_Target_Generation_and_Detection

Implementation steps for the 2D CFAR process;
- calculation of the Bandwidth (B), Chirp Time (Tchirp) and Slope (slope) of the FMCW,
- transmitted, received and then beat signal generation,
- reshape of beat signal, calculating FFT of it and normalization,
- selection of guard and training cell sizes,
- noise level calculation and updating RDM according to determined threshold,
- suppressing non-thresholded cells

Selection of Training, Guard cells and offset;
- training and gurard cell sizes has been seleceted from varios performance test and best performing numbers are utilized.
- the offset has been selected from data.

Steps taken to suppress the non-thresholded cells at the edges;
- thresholded RDM elements has value either 1 or 0. So RDM has been looped and elements has value rather then 0 or 1 have been suppressed to 0.
