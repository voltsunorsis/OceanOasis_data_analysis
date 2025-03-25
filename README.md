# Project Name: Data Conversion and Analysis Toolkit

## Overview
This project offers a comprehensive set of tools for converting `.prn` files to `.csv`, performing data analysis, and conducting various engineering conversions. It includes utilities for force and power conversion, data visualization, and statistical analysis.

## Features
- **PRN to CSV Conversion:** Convert `.prn` binary files to `.csv` using automatic structure detection.
- **Data Cleaning:** Separate junk data (first 16 rows) and store them in a separate CSV.
- **Metadata Extraction:** Extract and store file metadata from `.prn` files in a readable `.txt` file.
- **Data Merging:** Combine multiple `.csv` files into a single output CSV.
- **Power Conversion:** Convert power measurements between different units.
- **Force Conversion:** Convert forces across various measurement systems.
- **Visualization:** Generate line plots for data columns.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/username/project-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd project-name
    ```
3. Install dependencies using:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
### Convert PRN to CSV
```python
process_all_prn_files(input_folder, output_folder)
```
- Converts `.prn` files and removes junk data.

### Perform Power Conversion
```python
convert_power(value, input_unit, output_unit)
```
- Supports conversions between watts, kilowatts, horsepower, and other units.

### Perform Force Conversion
```python
convert_force(value, input_unit, output_unit)
```
- Supports conversions between newtons, dynes, pound-force, and kilograms-force.

### Generate Plots
```python
plot_and_save_data(input_file, column_name, output_folder)
```
- Plots specified data columns and saves visualizations.

## File Structure
```
.
├── data
│   ├── example.prn
├── notebooks
│   ├── data_analysis.ipynb
├── scripts
│   ├── converter.py
│   ├── visualizer.py
├── models
│   ├── trained_model.pkl
├── images
│   ├── output_plot.png
├── requirements.txt
└── README.md
```

## Conclusion
The project offers flexible and scalable data conversion, visualization, and analysis tools, suitable for both engineering and scientific applications.

## Acknowledgments
- Libraries used: `numpy`, `pandas`, `matplotlib`, and `scikit-learn`.

