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

- [**Machine Learning**](#Machine-Learning)
- [**Traitement du langage naturel**](#Traitement-du-langage-naturel)
- [**Time series**](#Time-Series)
- [**Big Data**](#Big-Data)
- [**Agriculture**](#Agriculture)
- [**Images**](#Images)
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

Aperçu du fichier "April 2021 (CSV – 216M)" :



<p align="left"><a href="https://fdc.nal.usda.gov/download-datasets.html"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>


<br/>

## 2. Données hyperspectrales d'un échantillon de sol en campagne

Aperçu :

<p align="center">
<img width="1210" alt="Capture d’écran 2021-05-21 à 16 54 37" src="https://user-images.githubusercontent.com/63207451/119157232-422a7f80-ba55-11eb-8c86-cc7fa64d920c.png">
<p/>
<p align="left"><a href="https://zenodo.org/record/2530634#.YKf_ZS8iuRs"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

	
<br/>

# Images


<br/>

# Climat et météo

<br/>
