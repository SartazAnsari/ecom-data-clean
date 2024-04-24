# E-Commerce Sales Data Cleaning Project

## Overview
This project involves downloading and cleaning sales data downloaded from Kaggle. The dataset used can be found [here](https://www.kaggle.com/datasets/sartazansari/e-commerce-sales-dataset). The dataset has been categorized into different folders for better organization.

***Note:** The original dataset is provided by [The Devastator](https://www.kaggle.com/thedevastator) in Kaggle and can be found [here](https://www.kaggle.com/datasets/sartazansari/e-commerce-sales-dataset). Credit goes to the dataset provider for making it available.*

## Dataset

The dataset is structured into the following categories:
* Expense
* Inventory
* Pricing
* Sales
* Warehouse

## Environment Setup

1. Clone the repository to your local machine:
   ```
   git clone https://github.com/SartazAnsari/ecom-data-clean.git
   cd ecom-data-clean
   ```

2. ### Conda Setup
    1. Create a new Conda environment:
        ```
        conda create --name ecom-data-clean-env python=3.12
        ```
    2. Activate the environment:
        ```
        conda activate ecom-data-clean-env
        ```
    3. Install the required packages:
        ```
        conda install -c conda-forge ipykernel
        conda install -c conda-forge kaggle
        conda install pandas #if not installed
        ```
3. ### Python Setup (Alternative)
    1. If you prefer Python’s built-in virtual environment
        ```
        python -m venv ecom-clean-data-env
        ```
    2. Activate the environment:
        * Windows:
            ```
            ecom-clean-data-env\Scripts\activate
            ```
        * Unix or MacOS:
            ```
            source ecom-clean-data-env/bin/activate

            ```
    3. Install the required packages:
        ```
        pip install ipykernel
        pip install kaggle
        pip install pandas
        ```

## Setting up the Kaggle API
1. Sign in to **Kaggle** and navigate to the **Account** tab of your user profile.
2. Scroll down to the **API** section and click on **Create New API Token**. 
3. This will download a file named ```kaggle.json``` containing your API credentials.
4. Place the ```kaggle.json``` file in the ```~/.kaggle/``` directory. If the directory does not exist, create it.
5. You're all set up! You can now use the Kaggle API to download datasets directly to your project.

## Cleaning Process
The cleaning process involves reading, cleaning, and organizing the data files from each category. Specific cleaning functions are implemented for each category to ensure data consistency and accuracy.

## Usage
To clean the data, execute the provided Python script. It will automatically clean the data files and save the cleaned versions in the “Clean Dataset” directory.