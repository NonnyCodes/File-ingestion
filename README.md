## Large Dataset Files

Due to GitHub's file size limitations, the following files are hosted on Google Drive:

- [employee_churn_large_2gb.csv.gz](https://drive.google.com/file/d/1d6JXqrx1nZZI6Pv1w2CgEwV431tY7IJ-/view?usp=sharing)
- [employee_churn_large_pipe.csv](https://drive.google.com/file/d/1-CehfAGFCWK6sv3c31JpZaizo_PcFLAg/view?usp=sharing)
- [employee_churn_large_2gb.csv](https://drive.google.com/file/d/1-AQH2oJMG0A4YWu2nAr1DSV155ljlAYQ/view?usp=sharing)


STEPS
2+ GB employee churn dataset was created on Google colab)


different methods of file reading was done
Dask read time: 0.06 seconds. it was fast because it dosent load everything into memory immediately
Modin read time: 208.17 seconds
pandas kept crashing due to the large file size and thats because it loads the entire dataset into memory
Pandas (with chunking) read time: 72.63 seconds


basic validation on data columns 
column names were cleaned removing whitespaces and special characters


YAML schema file created as 'schema.yml'
Column validation passed


File written in pipe-separated format and compressed as 'employee_churn_large_pipe.gz'


FILE SUMMARY
Total number of rows :45,000,000
total number of columns: 12
file size: 2.12GB
