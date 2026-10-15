# Parasite Egg Classification — Deep Learning on KFM Microscopy Images

**Università degli Studi di Napoli Federico II | Machine Learning 2025/2026**

Progetto di classificazione multiclasse di immagini microscopiche (10 categorie di elementi parassitari e artefatti) nell'ambito della challenge **UniNa – ML 25/26 – Parasite Egg Classification Contest**. Il dataset AI-KFM contiene patch 224×224 ottenute dal Kubic FLOTAC Microscope (KFM) in condizioni operative reali: possibili detriti, variazioni di illuminazione, sfocatura, somiglianza fra classi e sbilanciamento.

## Metodologia
Il lavoro comprende analisi dei dati, suddivisione stratificata, data augmentation, transfer learning e fine-tuning, confronto tra **ConvNeXt-Tiny** ed **EfficientNetV2-S**, sette esperimenti di training, selezione dei checkpoint, ensemble pesato di tre modelli e **Test-Time Augmentation (TTA)**. La metrica di riferimento è la **Balanced Accuracy**, media del recall per classe.

## Risultati (valutazione interna)
| Metrica | Valore |
| --- | ---: |
| Balanced Accuracy | **97,61%** |
| Accuracy | **97,53%** |

I risultati sono relativi all'**hold-out interno**, **non** alla private leaderboard Kaggle. La separazione è stratificata per classe ma non per sessione di scansione; perciò le prestazioni su sessioni totalmente nuove richiedono ulteriore verifica.

## Materiali
Il notebook completo (.ipynb), la relazione tecnica PDF

**Link notebook originale su Kaggle:** (https://www.kaggle.com/code/alessiaabbagnanoo/notebookpulito)

## Competenze
Python, PyTorch, Computer Vision, Deep Learning, CNN, Transfer Learning, Fine-tuning, Cross-Validation, Ensemble Learning, Test-Time Augmentation, valutazione di modelli e analisi degli errori.

## Attribuzioni e uso
Challenge organizzata nell'ambito dell'Università degli Studi di Napoli Federico II; si ringraziano gli organizzatori e il gruppo di ricerca KFM. Il progetto è un'esercitazione accademica e non un sistema diagnostico validato. Dati e immagini restano soggetti alle regole della competizione.

**Autrice:** [alessiaabbagnano](https://github.com/alessiaabbagnano)
