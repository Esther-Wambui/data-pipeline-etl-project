

# ETL Extract Lab

**Name:** Esther Wambui


## Description

This project covers **Lab 3, Lab 4, and Lab 5** from the **DSA 2040A – Data Warehousing and Data Mining** course. 
It demonstrates the key stages of a real-world ETL (Extract, Transform, Load) pipeline using Python and Jupyter.

Covered ETL Stages::

- **Full Extraction** – loading the entire dataset and displaying key statistics.
- **Incremental Extraction** – extracting only new or updated rows since the last recorded extraction timestamp.
- **Data Transformation** – cleaning, enriching, and structuring the extracted data for analysis.
-**Data Loading** – Save transformed datasets into structured Parquet files.
The project also updated the timestamp after every incremental extraction.


---

## Tools Used

- Python 3.12  
- Jupyter Notebook  
- pandas  
- pyarrow (for Parquet support)  
- Pathlib (for cross-platform file handling)

---

## How to Reproduce

1. Clone this repository or download the ZIP.

```bash
git clone https://github.com/Esther-Wambui/ETL_Extract_EstherWambui_669399-.git
```

2. Open the project folder.

3. Run `etl_extract.ipynb` in **Jupyter Notebook**.

4. Files used:

   * sales_data_sample.csv → dataset used for the extraction.
   * last_extraction.txt → stores the timestamp of last extraction.

5. The notebook will:

   * Perform **Full Extraction** of the dataset.
   * Perform **Incremental Extraction** based on last_extraction.txt.
   * Save the new timestamp.

6. After running `etl_extract.ipynb`, two files will be created:

   * `transformed_full.csv` – the cleaned full dataset.
   * `transformed_incremental.csv` – the cleaned incremental dataset.

7. Then run `etl_load.ipynb` to load both transformed datasets into structured Parquet files.

8. This notebook will:

   * Load `transformed_full.csv` and `transformed_incremental.csv` using pandas.
   * Save each as a `.parquet` file using the `pyarrow` engine.
   * Create a `loaded_data/` folder (if not already existing).
   * Preview the first 5 rows from both Parquet files to confirm successful loading.

9. Output files from Lab 5:

   * `loaded_data/full_data.parquet`
   * `loaded_data/incremental_data.parquet`
  
10. Ensure you have `pyarrow` installed before running `etl_load.ipynb`:

```bash
pip install pyarrow 
```
---

## Dataset Source

Dataset used: **Sales Data Sample**
(Sourced from Kaggle )

---

## Screenshots 

* ![image](https://github.com/user-attachments/assets/3b37702b-c7f7-4960-ad2f-b52de4f7bb08)
* ![image](https://github.com/user-attachments/assets/cfcd18c5-59b0-4425-bfc3-ec5e3da25c74)
* ![image](https://github.com/user-attachments/assets/dd209b16-5a3f-4349-896a-f09389cf4839)
* ![image](https://github.com/user-attachments/assets/907e37b5-e6ed-4dc0-a601-8acd054643f1) 
* ![image](https://github.com/user-attachments/assets/4f8916ca-33fa-4a0a-b7c2-2afd57273bc7)
*  ![image](https://github.com/user-attachments/assets/0e8f199f-f8c0-4074-8c9b-95e510f2b9e8)
*  ![image](https://github.com/user-attachments/assets/460d3177-f4b0-4399-aacd-b2b9aa5462b2)

*  ![image](https://github.com/user-attachments/assets/049ba52f-d1c6-465a-a6af-a0186f02a5cf)
* ![image](https://github.com/user-attachments/assets/ac817931-582a-47f9-94c9-90e1b7092d14)
* ![image](https://github.com/user-attachments/assets/a85ce39b-3bf9-463e-8233-fcf7aa6c3ba2)
* ![image](https://github.com/user-attachments/assets/82a871e7-1262-4873-a212-f66f818d955c)
* ![image](https://github.com/user-attachments/assets/5086cd81-aece-439d-bb25-3d10fdfac57f)



 




 *

---


