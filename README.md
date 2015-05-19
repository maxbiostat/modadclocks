This repository was made to accompany the article 'Evaluating the adequacy of molecular-clock models using posterior predictive simulations'
============================================================================================================================================

This repository was contributed by David Duchene and Sebastian Duchene

david.duchene[at]anu.edu.au

sebastian.ducnene[at]sydney.edu.au

19 May 2015

Summary
-------

This repository was designed to assess the adequacy of clock and substitution models used in phylogenetics. It requires the posterior of trees and parameter estimates, and provides the substitution model adequacy, the overall (A index) and branch-wise clock model adequacy, the effect size of the branch wise adequacy, and the uncertainty in posterior predictive simulations.

A flexible application for assessing clock model adequacy is being built. The present repository is specifically to accmpany the article; it is designed to test the clock model adequacy method on simulated data, so it is only suitable for the output of analyses from BEAST2 and a single gene partition. Clock models supported are the strict clock, the uncorrelated lognormal clock, and the random local clock. Substitution models supported inlcude the JC, HKY, and GTR models, including gamma-distributed rates.

The following are a set of examples of how to use the functions and how to present the results.


Example of usage
----------------
In the folder example_run_and_results you will find a simulated genetic alignment with 2000 base pairs in nexus format (al.nex) and chronogram in newick format (chrono.tre) with 50 taxa. The alignment was simulated along the chronogram under a Jukes-Cantor substitution model and with rate auto-correlation among lineages. You will also find an XML file to run BEAST 2 under a strict clock and a Jukes-Cantor model of substitution and a root calibration.

In this folder we also include the output log and tree files from BEAST 2, and the results from assessing clock and substitution model adquacy using the functions in the folder clock_modad.

The following is a simple example code to run and save the results for clock model adequacy after the BEAST 2 run has completed:








Graphical examples of results
-----------------------------



