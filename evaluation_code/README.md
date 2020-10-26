# Hackathon Evaluation Metrics

In the provided notebook we give the functions that are used to calculate the quantitative evaluation metric for each magnification in the data set. The quantitative evaluation metric used to assess the hackathon contributions is divided into two parts: The images are compared using the mean absolute error (MAE) between generated and ground truth images using 1) features extracted by the CellProfiler and 2) pixel values.  

<img src="evaluation_pipe_line.PNG" align="center" >

These are averaged to yield the final metric value. The evaluation suite in the provided notebook will be run on each magnification seperately and the final metric is given by a weighted average as detailed in the notebook.  

IMPORTANT! To be able to compare target and generated images using the provided pipe-line, the images in the respective set need to adhere to the same naming convention. We recommend that the generated and target images are named identically to avoid errors in the evaluation suite. 