# DAS Visualization Tool for AWS Repository

This repository provides a Jupyter notebook and necessary configuration files to assist users in visualizing Distributed Acoustic Sensing (DAS) data intended for public distribution through an AWS data repository. The notebook is designed for ease of use with minimal preprocessing and customizable channel selection.

## Contents

- `DAS_Visualization_AWS.ipynb`: Main Jupyter notebook for loading, visualizing, and interacting with DAS data.
- `channels_to_read_new.json`: A JSON file specifying a list of useful channels to plot from the DAS array.
- `DAS_Data/`: A folder where users should place their DAS `.hdf5` or similar formatted files for use with the notebook.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.9
- Jupyter Notebook
- Required packages:
  ```bash
  conda install numpy==1.26.4
  conda install matplotlib==3.9.2
  conda install pandas==2.2.3
  conda install h5py==3.12.1
  pip install obspy==1.4.1
  pip install joblib==1.2.0
  ```

### Instructions

1. **Place DAS Data**: Add your DAS data files into the `DAS_Data/` folder.
2. **Channel Configuration**: Review `channels_to_read_new.json` to understand or modify which channels will be loaded for visualization.
3. **Run the Notebook**: Launch `DAS_Visualization_AWS.ipynb` using Jupyter and follow the cells in order. The notebook includes plots and comments to guide usage.

## Notes on Preprocessing

This notebook uses raw or minimally preprocessed DAS data. For more advanced preprocessing steps (e.g., filtering, noise reduction), we recommend reviewing the following references:

- *Willis, R. M. (2025). From Injection to Ice: Advancing Climate Solutions Through Seismology, Machine Learning, and Open Science (Doctoral dissertation). Colorado School of Mines.*
- *Grimm, J. (2021). Cryoseismic Event Analysis on Distributed Strain Recordings Leveraging Statistical Learning Methods (Master’s thesis). Delft University of Technology. https://repository.tudelft.nl/record/uuid:b98362cd-ab70-4158-9055-733e86d29b13*
- *Manos, J.-M., Graff, D., Martin, E. R., Paitz, P., Walter, F., Fichtner, A., Lipovsky, B. P. (2024). DAS to discharge: using distributed acoustic sensing (DAS) to infer glacier runoff. Journal of Glaciology, 70 , e67.*

These works detail recommended methods for enhancing DAS signals for various environmental sensing applications.

## Citation

If you use this notebook or the associated methodology in your work, please cite any of our related publication:  

- *Willis, R. M., et al. (in preparation). Creating a Comprehensive Cryoseismic Catalog at Rhonegletscher: A Scalable Approach Using Distributed Acoustic Sensing and Machine Learning*
- *Willis, R. M. (2025). From Injection to Ice: Advancing Climate Solutions Through Seismology, Machine Learning, and Open Science (Doctoral dissertation). Colorado School of Mines.*
- *Grimm, J. (2021). Cryoseismic Event Analysis on Distributed Strain Recordings Leveraging Statistical Learning Methods (Master’s thesis). Delft University of Technology. https://repository.tudelft.nl/record/uuid:b98362cd-ab70-4158-9055-733e86d29b13*
