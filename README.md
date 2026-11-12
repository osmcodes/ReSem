# ReSem

Dataset available at: just download and use the dataset from "Google drive" data folder to local repository.
https://drive.google.com/drive/folders/1Glu03cg9zn1gpmrfpgxe0ZZ26GWQjSxR?usp=sharing

Take the dataset DBP15K (ZH-EN) as an example, the folder "zh_en" contains:
* ent_ids_1: ids for entities in source KG;
* ent_ids_2: ids for entities in target KG;
* ref_ent_ids: entity links encoded by ids;
* triples_1: relation triples encoded by ids in source KG (DBP_ZH);
* triples_1_s: remaining relation triples encoded by ids in source KG (S-DBP_ZH);
* triples_2: relation triples encoded by ids in target KG (DBP_EN);
* triples_2_s: remaining relation triples encoded by ids in target KG (S-DBP_EN);
* vectorList.json: the input entity feature matrix initialized by word vectors;

## Environment

* Python>=3.5
* Tensorflow>=1.8.0
* NetworkX
* Scipy
* Numpy


## Running

For example, to run ReSem on DBP15K (ZH-EN), use the following script:
```
python3 main.py --dataset DBP15k --lang zh_en
```


> Due to the instability of embedding-based methods, it is acceptable that the results fluctuate a little bit (±1%) when running code repeatedly.


## Citation
Will be provided
