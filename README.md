# Final Assignment EIO2
## Jaap Abbring and Tobias Klein

You will complete this assignment in two stages. You will first, together with us, develop a short proposal. Then, independnetly, you will execute this proposal.

## Stage 1. Proposal 

Deliverable: A one-page file `proposal.pdf` that 
- specifies a research question, 
- identifies a paper with a dynamic structural model that is suitable for answering this question, and 
- outlines a "bare-bones" version of this model that captures the application's essential mechanisms but leaves out all complicating details.

Please check out our example proposals covering [teacher incentives in India](), [occupation choice](), and [childcare and female labor supply]().

Some directions:
- You will _not_ use real data, only data you simulate yourself from the model.
- Include a permanent (`doi`) link in your reference to the paper, so that we can easily check it out.
- Check out the example proposals 

## Stage 2. Execution 

Deliverables: A `pdf` file discussing your results and the code that produces them. 

### Results
The `pdf` file discussing your results should read like a paper (i.e., full sentences, typeset formulas, no code, etc.) and have six sections that
1. introduce the research question and the paper you build on (this can be taken from your proposal),
2. completely describe your bare-bones model (this completes the outline in your proposal),
3. detail how you (numerically) solve this model,
4. specify how and for which parameter values you generated data from the model, 
5. describe your estimator of the parameters and its implementation and present your estimation results, and
6. conclude by briefly reflecting on your results and discussing what else is needed to answer your research question (apart from real instead of simulated data; for example, particular counterfactual analyses using the estimated model). 

Because you work with simulated data, you can explore how well your estimation approach would work in different data settings. At a minimum, estimate your model for three simulated data sets of different size: many observations so that estimates are very close to the true values, very few observations so that estimates are relatively far away because of estimation error, and a situation somewhere inbetween. If time permits, you may also run a full Monte Carlo in which you assess the accuracy of the asymptotic approximations (again varying the number of observations).

Make sure to also commit the `tex` file to the repository and also commit any tables and figures that are produced by the code and that you use in the PDF document in a folder `analysisResults`.

### Code 
At its core, the code provides procedures for solving the model, simulating data, and estimating the parameters of the model. Then, the code either includes a single main script for reproducing all the reported results (as in our [DDC package](https://ddc.abbring.org)) or e.g. a `makefile` with instructions for the `make` utility to reproduce all results.  Please make sure to set a seed, so that we can exactly reproduce the results. 
