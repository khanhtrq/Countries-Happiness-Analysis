How to use the programs:
----------------
- First, download and merge the data using `download_data.inbpy`.
When the program is running, it'll ask you to modify some files, those files can be found inside the `code` folder.
How to modify those files is mentioned in the notebook file.
Their already-modified versions are also already there.
You may copy their content somewhere else to use later when asked.

    This step may be skipped.
    The downloaded and merged data can be found in `data/data_processed.csv`

- Then, remove countries with too many missing indicators and fill in the missing data by running `Handle missing value.inbpy`.
This step doesn't require manual interaction and can also be skipped.
The filled data can be found in `data/data_completed.csv`

- Finally, for EDA and visualization, run the file `EDA and Visualization.inbpy`.

- It is recommended to run the files in Google Colab because we wrote the code specially to run there.
If you run it in your local machine, some modifications and preparations must be made:
    - Install `pandas`, `numpy`, `matplotlib`, `plotly`, `seaborn`, `scipy` and `sklearn`
    - Remove the second code cell of all notebooks
    - Change the root in the third code cell of all notebooks to your project directory
    or to `os.path.dirname(os.path.dirname(__file__))`