# Hackathon Evaluation Metrics

In this notebook we provide the functions that are used to calculate the quantitative evaluation metric for each magnification in the data set. The quantitative evaluation metric used to assess the hackathon contributions is divided into two parts: The images are compared using the mean absolute error (MAE) between generated and ground truth images using 1) features extracted by the CellProfiler and 2) pixel values.  

<img src="evaluation_pipe_line.PNG" align="center" >

These are averaged to yield the final metric value. The evaluation suite in the provided notebook will be run on each magnification seperately and the final metric is given by the weighted average

\begin{equation*}
\mathrm{MAE}_\mathrm{tot} = \frac{1}{n_\mathrm{tot} }\left( n_{20x}\mathrm{MAE}_{20x} +  n_{40x}\mathrm{MAE}_{40x} +  n_{60x}\mathrm{MAE}_{60x} \right)
\end{equation*}

```math
\mathrm{MAE}_\mathrm{tot} = \frac{1}{n_\mathrm{tot} }\left( n_{20x}\mathrm{MAE}_{20x} +  n_{40x}\mathrm{MAE}_{40x} +  n_{60x}\mathrm{MAE}_{60x} \right)
\end{equation*}
```

where $n_\mathrm{tot}$ and $n_{20x}/n_{40x}/n_{60x}$ is the number of images in the total and $20x/40x/60x$ data set respectively. 


