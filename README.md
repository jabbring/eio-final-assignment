# Final Assignment EIO2
## Jaap Abbring and Tobias Klein

In this final assignment, you will 
- find an empirical application of the econometrics of dynamic discrete choices and/or games that fits your research interests,
- specify a "bare-bones" dynamic structural model that captures the application's essential mechanisms but leaves out all complicating details, and 
- develop and apply code to numerically solve this model, simulate data from it, estimate the structural parameters using simulated data.

You will complete the assignment in two stages, (1) proposal and (2) execution.

## Stage 1. Proposal 

Write a one-page proposal that specifies a research question, identifies a paper with a dynamic structural model that is suitable for answering this qeustion, and outlines your bare-bones version of this model. `proposal.tex` 


Find an empirical application of the econometrics of dynamic discrete choices and games that fits your research interests. This application may be in any field of economics, finance, or marketing. Ideally, propose a single paper that covers a question that interests you and that contains a dynamic structural model to answer it. 




in the literature that fits your research interests and propose a  dynamic structural model that captures its main features of interest to you, but . 




## Stage 2. Execution 
### Code 
The code solves the model, simulates data, and estimates the parameters of the model. 

Estimation can either be done for 3 simulated data sets of different size (many observations so that estimates are very close to the true values, very few observations so that estimates are relatively far away because of estimation error, and a situation somewhere in-between); or for some bonus points you can run a full Monte Carlo in which you also assess the accuracy of asymptotic approximations (varying again the number of observations).

Please set a seed so that we can reproduce the results. Also, please make sure that there is one main file that we need to run to reproduce all the results---a bit like for \href{https://ddc.abbring.org}{https://ddc.abbring.org}.

### PDF document
Please also write a PDF document with five sections that reads like a paper (i.e., full sentences, typeset formulas, no code, etc.).

The first section contains a complete description of the model. The second section contains a description of how you (numerically) solve the model. The third section describes how you generate data from the model, including a specification of the parameter values used in the simulations. The fourth section describes your estimator of the parameters and its implementation. It also discusses the results from estimating the parameters. The fifth section briefly reflects on your results and the possible application of the developed framework in your research. 

Please also commit the tex file to the repository and also commit any tables and figures that are produced by the code and that you use in the PDF document in a folder called ``analysisResults''.

### Grade 
50% of the grade is based on the code and 50% on the PDF document.
