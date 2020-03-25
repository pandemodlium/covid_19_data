This repository will support actuaries' interest in exploring COVID-19 data. R scripts to harvest data will be stored in the `data` folder. 

If you have the `make` program, you can use it to automatically and sensibly execute the scripts in the `data` folder. If you use RStudio, you can press CTRL-SHIFT-B to run `make`. Using `make` will ensure that you do not gather data which you have already stored on your device. This will minimize processing time and server load to data providers.

We love pull requests! When making them, though, please observe the following:

1. Do not use this repository to host data. Rather, create a script which will harvest the data from a publicly available source.
2. Stick with the current `data` and `eda` folder split.
3. There should be a one-to-one relationship between the script and the source. That is, any necessary processing after the data has been gathered should be in the same script used to source the data.
4. Each data gathering script should save its output as an `.rda` file with the same name as the script. 
5. Try to keep the technology stack straightforward. Base R, `tidyverse` and `data.table` are fine. Please avoid obscure data wrangling and analysis packages.