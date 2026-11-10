# Publishing this repository

The repository is committed locally on branch main. Two ways to publish it.

## Using the GitHub CLI

    gh auth login
    cd collections-conduct-eval
    gh repo create collections-conduct-eval --public --source=. --push

## Using git directly

Create an empty repository on github.com first, without a README or licence,
then:

    cd collections-conduct-eval
    git remote add origin https://github.com/Myoroject/collections-conduct-eval.git
    git push -u origin main

## Before publishing

Two things are worth doing first.

Check the final page of the Word document. It gives the repository address as
github.com/Myoroject/collections-conduct-eval. If you publish under a different
name, change it in docs/combined source and rebuild, or edit the document.

Decide whether the Word and PDF files belong in the repository. They are
committed now because they are the readable form of the two papers, and anyone
arriving at the repository will want them. If the repository later carries code
and test runs, move them to a release instead, so the history stays light.
