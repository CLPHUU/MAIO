# Making, Analysing and Interpreting Observation Poster Presentation
This is the github page for the plots and data for the poster 'Random Forests vs. Neural Networks, a Comparison in NO2 Concentration Prediction'. All the code for the plots on the poster as well as Random Forest layout and Neural Network layout is present here. The code for the Random Forest can be found in Code/Random_Forest.ipynn and the NN code is avaiblable in Code/Neural_Network.ipynb.

## Data
The dataset used is courtesy of the RIVM. The data that was used can be found [here](https://statline.rivm.nl/portal.html?_catalog=RIVM&_la=nl&tableId=50084NED&_theme=96) with the license for the data [here](https://creativecommons.org/licenses/by/4.0/deed.nl). Like stated on the poster, all timestamps with unphysical data (negative values) were corrected to 0, while timestamps with missing data (< 3% of dataset) were cleaned from the dataset.
 
## Images
All the images that are deplicted on the screen are plotted in Code/Plotting.ipynb. The output from both the Random Forest as well as the Neural Network are saved in the Model_results/ folder, thus it is not needed to run the models yourself to see the data. For questions, contact the authors. 


## Dependencies
It is adviced to create a new envirmonent if working with conda. 

```bash
conda create -n MAIO_g14 python=3.9.2
conda activate MAIO_g14
```

Install the required Python packages:

```bash
pip install numpy pandas xarray scipy matplotlib datetime statsmodels scikit-learn ipykernel torch torchvision torchaudio ray ray[tune]
```
