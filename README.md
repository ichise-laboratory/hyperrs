# hyperrs

This project follows BSD 3-Clause License.

Source Code for the paper "HyperRS: Hypernetwork-based Recommender System for the User Cold- Start Problem"

Dependencies:

tqdm
tensorflow 2.8.0
numpy

Requirement:

At least 10GB GPU memory.
At least 32GB memory.


1. Download the preprocessed data from (this will be replaced by an URL from our lab page).
2. Unzip the `data.tar.gz`. Move all files in the same directory with `trainer.py`
3. Modify `DATASET` in `dataset_info.json` to choose `ml-10m` (Movielens), `tokyoTV` (Tokyo TV), `Book` (BookCrossing) 
4. Use `python trainer.py -m [CONFIG_FILE_NAME]` to train the dataset.
[CONFIG_FILE_NAME]: HyperRS.ml-10m.C-W for Movielens, Cold User Warm Item.

Change the `use_existing_items` in the [CONFIG_FILE_NAME] to `false` to test the Cold User Cold Item setting.
