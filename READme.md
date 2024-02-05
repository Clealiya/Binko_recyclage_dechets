Ce dépôt Github concerne le prototypage d'un classifieur de déchets multiclasses dans le cadre de mon stage "ouvrier" de 2 mois de 1e année d'école d'ingénieure à Centrale Méditerranée, en 2022. 

Le classifieur s'inspire des modèles classiques de classifieurs (MobileNet et ResNet) afin de comparer les différentes performances sur les données visuelles de l'entreprise

Le projet a été effectué avec Tensorflow et Pytorch afin de donner la possibilité à l'entreprise de reprendre le projet avec la librairie qu'il souhaite.

Le projet s'est suivi d'une optimisation des hyperparamètres à travers un POC, qui n'est pas présent dans le repository pour des raisons de confidentialités. 

## Données
Données visuelles de l'entreprise confidentielles, non fournies avec le projet. 

## Contenu :

Dans ce projet vous trouverez les dossiers et fichiers suivants: 

- `/IA_pytorch/src`: dossier du code source du modèle **ResNet** utilisant la librairie Pytorch
    - `generator.py`: script de génération des données pour le modèle
    - `model.py`: modèle utilisé
    - `parameters.py`: fichier des paramètres et hyperparamètres du modèle
    - `predict.py`: script d'inférence du modèle
    - `requirements.txt`: cf. section Execution du code
    - `train.py`: script d'entraînement du modèle
    - `traitement.py`: script de traitement des données d'entrées selon leur format
- `/IA_tensorflow/src`: dossier du code source du modèle **MobileNet** utilisant la librairie TensorFlow
    - `generator.py`: script de génération des données pour le modèle
    - `model.py`: modèle utilisé
    - `parameters.py`: fichier des paramètres et hyperparamètres du modèle
    - `predict.py`: script d'inférence du modèle
    - `requirements.txt`: cf. section Execution du code
    - `train.py`: script d'entraînement du modèle
    - `traitement.py`: script de traitement des données d'entrées selon leur format

## Execution du code
Installez les librairies nécessaires: 
```sh
pip install -r requirements.txt
```

Les fichiers .py sont équipés du test 
```python
if __name__ == '__main__':
```
Pour exécuter l'entraînement d'un des deux modèles, il suffit d'executer dans le terminal:
```sh
python <nom du fichier>
```