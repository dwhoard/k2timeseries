# Sample Output Data Visualization Files for k2timeseries
		
### 212218649_sap_01_input_data.png
Visualization of the raw and pre-processed input data, showing the full light curve.

### 212218649_sap_02_LSperiodogram.png
Lomb-Scargle periodogram of the sample input data provided in the k2timeseries repository.

### 212218649_sap_03_bootstrap_max_npgram_trials_100000.txt
Results of a Monte Carlo simulation with N=100,000 trials. In each trial, the amplitude data were randomly scrambled relative to the input time data and a periodogram was recalculated. This output file lists the height of the tallest peak in the periodogram from each trial. The distribution of peak heights can be used to estimate the false alarm probability confidence levels for the original periodogram.

### 212218649_sap_04_fap_cumulative_trials_100000.png
Cumulative distribution curve to assess the false alarm probability (FAP) of signal peaks in the periodogram. The fiducial lines show the minimum peak heights corresponding to confidence levels of (left to right) 50%, 68.27% (1-sigma), 90%, 95.45% (2-sigma), and 99.73% (3-sigma). The FAP distribution was constructed by performing a Monte Carlo simulation with 100,000 trials; in each trial, the input data amplitudes (Y) were randomly redistributed onto the time (X) values before recalculating the periodogram.

### 212218649_sap_05_LSperiodogram_panels.png
Zoomed views of several regions of the periodogram, showing peaks that were automatically identified and their frequency centers as found from Gaussian model fitting.

### 212218649_sap_06_lc_folded_3.png
Multipanel plot showing the light curve folded on the orbit, spin, and beat periods found from the periodogram analysis.

### 212218649_sap_07_lc_trailed_0.18789412.png
Two-dimensional trailed light curve of the input data. The horizontal axis shows the cycle phase folded on one of the periods found from the time series periodogram analysis, and binned into 10 phases bins. The data are repeated over two cycles. Th vertical axis shows the cycle count over the full 79.5-day span of the data. The panel on the left shows the raw data; empty phase bins are depicted in white (NaNs in the DataFrame structure). The middle panel shows the data in each phase bin smoothed upward in the cycles direction by a moving window with the smallest size that eliminates all empty phase bins. The right panel uses a larger moving window size to present a more smoothed version of the data.

### 212218649_sap_08_lc_trailed_folded_0.18789412.png
Two-dimensional trailed light curve of the input data, with the vertical axis (cycle count) folded over a specified number of cycles. The data are repested over two cycles in both the horizontal (cycle phase) and vertical directions.
