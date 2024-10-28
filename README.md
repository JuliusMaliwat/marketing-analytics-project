
# Operational Guide 

## Environment Setup

- **Python version**: 3.12.1
- Create a virtual environment:
  
    ```bash
    python -m venv .venv
    ```
    
- Activate the virtual environment:
  - On macOS/Linux:
    ```bash
    source .venv/bin/activate
    ```
  - On Windows:
    ```bash
    .venv\Scripts\activate
    ```
- Install dependencies:
    ```bash
  pip install -r DSLab_info.txt
    ```

## Repository Structure

- **data**:
  - **raw**: Contains the raw CSV files used for analysis. Place your raw data files here before running the notebooks.
  - **processed**: Contains pre-processed data before the sentiment analysis model.
  - **shapefile**: Contains shapefiles for visualizing the map of Italy.

- **models**: This directory stores the best-performing sentiment analysis model.

- **src**:
  - Contains all the Jupyter notebooks used for analysis.
  - **modules**: Includes utility modules such as `constants.py` and `product_utils.py`.

## Execution Sequence

- Ensure that the necessary CSV files are placed in `data/raw`.
- For reproducibility, execute the notebooks in the `src` folder in the following sequence:
  1. S01_Data_Understanding.ipynb
  2. S02_Customer_Focus.ipynb
  3. S03_Product_Focus.ipynb
  4. S04_Feedback_Focus.ipynb

