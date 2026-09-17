**HZALMACAT: A catalog of FIR observations at z > 6.5**
 
============

Overview
-----------
The catalogue compiled and presented here contains the published ALMA and NOEMA observations of galaxies at z > 6.5 as presented in the review article entitled "An ALMA view of high-redshift galaxy formation" by Renske Smit and Rebecca Bowler published in the Annual Review of Astronomy and Astrophysics in 2026.
We enteavor to keep this catalogue up to date in future.

Here we include

 - the original catalogue
 - any updated catalogues
 - a description of the columns
 - basic codes for reading in and displaying the results [to follow]


The catalogue
~~~~~~~~~~~
Note that a -99 in the _ue column signifies an upper limit.  In this case the value is given as the 3 sigma limit.  e.g. if fobs_ue = -99, then the value listed as fobs for that source is an upper limit of 3 sigma and should be plotted as a limit.

The columns are as follows:

* Column ID: Source name.
* Column altID: any alternative names in the literature separated by a comma.
* Column RA: Right ascension in degrees.
* Column DEC: Declination in degrees.
* Column mu: magnification factor, nan if not lensed.
* Column redshift: Spectroscopic redshift if available, if not the photometric redshift.
* Column z_spec: Spectroscopic redshift from FIR lines if available, nan if unavailable.
* Column z_specother: Spectroscopic redshift from Lya if available, nan if unavailable.
* Column z_phot, z_phot_ue,  z_phot_le: Photometry redshift, nan if unavailable.
* Column Muv, Muv_e: absolute UV magnitude from the literature. Typically at 1500 or 1600A rest-frame.
* Column lMstar, lMstar_ue, lMstar_le: log10 (stellar mass/solar mass) from the literature.
* Column beta, beta_le, beta_ue: the rest-frame UV slope from the literature.
* Column Category: The final category of the source, either
 * LBG
 * LAE, if the rest-EW of Lyman-alpha is > 25A
 * Quasar
 * ALMA, a FIR selected source (e.g. ALMA or SPT)
* Column Selection: as above, except LAEs are only sources that were originally selected with the narrowband technique (not LBGs that have strong line emission)
* Column EWLyman: the rest-frame equivalent width of Lyman-alpha in Angstrom, nan if unavailable. If there is an upper limit we quote the 1 sigma limit as a negative value.
* Column LCII/LCII_e: luminosity and error of the [CII]158 line, from the literature. For -99 in the error column, the LCII column gives 1 sigma upper limits. Nan if no data is available. * Column CII_FWHM, CII_FWHM_e: the full width at half maximum (and error) of the [CII]158 linein km/s, nan if not available  
* Column CII_FWHM/CII_FWHM_e: the full width at half maximum (and error) of the [CII]158 line in km/s, nan if not available
* Column LOIII/LOII_e: luminosity and error of the [OIII]88 line, from the literature. For -99 in the error column, the LOIII column gives 1 sigma upper limits. Nan if no data is available. 
* Column OIII_FWHM/OIII_FWHM_e: the full width at half maximum (and error) of the [OIII]88 line in km/s, nan if not available  
* Column EWOIIIHb/EWOIIIHb_e: the rest-frame equivalent width of the Hb Balmer line combined with the [OIII]4969,5007 doublet in Angstrom. Nan is no data is available.
* Column SFR_UV, SFR_UV_ue, SFR_UV_le: UV luminosity, uncorrected for dust, converted to a SFR using the Madau & Dickenson conversion corrected by a factor of 0.63 for a Chabrier IMF. 
* Column Luv, Luv_e: absolute UV luminosity from the literature. Typically at 1500 or 1600A rest-frame in solar luminosity.  Directly quoted from the literature where available or else converted from Muv.
* Column Lir, Lir_e: Luminosity from 8-1000 microns, from our modified Black Body with an evolving dust temperature that is 41K at z ~ 6 (see review), and beta_d = 1.8.
* Column IRX, IRX_le, IRX_ue: log10(infrared excess) derived from the Lir and Luv computed in the review.
* Column SFR_IR, SFR_IR_e: SFR derived from the IR luminosity abvoe, converted to a SFR using the Kennicutt & Evans calibration 2012, corrected by a factor of 0.63 for a Chabrier IMF.
* Column fobs, fobs_le, fobs_ue: obscured fraction computed from the SFR_UV and SFR_IR.  
* Column Td, Td_le, Td_ue: dust temperature from the literature, when quoted as the Black Body temperature (not peak).
* Column Tpeak, Tpeak_le, Tpeak_ue: peak dust temperature from the literature.
* Column dustmass, dustmass_le, dustmass_ue: estimated as in the review from the best-fitting modified Black body.
* Column flux90, error90, freq90: from the literature in the band closest to rest-frame 90 microns (e.g. around OIII in Band 7 at z ~ 7)
* Column flux160, error160: flux and error from the literature in the band closest to rest-frame 160 microns (e.g. around CII in Band 6 at z ~ 7). For -99 in the error column, the flux160 column gives 1 sigma upper limits. Nan if unavailable. 
* Column freq160: observed frequency in GHz from the literature if reported, else using 1898.734/(1+redshift).
* Column flux90, error90: flux and error from the literature in the band closest to rest-frame 90 microns (e.g. around OIII in Band 8 at z ~ 7). For -99 in the error column, the flux90 column gives 1 sigma upper limits. Nan if unavailable. 
* Column freq90: observed frequency in GHz from the literature if reported, else using xxxx/(1+redshift).

Redshifts from REBELS
~~~~~~~~~~~
The redshifts used for the REBELS sample were obtained from the upcoming publication Schouws, Bouwens et al. in prep.

Errors or updates
~~~~~~~~~~~
If you find any errors in the catalogue or would like to supply updated values please contact rebecca.bowler manchester.ac.uk.


The python notebooks
~~~~~~~~~~~
To be updated 

Referencing
-----------
If you use the catalogue or notebook in a publication or presentation, please 1) cite the original review artile (https://www.annualreviews.org/content/journals/10.1146/annurev-astro-052722-104242) and 2) add a link to the GitHub repository: https://github.com/raabowler/hzalmacat

Contributors
~~~~~~~~~~
* Rebecca Bowler & Renske Smit

