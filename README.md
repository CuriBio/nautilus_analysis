# Nautilus Analysis #
## Tools to extract data produced by multi-well microscope experiments i.e. Nautilus ##

### Run the script from the command line ###
` > python /path/to/well_data.py /path/to/toml_config --input_video_path /path/to/input/video --output_dir_path /path/to/output/dir`</br></br>
args with a leading -- are optional and if supplied will override keys with the same name in the json config.

### Basic System Test ###
To run a basic system test, if you are in the main directory (nautilus_analysis) :</br></br>

python src\well_data.py test_data\settings.toml

This will run the well data extraction function which will produce:
* xlsx files with the time series data from each well,
* a zip archive of all the xlsx files,
* an image with the roi's drawn on one frame of the input video,
* a plot of every wells time series data.
* a csv file with the time series data from all wells

