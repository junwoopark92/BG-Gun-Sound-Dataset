# BGGunSoundDataset
This repository provides the official BGG dataset and implementation of the following paper: 
"Enemy Spotted: In-game Gun Sound Dataset for Gunshot Classification and Localization" accepted at Conference of Games (GoG) 2022.


## Dataset
1. Unzip the "gun_sound_v2.zip" in data folder.
2. Follow the path structure below.
```
BGGunSoundDataset
├── data
    ├── gun_sound_v2
    │   ├── ak_0m_center_0000.mp3
    │   ├── ak_0m_center_0001.mp3
    │   ├──  ...
    │   └── scar_0m_center_2194.mp3
    ├── v3_exp1_train.csv
    ├── v3_exp1_test.csv
    ├── v3_exp2_train.csv
    └── v3_exp2_test.csv
```

## Run Gunshot classfication and Localization on BGG dataset.

### Gunshot Classification
```
train_classification.py  --backbone {CNN, RNN, CRNN, Trans, CTrans} --lr 1e-3 --input_sec 2
```
### Gunshot Localization
```
train_localization_and_classification.py --backbone {CNN, RNN, CRNN, Trans, CTrans} --lr 1e-4 --input_sec 3
```

## Citation
```

```
