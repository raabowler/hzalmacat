**HZALMACAT: A catalog of FIR observations at z > 6.5, including code to read the data**
 
============

** To be updated in the next month **

Overview
-----------
The catalogue compiled and presented here contains the published ALMA and NOEMA observations of galaxies at z > 6.5 as presented in the review paper entitled "An ALMA view of high-redshift galaxy formation" by Renske Smit and Rebecca Bowler 2026 published in the Annual Review of Astronomy and Astrophysics.
We enteavor to keep this catalogue up to date in future.

Here we include
 - the original catalogue
 - any updated catalogues
 - a description of the columns
 - basic codes for reading in and displaying the results


The catalogue
~~~~~~~~~~~
Listed in the catalogue directory.  The columns are as follows:

* Column ID: Source name
* Column altID: any alternative names in the literature
* Column RA: Right ascension
* Column DEC: Declination
* Column redshift: Spectroscopic redshift if available, if not the photometric redshift
* Column z_spec: Spectroscopic redshift from FIR lines if available
* Column z_phot: Photometry redshift (errors available)
* Column Category: The final category of the source, either
    * LBG
    * LAE,  if the rest-EW of Lyman-alpha is > 25A
    * Quasar
    * ALMA, a FIR selected source
* Column Selection: as above, except in the case of a narrow band LAE source, that has too low an EW of Lyman-alpha
* Column LCII/LCII_e: luminosity and error of CII, from the literature
* Column flux160, error160, freq160: from the literature in the band closest to rest-frame 160 microns (e.g. around CII in Band 6 at z ~ 7)
* Column LIR, LIR_lerr, LIR_uerr: Luminosity from 8-1000 microns, from our modified Black Body with an evolving dust temperature that is 41K at z ~ 6 (see review), and beta_d = 1.8.
* Column Muv, Muv_e: absolute UV magnitude from the literature.  Typically at 1500 or 1600A rest-frame.
* Column lMstar, lMstar_ue, lMstar_le: log10 (stellar mass/solar mass) from the literature.
* Column beta, beta_le, beta_ue: the rest-frame UV slope from the literature
* Column flux90, error90, freq90: from the literature in the band closest to rest-frame 90 microns (e.g. around OIII in Band 7 at z ~ 7)
* Column Luv, LuvErr: absolute UV luminosity from the literature (matches Muv).  Typically at 1500 or 1600A rest-frame.

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
