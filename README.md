# Generating PDF Presentation from Inkscape Layers

## Description

This repository provides a Python script that generates a PDF based on the 
layer(s) contained in an Inkscape SVG file.

The script works as follows:

1. It converts each layer of an Inkscape SVG into individual SVG files stored in 
a temporary folder (`temp`). This step is based on 
[https://github.com/james-bird/layer-to-svg](https://github.com/james-bird/layer-to-svg).  
2. It converts each layer-SVG into a PDF using Inkscape.  
3. It merges all PDFs into a single output file.

By default, the script expects an input file named `presentation.svg` and 
produces an output file named `presentation.pdf`. Both the input and output 
can be customized with optional arguments.

The temporary folder (`temp`) is automatically removed at the end of the process.

## Usage

You can run the script using:

**python3 inkpres.py [--input 'path_to/svg_file'] [--output 'path_to/pdf_file']**

### Behavior

- **No arguments provided:**  
  Input defaults to `presentation.svg`, output defaults to `presentation.pdf`.

- **Only `--input` provided:**  
  Output will automatically be named after the input, replacing `.svg` with `.pdf`.

- **Only `--output` provided:**  
  Input defaults to `presentation.svg`. Output must have a `.pdf` extension.

- **Both `--input` and `--output` provided:**  
  Uses the specified input and output files. Output must have a `.pdf` extension.

The script validates:

- Existence of the input file.  
- Correct input (`.svg`) and output (`.pdf`) extensions.  
- Output folder creation if it does not exist.

## Repository mirrors

This repository is mirrored on both GitLab and GitHub. You can access it via the following links:

- **GitLab**: [https://gitlab.com/maximelenormand/inkscape-presentation](https://gitlab.com/maximelenormand/inkscape-presentation)  
- **GitHub**: [https://github.com/maximelenormand/inkscape-presentation](https://github.com/maximelenormand/inkscape-presentation)  

The repository is archived in Software Heritage:

[![SWH](https://archive.softwareheritage.org/badge/origin/https://github.com/maximelenormand/inkscape-presentation/)](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/maximelenormand/inkscape-presentation)
