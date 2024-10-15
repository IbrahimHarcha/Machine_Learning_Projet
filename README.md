PROJET HAI923I - 2024-2025

Ce projet est à réaliser en groupe, composé de 3 à 4 personnes maximum.

Informations générales
Les consignes concernant le rendu, les dates importantes ainsi que le lien d'inscription pour préciser la composition de votre groupe seront bientôt disponibles. En attendant, vous pouvez déjà commencer à travailler sur le projet.

Objectif du projet
Comme expliqué en amphithéâtre, le projet consiste à travailler sur des images et à développer des modèles de classification pour différents jeux de données. Vous avez à votre disposition trois jeux de données différents :

Tiger vs autres animaux
Fox vs autres animaux
Elephant vs autres animaux
Les jeux de données ainsi que les premiers pré-traitements sont disponibles dans le notebook de la section projet 2024-2025.

Remarque importante
Les jeux de données ne sont pas très volumineux (200 éléments par classe) afin de réduire les temps d’apprentissage. Cependant, en fonction des modèles utilisés ou si vous générez des images, l’apprentissage peut prendre plus de temps. Pensez à utiliser des GPU sur Google Colab pour accélérer le processus (via le menu Modifier > Paramètres du Notebook).
N'oubliez pas d’utiliser des checkpoints pour sauvegarder les modèles en cours d'apprentissage, cela est utile si la session est interrompue.

Un guide pratique est disponible ici :
How to Continue Training a Saved and Loaded Keras Model

Travail à réaliser
Modèle baseline
Créez un modèle de classification de base (modeleBaseline) avec une seule couche CNN et évaluez-le sur les différents jeux de données. Vérifiez si ce modèle est performant pour toutes les classes d’animaux et ajustez les hyperparamètres sans modifier le modèle pour essayer d'améliorer la classification d'une classe spécifique. Sauvegardez les résultats pour le rapport final.
Améliorations des modèles
Proposez des améliorations pour chaque classe d'animaux avec des architectures de modèles adaptées : modeleTiger, modeleFox, et modeleElephant. Testez chaque modèle sur les autres classes pour évaluer leurs performances. Sauvegardez également les résultats.
Génération de nouvelles données
Utilisez l'Image Data Generator pour générer de nouvelles données et comparez les performances des classifiers précédents (modeleBaseline, modeleTiger, modeleFox, modeleElephant) sur ces nouvelles données. Développez de nouveaux modèles si nécessaire : modeleIDGTiger, modeleIDGFox, modeleIDGElephant. Sauvegardez les résultats pour le rapport.
Transfer Learning
Appliquez une approche de Transfer Learning en utilisant des modèles existants (par ex. RESNET, VGG) sur les trois jeux de données : modeleTLTiger, modeleTLFox, modeleTLElephant. Comparez les performances avec les modèles précédents.
Génération d'images avec GAN
Utilisez un GAN pour générer des images de renards à partir du jeu de données Fox. Sélectionnez et sauvegardez 10 images générées. Utilisez votre meilleur modèle précédent (modeleFox, modeleIDGFox, ou modeleTLFox) pour prédire ces images et vérifiez comment elles sont perçues par le modèle.
Visualisation des features maps
Affichez les features maps des couches CNN de votre modèle le plus complexe.
Optionnel - Autoencodeurs et coloration d'images
Si vous êtes intéressé par les autoencodeurs ou les variational autoencoders, essayez de faire de la coloration d’images en utilisant un autoencodeur pour convertir des images en noir et blanc en images couleurs. Utilisez le jeu de données Tiger pour cet exercice (voir exemple ici).
Optionnel - Interprétabilité du modèle
Explorez les parties des images qui ont influencé la décision de votre classifieur. Vous pouvez utiliser des techniques comme LIME pour obtenir des insights supplémentaires.
