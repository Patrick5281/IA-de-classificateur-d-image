# Classificateur d'Images avec TensorFlow

Ce projet a été réalisé par **Patrick HOUNTON** et utilise **TensorFlow** pour entraîner un modèle de classification d'images. Ce modèle est capable de classer des images dans différentes catégories à l'aide d'un réseau de neurones convolutifs (CNN). Le projet est conçu pour fonctionner dans un environnement Python avec Anaconda.

## Prérequis

- Python 3.10 ou version supérieure
- Anaconda
- TensorFlow
- OpenCV (pour le prétraitement des images)

## Installation d'Anaconda

### Guide d'installation Anaconda

1. Aller sur la [page d'installation d'Anaconda](https://www.anaconda.com/products/distribution) et choisir l'installateur correspondant à votre système d'exploitation (Windows, Mac ou Linux). Sélectionner **Python 3.10** ou une version supérieure.
   
2. Suivre les instructions d'installation (très similaire à l'installation de tout autre logiciel).
   
3. Une fois installé, ouvrir le logiciel **Anaconda Navigator** via une recherche sur votre machine.

## Mise en place de l'environnement pour le classificateur d'images

1. Télécharger le fichier `formation-IA.yml` (fourni avec ce projet).
2. Ouvrir **Anaconda Navigator**, aller dans l'onglet **Environments**, puis sélectionner **Import**.
3. Sélectionner le fichier `formation-IA.yml`, importer l'environnement et l'activer.
4. Ouvrir **Spyder** depuis l'environnement `formation-IA`.

## Tester l'installation de TensorFlow

### Test TensorFlow

Ouvrir **Spyder** et exécuter le code suivant pour vérifier que TensorFlow est correctement installé :

```python
import tensorflow.compat.v1 as tf
tf.disable_v2_behavior()

hello = tf.constant('Hello, TensorFlow!')
with tf.Session() as sess:
    print(sess.run(hello))