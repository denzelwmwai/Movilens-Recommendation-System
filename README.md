# MovieLens Movie Recommendation System Using Collaborative Filtering

**Machine Learning Project — MovieLens `ml-latest-small`**

This repository contains the **original supplied notebook, renamed for the assignment without altering its contents**. It implements a movie recommendation system that identifies **five previously unrated films** using collaborative filtering on MovieLens ratings.

## Scope

The notebook covers the research problem and objectives, a data-quality audit and cleaning, exploratory data analysis (EDA), a reproducible train/validation/test evaluation, collaborative-filtering model development, top-five ranking metrics, five recommendations for an existing MovieLens user, and an optional new-user onboarding demonstration.

The models include a regularized rating-bias baseline, user-based *k*-nearest-neighbor (KNN) collaborative filtering, and biased matrix factorization. Evaluation includes **Precision@5, Recall@5, NDCG@5, Hit Rate@5, RMSE, and MAE**. The notebook documents the splitting, selection, and testing methodology.

## Repository structure

```text
MovieLens_Collaborative_Filtering_Recommendation_System/
├── MovieLens_Collaborative_Filtering_Recommendation_System.ipynb    # Original notebook, renamed only
├── ml-latest-small.zip                                  # Dataset archive; required by the notebook
├── requirements.txt                                     # Python dependencies
├── README.md                                            # Project and run instructions
└── .gitignore                                           # Local/generated files excluded from Git
```

## Running the notebook

1. Clone or download this repository and open a terminal in its root directory.
2. Install the dependencies using `python -m pip install -r requirements.txt`.
3. Launch Jupyter with `jupyter lab` (or open the notebook in Google Colab).
4. Run the notebook cells in order. **Keep `ml-latest-small.zip` in the same working directory as the notebook** - the notebook expects this exact filename and the enclosed `ml-latest-small/` directory.
5. The notebook extracts the CSV files to `data/raw/` and saves evaluation reports in `outputs/` automatically.

For **Google Colab**, upload both the `.ipynb` and `ml-latest-small.zip` into the Colab runtime working directory before running the notebook. No notebook edits are needed when its working directory contains the ZIP.

## Data provenance and permissions

Dataset: [MovieLens ml-latest-small](https://grouplens.org/datasets/movielens/latest/), GroupLens Research, University of Minnesota. The archive includes the original dataset `README.txt` containing the GroupLens usage conditions. This dataset is for research use; commercial use requires separate permission under the stated data license. The dataset is not endorsed by GroupLens or the University of Minnesota for this project.

Reference: Harper, F. M., & Konstan, J. A. (2015). *The MovieLens Datasets: History and Context*. ACM Transactions on Interactive Intelligent Systems, 5(4), Article 19. https://doi.org/10.1145/2827872

## Notebook integrity

The Jupyter notebook was **not rewritten, reformatted, re-executed, or altered** while creating this repository. Its original cell code, prose, metadata, and saved outputs are preserved byte-for-byte; only the `.ipynb` filename is different. This README, dataset archive, requirements and `.gitignore` are separate supporting files.
