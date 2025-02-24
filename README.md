# Generating PDF presentation from Inkscape layers

## Description

This repository provides a Python script that generates a PDF based on the 
layer(s) contained in an Inkscape SVG file. 

## Execution

The script should be executed from a folder containing the Inkscape SVG file 
named ***presentation.svg***. The script will first convert the layers into 
SVG files (stored in a temporary folder ***temp*** that will be removed at the 
end of the process). This firt step is based 
on https://github.com/james-bird/layer-to-svg. The script will then convert the 
individual SVG files into PDF files. The PDF files will be eventually merged in 
a file ***presentation.pdf***.

You can run the scripts using the command:

**python3 inkpres.py**

If you need help, find a bug, want to give me advice or feedback, please contact me!

## Repository mirrors

This repository is mirrored on both GitLab and GitHub. You can access it via the following links:

- **GitLab**: [https://gitlab.com/maximelenormand/inkscape-presentation](https://gitlab.com/maximelenormand/inkscape-presentation)  
- **GitHub**: [https://github.com/maximelenormand/inkscape-presentation](https://github.com/maximelenormand/inkscape-presentation)  

The repository is archived in Software Heritage:

[![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/maximelenormand/inkscape-presentation/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/maximelenormand/inkscape-presentation)