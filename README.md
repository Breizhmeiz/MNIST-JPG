---
created: 2022-03-23T12:41:36 (UTC +01:00)
tags: []
source: https://simplonline.co/briefs/f5603589-2cdb-4227-94d3-12cc13b42f3d
author: 
---

# Classification des chiffres manuscrites

![](https://simplonline.co/_next/image?url=https%3A%2F%2Fsimplonline-v3-prod.s3.eu-west-3.amazonaws.com%2Fmedia%2Fimage%2Fpng%2Ff9abcac9-1e38-4c24-b681-7f46d393fe9c.png&w=1280&q=75)

Fabio
Morgan
Romain

## Partie 1 : Base de données, Analyse et Préparation

Pour aborder cette problématique de la reconnaissance des chiffres, il est primordial d’avoir une DataSet. Pour cela, vous devez télécharger la Dataset MNIST (https://github.com/teavanist/MNIST-JPG).

Par la suite, il faut développer une boucle for pour lire les images et les charger sous forme un tenseur.

Outils :
- Import os
- Import cv2
- from sklearn.model\_selection import train\_test\_split
- os.listdir(chemin)
- cv2.cvtColor(img, cv2.COLOR\_GRAY2BGR) si besoin
- cv2.resize(img,(width,height), interpolation = cv2.INTER\_AREA) si besoin
- Data.append(image) – Label.append(classe)

## Partie 2 : Architecture CNN sur Tensorflow

Cette deuxième partie est réservée pour développer une architecture CNN sur tensorflow, et lancée par la suite l’apprentissage de CNN. Calculer l’accuracy et la matrice de confusion sur les données de test, commenter les performances obtenues. Outil : https://www.tensorflow.org/tutorials/images/cnn

## Partie 3 : Tester l’efficacité du modèle

Nous cherchons à tester le modèle développer sur des nouvelles données. Pour un début, utiliser l’application Paint pour simuler des chiffres, et tester les performances de votre modèle sur les chiffres simulés.

Il sera intéressant de développer une application python pour reconnaitre automatiquement les chiffres en intégrant votre modèle CNN.

## Original repository

This repository contains the MNIST dataset in JPG format. 
The converted files in JPG format is attached in a zip file. There is one folder each for Testing and Training 

I made this when I was playing around with MNIST and trying to understand ML. There was I think a repo that converted files to PNG. I wanted to test and train on JPG files and hence this simple python script. Since I didnt think the code would need further development, I have included a zip file of all the MNIST images. You can download and start using it straigtaway instead of bothering with the python file. 

The original inspiration is this repo:
https://github.com/myleott/mnist_png
