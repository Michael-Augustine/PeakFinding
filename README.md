# PeakFinding
## Analysis of Gaussian Spectra

In this analysis, we work with a dataset containing Gaussian spectra, which provides information about wavelengths and corresponding power values. The main objectives are to find peaks in the spectra, calculate their Full Width at Half Maximum (FWHM), and visualize the results.

### Loading and Preprocessing the Data

We start by importing the necessary libraries, including Pandas for data manipulation, NumPy for numerical operations, Matplotlib for visualization, and SciPy's `find_peaks` function for peak detection. The data is loaded from a CSV file named `gaussian_spectra_1545.997.csv` and then renamed to have more meaningful column names. Next, the data is sorted based on the wavelength column.

### Normalizing the Power Data

To ensure consistent scaling, we normalize the power data to bring all values within the range [0, 1]. This step is essential for better analysis, as it allows us to compare power values effectively.

### Finding Peaks and Calculating FWHM

Using the `find_peaks` function from SciPy, we detect peaks in the normalized power data based on a specified prominence value. Peaks represent regions where the power values are significantly higher than their surroundings.

Next, we calculate the Full Width at Half Maximum (FWHM) for each peak. FWHM is the width of the peak at half of its maximum height and provides a measure of the peak's width or spread.

### Visualizing the Gaussian Spectra

We create a plot to visualize the normalized power values against the corresponding wavelengths. The Gaussian peaks are marked with red points, and vertical dashed lines are drawn at the positions of the peaks. Additionally, annotations are added to each peak, providing information about the peak number, its wavelength, peak power, and FWHM.

### Printing Peak Data

Finally, we print out the peak data for each identified peak. This includes the peak wavelength, normalized peak power value, and FWHM. These details provide essential insights into the characteristics of each peak.

Overall, this analysis gives a clear and comprehensive view of the Gaussian spectra, identifying peaks and their associated properties.

### Sample Dataset 
![image](https://github.com/Michael-Augustine/PeakFinding/assets/88915387/b852e513-e3bc-4470-8b10-41bd1e1da4f2)
