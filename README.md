📘 README.md
📌 Project Title: Circular Fourier Harmonic Analysis of Imaging Data
📖 Description
This Python script performs advanced signal processing and visualization on circular imaging data collected from mechanical stimulation experiments. The script reads .csv files containing orientation and intensity data, normalizes and smooths the signal, applies a circular shift-based peak detection method, performs Fourier analysis to extract harmonic information, and visualizes results using polar (rose) plots. It outputs both annotated visualizations and a summary .csv with key metrics per sample.

🧠 Why is this Important?
Understanding how signals behave over a 360° circular space—especially in biomechanics or neuroscience—is essential. Harmonic analysis gives insight into periodic patterns, such as whether the signal is dominated by twofold or fourfold symmetry. This analysis can be crucial for interpreting directional sensitivity or anisotropy in biological tissues.

🛠️ Features
Peak detection using circular shifts to avoid bias.

Fourier harmonic extraction (2nd and 4th harmonics).

Ratio and dominance calculation between harmonics.

Beautiful polar rose plots with visualized peaks and angular distances.

Summary CSV output with quantitative metrics.

📂 Folder Structure
bash
Copy
Edit
project-root/
│
├── analysed/                 # Folder containing input CSV data
├── script.py                 # Main Python script
├── harmonic_analysis_results.csv  # Output metrics
└── *.svg                     # Rose plots for each sample
🧪 Dependencies
Make sure you have the following Python libraries installed:

bash
Copy
Edit
pip install numpy pandas scipy matplotlib
🚀 How to Run
Place your .csv files in the specified folder (analysed).

Modify the folder_path variable if needed to reflect your file path.

Run the script:

bash
Copy
Edit
python script.py
Results will be saved as .svg plots and a harmonic_analysis_results.csv file.

📊 Output Summary
For each input file, the script calculates:

Number of detected peaks.

2nd and 4th harmonic amplitudes.

Ratio between H4 and H2.

Dominant harmonic.

Mean angular difference between peaks (0–180°).

Number of peaks in the first half-circle.

📝 Notes
Circular interpolation and data extension helps minimize edge artifacts.

Uses Savitzky-Golay filtering for signal smoothing.

Visual outputs are suitable for presentations and publications.

👨‍🔬 Author
This script was developed by a PhD researcher at The University of Manchester for processing experimental imaging data in a biomechanical context.

