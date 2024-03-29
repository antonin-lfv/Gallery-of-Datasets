<p align="center">
	<img src="https://user-images.githubusercontent.com/63207451/119138957-c4f60f00-ba42-11eb-89fa-e999bb5d256a.png" alt="Haut de la page">
	<p/>


<br/>
<br/>

<p align="center">
	Vous trouverez des <b>Datasets</b> dans diverses catégories. Toutes les catégories sont accessibles via le menu en dessous de cette introduction. Les Datasets sont tous open sources et gratuits, et ne nécessitent aucune autorisation. Pour l'ouverture des datasets avec python voici un petit <a href="#Ouvrir-un-dataset-avec-python">tuto</a> qui montre comment les ouvrir en fonction des types de fichiers.
		<p/>

<br/>

# Moteurs de recherches de Datasets

- [**Classification**](https://sci2s.ugr.es/keel/category.php?cat=clas)
- [**Regression**](https://sci2s.ugr.es/keel/category.php?cat=reg)
- [**Physique**](http://opendata.cern.ch)
- [**Climat**](https://www.ncdc.noaa.gov/data-access/quick-links)
- [**Human Progress**](https://www.humanprogress.org/datasets/)
- [**USA government datasets**](https://data.census.gov/table)
- [**Grosse base de datasets**](https://github.com/awesomedata/awesome-public-datasets)
- [**Kaggle**](https://www.kaggle.com/datasets)
- [**Hugging Face**](https://huggingface.co/datasets)
- [**Google Dataset search**](https://datasetsearch.research.google.com)

<br/>

# Categories

- [**Machine Learning**](#Machine-Learning)
- [**Traitement du langage naturel**](#Traitement-du-langage-naturel)
- [**Time series**](#Time-Series)
- [**Big Data**](#Big-Data)
- [**Agriculture**](#Agriculture)


<br/>
<br/>

# Ouvrir un Dataset avec python

## Fichier nc/nc4

```py
import xarray as xr

ds = xr.open_dataset('your/path/dataset.nc4')
df = ds.to_dataframe()

```
<br/>

## Fichier csv

```py
import pandas as pd

df = pd.read_csv('your/path/dataset.csv') # delim_whitespace=True si colonnes séparés par des espaces

```

<br/>

## Fichier excel

```py
import pandas as pd

df = pd.read_excel('your/path/dataset.xls(x)') # delim_whitespace=True si colonnes séparés par des espaces

```

<br/>

## Fichier tsv
```py
import pandas as pd

df = pd.read_csv('your/path/dataset.tsv', delimiter="\t")

```

<br/>

## Fichier txt
```py
import pandas as pd

df = pd.read_csv('your/path/dataset.txt', delimiter="\t", header = None)

```

<br/>

## Fichier dat
```py
import numpy as np
# Il faut spécifier le nom des colonnes et choisir le bon séparateur
df = pd.read_table('your/path/dataset.dat', names=['x1','x2','x3'], sep=',' ,encoding='utf-8')
```


<br/>

# Machine Learning

## 1. Visages labelisés

Aperçu du dataset (173 Mb) :

<img width="499" alt="Capture d’écran 2021-05-24 à 10 09 41" src="https://user-images.githubusercontent.com/63207451/119317297-39fe5a00-bc78-11eb-9df7-9810359b4fd2.png">

Il est composée de 5749 dossiers, qui contiennent chacun une ou plusieurs images d'une même personne. Par exemple ci-dessus le dossier Matt_Damon.

<p align="left"><a href="http://vis-www.cs.umass.edu/lfw/"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

## 2. IMDb Datasets

Aperçu du dataset __title.ratings.tsv__ :

<img width="1431" alt="Capture d’écran 2021-05-22 à 12 36 37" src="https://user-images.githubusercontent.com/63207451/119223539-5bd1d280-bafa-11eb-98df-069c1259bcf7.png">

Il y a 7 datasets tsv disponibles, les données sont mises à jour tous les jours.

<p align="left"><a href="https://www.imdb.com/interfaces/"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

## 3. Classification de bananes

Aperçu du dataset complet : 

<img width="408" alt="Capture d’écran 2021-05-22 à 18 24 12" src="https://user-images.githubusercontent.com/63207451/119233808-e9c5b180-bb2a-11eb-99bb-915d376301d8.png">

Le dataset est détaillé dans le fichier __header__, dat1 et dat2 correspondent aux coordonnées des points x, y et class à la classe.
Exemple de plot des bananes par classe :

![Capture d’écran 2021-05-24 à 17 41 24](https://user-images.githubusercontent.com/63207451/119372157-4bb32200-bcb7-11eb-98b7-65de85c9c397.png)


<p align="left"><a href="https://sci2s.ugr.es/keel/dataset.php?cod=182"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

## 4. Classification de voitures

Aperçu :

<img width="1432" alt="Capture d’écran 2021-05-22 à 18 08 23" src="https://user-images.githubusercontent.com/63207451/119233316-b84be680-bb28-11eb-82b0-5bdd014cdc39.png">

<p align="left"><a href="https://sci2s.ugr.es/keel/dataset.php?cod=56"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

## 5. Regression - tremblements de terre

Aperçu :

<img width="408" alt="Capture d’écran 2021-05-22 à 18 30 15" src="https://user-images.githubusercontent.com/63207451/119233994-ccddae00-bb2b-11eb-8526-f89dbcd26968.png">

Le dataset renseigne sur la profondeur, les coordonnées géographiques et l'intensité sur l'échelle de Richter. <br>
Exemple de plot en coloriant suivant l'intensité:

<img width="1426" alt="Capture d’écran 2021-05-22 à 23 16 19" src="https://user-images.githubusercontent.com/63207451/119240977-c105e200-bb53-11eb-885f-7aaf7dc59c4e.png">

<p align="left"><a href="https://sci2s.ugr.es/keel/dataset.php?cod=75"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

<br/>
<br/>

# Traitement du langage naturel

## 1. Messages SMS spam

Aperçu du dataset depuis le __"Link1"__ du tableau :

<p align="center">
<img width="1431" alt="Capture d’écran 2021-05-22 à 12 20 54" src="https://user-images.githubusercontent.com/63207451/119322545-01fa1580-bc7e-11eb-8b52-a3829a53802b.png">
	<p/>

C'est un fichier texte qu'on manipule avec pandas comme ceci :

```py
df = pd.read_csv('your/path/SMSSpamCollection.txt', header = None, delimiter='\t')

df.columns =['type', 'sms']
df['type']=df['type'].astype(str)
df['sms']=df['sms'].astype(str)
```

<p align="left"><a href="https://www.dt.fee.unicamp.br/~tiago/smsspamcollection/"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

# Time series

## 1. Disques durs anomalies

Aperçu des 5 premières colonnes sur 85 :

![Capture d’écran 2021-05-24 à 14 11 43](https://user-images.githubusercontent.com/63207451/119346240-41cef600-bc9a-11eb-8c01-4f003b108725.png)

Il a un dataset par année, pour accéder aux datasets il faut aller tout en bas de la page. Puis dans chaque dossier de chaque année il y a un fichier csv par jour.

<p align="left"><a href="https://www.backblaze.com/b2/hard-drive-test-data.html"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>

# Big data

# Agriculture

## 1. Food data - U.S. DEPARTMENT OF AGRICULTURE

Aperçu du dataset __food_calorie_conversion_factor.csv__ du fichier "April 2021 (CSV – 216M)" :

<p align="center">
<img width="1431" alt="Capture d’écran 2021-05-22 à 12 20 54" src="https://user-images.githubusercontent.com/63207451/119223165-35129c80-baf8-11eb-8a1e-07e8d03fc15c.png">
	<p/>

Le fichier contient 35 Datasets csv qui sont tous détaillés dans le pdf joint avec.

<p align="left"><a href="https://fdc.nal.usda.gov/download-datasets.html"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>


<br/>

## 2. Données hyperspectrales d'un échantillon de sol en campagne

Aperçu :

<p align="center">
<img width="1210" alt="Capture d’écran 2021-05-21 à 16 54 37" src="https://user-images.githubusercontent.com/63207451/119157232-422a7f80-ba55-11eb-8c86-cc7fa64d920c.png">
<p/>
<p align="left"><a href="https://zenodo.org/record/2530634#.YKf_ZS8iuRs"><img src="https://user-images.githubusercontent.com/63207451/119182524-4d8ca380-ba73-11eb-8fb0-6e4a4c86d9c4.png" alt="Download" height="180"/></a></p>


<br/>

<br/>

<p align="center"><a href="#categories"><img src="http://randojs.com/images/backToTopButton.png" alt="Haut de la page" height="29"/></a></p>
