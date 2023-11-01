# ecgi
A simple ECGI solution using brute force methods.

Step 1:
Create a heart mesh using CT Data 
- Total Segmentator via Python API?
- 3D Slicer
Fill Myocardium with evenly spaced nodes in a coordinate system
- Research Filterung Algorithms/methods for Differentiation of myocardium and Rest
- Research methods to cut away the valves, and atriae

Step 2:
For each of the nodes run a complete depolarisation/repolarisation cycle
If there is reentry, run for 3 cycles (defined via time or via depolarisation of initial node)
For each run record amplitudes of XYZ vectors
- Research methods to simulate a Heart muscle cell cycle efficiently
- Research how to trigger depolarisation of neighboring Cella/nodes

Step 3:
For each vector loop calculate difference to observed vector loop of the patient
Best fit determines most probable depolarisation path

Step 4:
Draw selected loop on mesh with amplitude coloring


Research:
- What Python Library can do 3D Visualisation?
- Plan data storage to fit this library

https://docs.enthought.com/mayavi/mayavi/example_heart.html
