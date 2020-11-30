# IdentifyBots Replication Package

This repository contains the replication package for our study about identifying bots in social coding platforms submitted to JSS journal (*"A ground-truth dataset and classification model for detecting bots in GitHub issue and PR comments"*). A link to the paper will be added to this README as soon as the paper is accepted for publication.

# Ground-truth dataset
The ground-truth dataset is available on Zenodo: http://doi.org/10.5281/zenodo.3626071

# The BoDeGHa Tool
The BoDeGHa tool is available on GitHub: https://github.com/mehdigolzadeh/BoDeGHa

# Replication package

We followed a Grid-search cross validation in "notebooks/Classification of accounts.ipynb" to find the best classifier and construct the final mode. The replication package was originally created on Python 3.8  and the dependencies required to run these notebooks are listed in requirements.txt and can be automatically installed using pip install -r requirements.txt.

The data used to construct and validate the model can be found in "data/accounts.csv.gz". They were produced in the "notebooks/Computing clusters.ipynb". To avoid any conflict with GDPR regulations we have removed the "ccount_comments.csv.gz" dataset. The "notebooks/Evaluation of the classifier.ipynb" contains scripts to evaluate the classifier and it will create the "prediction.csv.gz" file that contains the prediction of the model for the entire dataset.
