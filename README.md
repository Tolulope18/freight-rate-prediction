# Freight Rate Prediction

Machine learning project for predicting posted freight rates from load characteristics.

## Project Structure

```text
freight-rate-prediction/
│
├── freight_rate_prediction.ipynb
├── score.py
├── requirements.txt
├── README.md
├── validation_predictions.csv
├── december_predictions.csv
│
└── data/
    ├── train_test.csv
    ├── validation.csv
    └── december.csv
```

## Data

The assessment provides three datasets:

* `train_test.csv` — labelled development data used for model training and validation.
* `validation.csv` — unlabeled data used to generate the final 12,000 predictions.
* `december.csv` — December data used to generate the required December predictions and chart.

Place the provided datasets inside the `data/` folder.

## Setup

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Running the Project

Open and run:

```text
freight_rate_prediction.ipynb
```

The notebook handles data preparation, feature engineering, model training and prediction generation.

The final prediction files are:

```text
validation_predictions.csv
december_predictions.csv
```

## Scoring

Run the provided scoring script with:

```bash
python score.py --predictions validation_predictions.csv --december-predictions december_predictions.csv
```

This checks the prediction files and generates the required December prediction chart.
