#addy-latlng
Simple script to read in a CSV with the column "full_address" and append latitudes, longitudes and confidence scores to a new CSV.

##Requirements
To run addy-latlng, you'll need to import the [Data Science Toolkit](http://www.datasciencetoolkit.org/developerdocs#street2coordinates).

```
pip install dstk
```

You'll also need an existing CSV with addresses in a column marked "full_address." The script will search for this column before running geolocation.

##Running it
Run addy-latlng by passing in the path to your CSV as an argument.

```
python addy-latlng.py SOURCE_DATA.csv
```

The file (e.g. SOURCE_DATA_latlng.csv) will be stored in the directory in which you run the script.

##Like it?
Check out a related script, [zips2fips](https://github.com/mtdukes/zips2fips), which helps convert zip codes to FIP codes for mapping purposes.
