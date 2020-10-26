# Cell Profiler Pipe Lines

This folder contains the Cell Profiler pipe lines that are used to extract biologically relevant information from the flourescence images. There is one pipe line for each magnification. 

<img src="cp_pipeline.png" align="center" >

To run the pipeline go to https://cellprofiler.org/ and download the latest version of the software. The pipeline is run by importing the .cpproj-file into the software. The image folder needs to contain image triplets with the following naming convention:

```sh
AssayPlate_Greiner_#655090_D02_T0001F007L01A01Z01C01.tif
AssayPlate_Greiner_#655090_D02_T0001F007L01A01Z01C02.tif
AssayPlate_Greiner_#655090_D02_T0001F007L01A01Z01C03.tif
```
representing the three target channels for each well and field of view. The output from the pipe line is a csv-file which contains image features for all provided input images. 
