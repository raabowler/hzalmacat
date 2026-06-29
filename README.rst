**HZALMACAT: A catalog of FIR observations at z > 6.5, including code to read the data**
 
============

** To be updated in the next month **

Overview
-----------
The catalogue compiled and presented here contains the published ALMA and NOEMA observations of galaxies at z > 6.5 as presented in the review paper entitled "An ALMA view of high-redshift galaxy formation" by Renske Smit and Rebecca Bowler 2026 published in the Annual Review of Astronomy and Astrophysics.
We enteavor to keep this catalogue up to date in future.

Here we include:
- the original catalogue
- any updated catalogues
- a description of the columns
- basic codes for reading in and displaying the results


The catalogue
~~~~~~~~~~~
Listed in the catalogue directory.  The columns are as follows:

* Column (1): Flag indicating whether the observation is considered as valid for the catalog
* Column (2): Flag indicating whether the source is the main targeted galaxy (M) or a companion (C)
* Column (3): Source name
* Column (4): Right ascension
* Column (5): Declination
* Column (6): Redshift
* Column (7): Cosmology used to calculate the luminosity distance
* Column (8): Luminosity distance, in [Mpc]
* Column (9): Homogenized source type as extracted from the literature search

   - quasars and AGN from various classification techniques
   - sub-mm galaxies and starbursts, mostly selected via their luminous dust continuum emission in the infrared wavelengths
   - main sequence and more `typical' star-forming galaxies
   - optically--selected galaxies (primarily Lyman Break Galaxies and Ly$\alpha$ emitters)
   - line emitters identified with interferometric observations
   - cluster members of diverse type
* Column (10): Instrument that carried out the observation

The python notebooks
~~~~~~~~~~~


Referencing
-----------
If you use the catalogue or notebook in a publication or presentation, please 1) cite the original review artile and 2) add a link to the GitHub repository: https://github.com/raabowler/hzalmacat

Contributors
~~~~~~~~~~
* Rebecca Bowler & Renske Smit

Bibcode
~~~~~~~~~
TBD


.. _this Google spreadsheet: https://docs.google.com/spreadsheets/d/1GBEhRR3zSSVupEGh4PbrzMAKzs3w1x2MC6JLtsIIgbk/edit?usp=sharing
