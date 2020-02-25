# parquet_files-to-csv

Here in this notebook I have used a python function "glob()" to convert the parquet files to csv. 

## The function is:
data_dir = Path('the path to your parquet files')\
full_df = pd.concat(\
    pd.read_parquet(parquet_file)\
    for parquet_file in data_dir.glob('*.parquet')\
)\
full_df.to_csv('df_name.csv')

## In order to save the parquet files you need to run this:

!cp df_name.csv 'path where you want to save your csv'

I had uploaded my data and saved the csv files to google drive 
