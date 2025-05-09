# MaskDino cable detection and segmentation
## Requisiti
Librerie necessarie per eseguire il codice:
* cocohelper
* pycocotools
* gitpython
* detectron2

## Project Overview
Addestramento del modello MaskDino (nella versione large da 223B parametri) per i task di object detection e segmentazioni di elementi costitutivi associati a tralicci in viste aeree.
L'addestramento del modello è stato effettuato usando il dataset TTPLA: An Aerial-Image Dataset for Detection and Segmentation of Transmission Towers and Power Lines [Y. Lu et al., 2021].\\
Al fine di ottenere le migliori performance possibili si sono sfruttate anche tecniche di data augmentation al fine di ridurre eventuali problemi di sottorappresentazioni di diverse componenti dei tralicci.

## Data Augmentation
Le principali tecniche di data augmentation usate sono state:
* Capovolgimento immagine
* Crop
* Resize
* Variazione saturazione
Non si sono usate tecniche di rotazione in quanto il dataset già includeva dati augmentati tramite tale tecnica.

## Risultati
