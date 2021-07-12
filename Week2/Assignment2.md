# Link to MLOps Assignment
https://github.com/raja-7-c/MLOps_Assignment

# Part 1

The first part of this assignment is to evaluate your basic understanding of DVC & its functionalities, as mentioned in the notes. In this part, you need to do the following:

- Create an empty (public) GitHub repository named `MLOps_Assignment` *(This will be a separate repo from the one that you have submitted earlier).* Clone it & initialize it as a DVC repository.
- Create a `data/` folder inside `MLOps_Assignment`.
- Create a folder named `external_cache` outside this repo & set it as the cache for the repository. *(Check out the [DVC command reference](https://dvc.org/doc/command-reference) for help)*
- Download the `creditcard.csv` file from [this Credit Card Fraud dataset](https://www.kaggle.com/creepycrap/creditcard-fraud-dataset), place it in the `data/` folder & enable DVC tracking for it.
- Create a new Amazon S3 bucket (name it anything you want).
- Set the S3 bucket as the default remote for the DVC repo & upload the dataset to this bucket (into a folder named `datastore`).

***$ git clone https://github.com/raja-7-c/MLOps_Assignment***

***$ git remote add origin https://github.com/raja-7-c/MLOps_Assignment***

***$ git branch -M main***

***$ dvc init***

***mkdir data***

***touch docs/.gitkeep***

git add *

***git commit -m "create data directory"***

***git push***
