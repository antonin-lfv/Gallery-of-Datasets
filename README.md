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

<a class="github-button" href="google.com" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-download" aria-label="Download antonin-lfv/Gallery-of-Datasets on GitHub">Télécharger</a>
[Télécharger le dataset](https://fdc.nal.usda.gov/fdc-datasets/FoodData_Central_csv_2021-04-28.zip)

<br/>

## 2. Données hyperspectrales et d'humidité d'un échantillon de sol en campagne

Aperçu :

<p align="center">
<img width="405" alt="Capture d’écran 2021-05-21 à 16 09 09" src="https://user-images.githubusercontent.com/63207451/119151112-5b303200-ba4f-11eb-905d-c24dad3fa739.png">
<p/>

Le dataset est indexé sur la position géographique en lat-long, il contient beaucoup de valeurs NaN comme mentionné dans le ReadMe de ce dernier.

[Télécharger le dataset ici](https://zenodo.org/record/2530634/files/felixriese/hyperspectral-soilmoisture-dataset-v1.0.3.zip?download=1)

	
<br/>

# Biologie


<br/>

# Climat et météo

<br/>
