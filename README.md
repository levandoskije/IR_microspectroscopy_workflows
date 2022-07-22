# Orange workflows for Agilent µ-FTIR spectroscopy data processing

In this repository you find [Orange](https://orangedatamining.com) workflows for processing Agilent µ-FTIR data. An example dataset including hyperspectral example data.

## Guidelines for downloading and oppening workflows:

1. Go to [AINDA PRECISA DE UM LINK](COLOCAR_O_LINK_AQUI)
2. Click on **Code** and then **Download ZIP**. This can take some time...
3. You should get the following files structure:

```diff
├───README.md
│
├───dataset
│   ├── hyper_sample_data.bsp
│   └── hyper_sample_data.dat
│
├───img
├───workflows
│   └── agilent_hyperspectral_workflow.ows
```
5. Open the Orange app (for Orange installation, access the links [Quasar](https://quasar.codes) or [Orange](https://orangedatamining.com). It is mandatory to have the **Spectroscopy** Add-On installed for this kind of data processing.);
6. Load the workflow](workflows/).

------------
## Workflows for processing FPA Agilent data

### 1. Processing data (\*.dat)
To process Agilent image spectrum, it is **mandatory** that the following files should be in the same folder:

```diff
└── data_folder
│   ├── hyper_sample_data.bsp
│   └── hyper_sample_data.dat
```
>*Files content and designation:*
>- **.dat** contains the experimental data of the measurement;
>- **.bsp** file contains the experimental parameters of the measurement (metadata).

A typical workflow for processing *.dat files is presented:

<p align="center">
<img width="1200" src="/img/agilent_workflow.svg"/>
<p/>


**Loading procedure:**
1. Double click on the *Multifile widget*, click on *Clear* and then on the folder to select the data from the [dataset](/dataset/);
2. Define the specific reader *Spectra ASCII or Agilent Single Tile Image (\*.dat)* and then select the \*.dat file in the folder;
3. Files are loaded and the workflow is ready. To double check the loading procedure, click on the visualization widgets (*Hyperspectra*). The spectral data should be displayed.