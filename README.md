# S3Model

[![Build Status](https://travis-ci.com/twcook/S3Model.svg?branch=master)](https://travis-ci.com/twcook/S3Model)

Shareable-Structured-Semantic Model (S3Model)

See the [Documentation]('https://s3model.com')


A S3Model Data Model (DM) RDF file is named using the CUID of the complexType restriction of ConceptType from the RM. The CUID is prepended with 'dm-' and has the file extension '.ttl'.


The rdf:about attribute of the rdf:Description defining the RDF Subject prepends the file name with 'http://www.s3model.com/ns/s3m/'.  This rdf:Description then contains each Predicate/Object pair.


All Reference Models are named with their version number and are dereferenceable in the '/ns/s3m/' folder on the site. I.e. http://www.s3model.com/ns/s3m/s3model_4_0_0.ttl

The complexTypes in the RM named Xd* all descend from XdAnyType where Xd denotes e**X**tended **d**atatype.

Python Implementation
=====================
The Python implementation is located in the project https://github.com/twcook/S3MPython
There are tutorials included in the examples folder as Jupyter notebooks.


See the *Getting Started* notebook.

You will need to install Anaconda for your platform.
https://www.anaconda.com/download/


Then create the S3Model environment with:
::code bash
    $conda env create -f S3Model.yml

The resulting Python environment name will be *S3Model*.
