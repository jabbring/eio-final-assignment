# Final Assignment EIO2
## Jaap Abbring and Tobias Klein

In this final assignment, you will find a paper that empirically studies an interesting (to you) problem using a dynamic model (possibly one with strategic interactions). You will specify a version of this model that captures its essential (to a question of your choice) mechanisms but leaves out all complicating details. You will numerically solve this "bare-bones" model, simulate data from it, and estimate its parameters using the simulated data. You will also discuss how you could answer your chosen question if you would have estimated the model with real data.

You will complete this assignment in two stages. You will first, together with us, develop a short proposal. Then, independently, you will execute this proposal.

## Github
From the very beginning, please work in your Github repository. Commit often. Also commit the PDF files `proposal.pdf` and `report.pdf` to the repository.

## Stage 1. Proposal 

**Deliverable**: A one-page file `proposal.pdf`. You can generate it using the [proposal template](proposal.tex) or any other way you like (in that case please still follow the structure in the template). The proposal
- identifies a paper in any field of economics, finance, or marketing that uses a dynamic structural model (include a link to this paper), 
- specifies a concrete research question that can be answered using this model, 
- outlines a bare-bones version of the model that is just rich enough for a nontrivial analysis of this question, and 
- specifies the type of data that will be simulated to estimate it (these do not have to be the type of data used in the paper).

Examples of such proposals: [teacher incentives](examples/proposalTeachers.pdf), [occupation choice](examples/proposalOccupation.pdf), and [childcare subsidies](examples/proposalChildcare.pdf).

## Stage 2. Execution 

**Deliverables**: A complete package that contains
- a report,
- code,
- a script that runs the code and produces the report.

### Report
The report should be in PDF format and should be saved under the name `report.pdf`. It should read like a paper (i.e., full sentences, typeset formulas, no code, etc.) and should have six short sections that
1. introduce the research question and the paper you build on (this can be taken from your proposal),
2. completely describe your bare-bones model (this completes the outline in your proposal),
3. detail how you (numerically) solve it,
4. specify how you generated data from the model and which parameter values you used for doing so, 
5. describe your estimator of the parameters and its implementation and present your estimation results, and
6. conclude by briefly reflecting on your results and discussing what else is needed to answer your research question (apart from real instead of simulated data; for example, a particular counterfactual analyses using the estimated model, which you do _not_ have to provide). 

Regarding 4. and 5., at a minimum, please report estimates for three simulated data sets of different size: many observations so that estimates are very close to the true values, very few observations so that estimates are relatively far away because of estimation error, and a situation somewhere in-between. If time permits, you may also run and report on a full Monte Carlo exercise in which you assess the accuracy of the asymptotic approximations (again varying the number of observations).

### Code 
At its core, the code provides procedures for solving the model, simulating data, and estimating the parameters of the model. Please make sure to set a seed, so that the results are reproduced exactly. Please make sure the code produces all numbers and plots in the report in one go. That is, do not ask us to re-run the script several times and always changing a parameter. Instead, automate this. Keep the code compact and avoid duplication. See for instance [here](https://tilburgsciencehub.com/building-blocks/develop-your-research-skills/tips/principles-good-coding/) for advice.

### Script
The code either includes a single main script for reproducing all the reported results and compiling these and `report.tex` into `report.pdf`; or e.g. a `makefile` with instructions for the `make` utility to reproduce all results and `report.pdf`; alternatively, you can use for instance a MATLAB live script, an R markdown document, or a Jupyter notebook to produce `report.pdf`. Please make sure that it is clear what needs to be done to re-create that file, for example in a readme file.