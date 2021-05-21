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

- [**Agriculture**](#Agriculture)
- [**Biologie**](#Biologie)
- [**Climat et météo**](#Climat-et-météo)


<br/>
<br/>

# Ouvrir un Dataset avec python

## Fichier nc4

```py
import xarray as xr

ds = xr.open_dataset('your/path/dataset.nc4')
df = ds.to_dataframe()

```
<br/>

## Fichier csv

```py
import pandas as pd

df = pd.read_csv('your/path/dataset.csv')

```

<br/>

## Fichier excel

```py
import pandas as pd

df = pd.read_excel('your/path/dataset.xls(x)')

```

<br/>


# Agriculture

## 1. Food data - U.S. DEPARTMENT OF AGRICULTURE

<p align="left"><a href="https://fdc.nal.usda.gov/fdc-datasets/FoodData_Central_csv_2021-04-28.zip"><img src="https://user-images.githubusercontent.com/63207451/119182210-e969df80-ba72-11eb-81bc-1f10fe5a81da.png" alt="Download" height="80"/></a></p>


<br/>

## 2. Données hyperspectrales et d'humidité d'un échantillon de sol en campagne

Aperçu :

<p align="center">
<img width="1210" alt="Capture d’écran 2021-05-21 à 16 54 37" src="https://user-images.githubusercontent.com/63207451/119157232-422a7f80-ba55-11eb-8c86-cc7fa64d920c.png">
<p/>

Il est composé d'une colonne avec la date, l'humidité de la parcelle, la température de la parcelle et les colonnes nommées 454 à 950 sont les longueures d'ondes utilisées en nanomètres par l'instrument de mesure. (il y en a 125)
<br/>

<p align="left"><a href="https://zenodo.org/record/2530634/files/felixriese/hyperspectral-soilmoisture-dataset-v1.0.3.zip?download=1"><img src="https://user-images.githubusercontent.com/63207451/119155205-350c9100-ba53-11eb-9e4b-8198f9f6cca2.png" alt="Download" height="80"/></a></p>

	
<br/>

# Biologie


<br/>

# Climat et météo

<br/>
