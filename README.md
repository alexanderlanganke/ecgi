# ecgi
A simple ECGI solution using brute force methods.

Step 1:
Create a heart mesh using CT/MRI Data 
Fill Myocardium with evenly spaced nodes in a coordinate system

Step 2:
For each of the nodes run a complete depolarisation/repolarisation cycle
If there is reentry, run for 3 cycles (defined via time or via depolarisation of initial node)
For each run record amplitudes of XYZ vectors

Step 3:
For each vector loop calculate difference to observed vector loop of the patient
Best fit determines most probable depolarisation path

Step 4:
Draw selected loop on mesh with amplitude coloring