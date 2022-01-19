Generating pdf presentation from Inkscape layers
===================================================================================

This python script generates a pdf based on the layer(s) contained in an Inkscape svg file. The script should be executed from a folder containing the Inkscape svg file named ***presentation.svg***. The script will first convert the layers into svg files (stored in a temporary folder ***temp*** that will be removed at the end of the process). This firt step is based on https://github.com/james-bird/layer-to-svg. The script will then convert the individual svg files into pdf files. The pdf files will be eventually merged in a file ***presentation.pdf***.
 
It was tested on Ubuntu 20.04 with Inkscape 1.1.
  
If you need help, find a bug, want to give me advice or feedback, please contact me!
You can reach me at maxime.lenormand[at]inrae.fr
