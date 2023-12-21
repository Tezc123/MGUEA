# UsM2EA
An unsupervised entity alignment method based on multi-dimensional entity features and alignment seeds noise reduction

# Dataset
The DBP15K dataset comes from the [EVA](https://github.com/cambridgeltl/eva) repository. You can download the image feature following the guidance of EVA repository, and then unzip it into the `data/pkls` directory. The name feature can be downloaded from [Glove](https://nlp.stanford.edu/data/glove.6B.zip), you can unzip it into the `data/embedding` directory.

The directory structure of `data` is as follows:
```
- data
    - DBP15K
        - fr_en
        - ja_en
        - translated_ent_name
        - zh_en
    - pkls
        - fr_en_GA_id_img_feature_dict.pkl
        - ja_en_GA_id_img_feature_dict.pkl
        - zh_en_GA_id_img_feature_dict.pkl
    - embedding
        - glove.6B.300d.txt
```

# Environment
* python==3.7
* torch==1.7.0
* scipy==1.5.2
* numpy==1.19.2

# Training
```
bash run_dbp15k.sh 0 42 zh_en
bash run_dbp15k.sh 0 42 ja_en
bash run_dbp15k.sh 0 42 fr_en
```

# Citation

# Acknowledgement
Our codes are modified based on [MCLEA](https://github.com/lzxlin/MCLEA), and we would like to thank their open-sourced work.
