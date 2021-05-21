<p align="center">
	<img src="https://user-images.githubusercontent.com/63207451/119138957-c4f60f00-ba42-11eb-89fa-e999bb5d256a.png">
	<p/>


<br/>
<br/>

<p align="center">
	Vous trouverez ici plus de ?? <b>Datasets</b> dans diverses catégories. Toutes les catégories sont accessibles via le menu en dessous de cette introduction. Les Datasets sont tous open sources et gratuits, et ne nécessitent aucune autorisation. Pour l'ouverture des datasets avec python voici un petit <a href="#Ouvrir-un-dataset-avec-python">tuto</a> qui montre comment les ouvrir en fonction des types de fichiers.
		<p/>

<br/>

# Categories

1. [Agriculture](#Agriculture)
2. [test2](#test2)



# Ouvrir un Dataset avec python

## Fichier nc4

```py
import xarray as xr

ds = xr.open_dataset('your/path/dataset.nc4')
df = ds.to_dataframe()

```



# Agriculture

## 1. Food data - U.S. DEPARTMENT OF AGRICULTURE

[Télécharger le dataset](https://fdc.nal.usda.gov/fdc-datasets/FoodData_Central_csv_2021-04-28.zip)


## 2. Données hyperspectrales et d'humidité d'un échantillon de sol en campagne Allemande

[Télécharger le dataset](https://zenodo.org/record/2530634/files/felixriese/hyperspectral-soilmoisture-dataset-v1.0.3.zip?download=1)

