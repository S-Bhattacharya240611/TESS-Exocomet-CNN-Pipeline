PROJECT TITLE: TESS-Exocomet-CNN-Pipeline
SUBTITLE: Independent Discovery and Characterization of Transient Exoplanetary Anomalies
RESEARCHER: Spandan Bhattacharya
ORCID ID: 0009-0006-4855-6296
AFFILIATION: Independent Researcher, India
PROJECT OVERVIEW
This repository hosts a professional-grade discovery pipeline designed to identify non-periodic exocometary transits in TESS (Transiting Exoplanet Survey Satellite) data. The system uses a hybrid approach: a 1D-Convolutional Neural Network (CNN) for anomaly detection and Markov Chain Monte Carlo (MCMC) parametric modeling for physical validation.
SCIENTIFIC VALIDATION: TIC 73149665
The pipeline was used to independently recover and characterize the exocomet candidate in TIC 73149665 (Anomaly at Day 2376.11 BTJD).
RESULTS SUMMARY:
Reduced Chi-Squared: 1.3026 (Statistically rejecting a symmetric planetary model).
Morphology: Clear asymmetric egress consistent with a trailing cometary dust tail.
Vetting: Centroid motion (sap_x/sap_y) confirmed as stable, ensuring astrophysical origin.
METHODOLOGY
The pipeline follows a two-stage scientific workflow:
STAGE 1 (Discovery):
A 1D-CNN trained on synthetic cometary injections scans binned TESS QLP lightcurves. This stage acts as a high-speed "scout" to flag potential candidates.
STAGE 2 (Validation):
High-precision modeling using the EXOTIC MCMC engine. By attempting to fit a symmetric planetary model to the data, we isolate the residuals. A high Chi-squared value and asymmetric residuals serve as proof of a cometary origin.
REPOSITORY CONTENTS
TESS_Exocomet_Discovery_Pipeline.ipynb: The primary Python research environment.
TIC73149665_Discovery_Report_Spandan.pdf: The formal technical research report.
figures/: Folder containing raw data, smoothed signals, and residual plots.
LICENSE AND CITATION
This project is licensed under the MIT License.
If you use this pipeline in your research, please cite as:
Bhattacharya, S. (2026). TESS-Exocomet-CNN-Pipeline: A hybrid deep learning and MCMC framework for exocomet detection. GitHub. https://github.com/S-Bhattacharya240611/TESS-Exocomet-CNN-Pipeline
ACKNOWLEDGMENTS
Special thanks to the NASA Exoplanet Watch community and the developers of the Lightkurve and EXOTIC packages. AI assistance was utilized for code optimization and technical drafting.
CONTACT:
Reach out via the ORCID profile linked at the top of this document.
