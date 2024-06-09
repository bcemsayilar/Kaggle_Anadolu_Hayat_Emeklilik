# Anadolu Hayat Emeklilik Datathon Project

This project contains code and data from a datathon held at the beginning of the year for Anadolu Hayat Emeklilik. The dataset includes detailed customer and product information, which is used to develop and optimize models for predicting customer behavior and product usage.
## Private score (weighted F1)  : 0.2434 - 120/185
## Public score  (weighted F1)  : 0.2550

## Description

The dataset includes the following features:

- **MUSTERI_ID**: Unique IDs distinguishing customers.
- **LABEL**: Type of life insurance product the customer has purchased.
- **FLAG**: The month to which the data belongs.
- **PP_CINSIYET**: Gender of the policyholder. (1: Male, 2: Female)
- **PP_YAS**: Age of the policyholder in months.
- **PP_MESLEK**: Occupation of the policyholder.
- **PP_MUSTERI_SEGMENTI**: Customer segment of the policyholder.
  - 101: A segment
  - 102: B segment
  - 103: C segment
  - 104: D segment
  - 105: E segment
  - 106: F segment
- **PP_UYRUK**: Nationality of the policyholder.
  - 1: Turkish Citizen
  - 2: Blue Card
  - 3: Foreign National
- **IL**: Province codes where policyholders reside (0 = Abroad).
- **SORU_YATIRIM_KARAKTERI_CVP**: Investment character based on survey responses.
- **SORU_YATIRIM_KARAKTERI_RG**: Time elapsed since the investment character survey response (months).
- **SORU_MEDENI_HAL_CVP**: Marital status based on survey responses.
- **SORU_MEDENI_HAL_RG**: Time elapsed since the marital status survey response (months).
- **SORU_EGITIM_CVP**: Educational status based on survey responses.
- **SORU_EGITIM_RG**: Time elapsed since the educational status survey response (months).
- **SORU_GELIR_CVP**: Income status based on survey responses.
- **SORU_GELIR_RG**: Time elapsed since the income status survey response (months).
- **SORU_COCUK_SAYISI_CVP**: Number of children based on survey responses.
- **SORU_COCUK_SAYISI_RG**: Time elapsed since the number of children survey response (months).
- **BES_AYRILMA_TALEP_ADET**: Number of requests to withdraw from BES account.
- **ODEMEME_TALEP_ADET**: Number of non-payment instructions given in the last year.
- **HAYAT_AYRILMA_TALEP_ADET**: Number of requests to withdraw from life insurance.
- **BILGI_TALEP_ADET**: Number of information requests regarding the contract.
- **VADE_TUTAR_0 - VADE_TUTAR_11**: Total installment amounts for the last 12 months.
- **ODEME_TUTAR_0 - ODEME_TUTAR_11**: Total payment amounts for the last 12 months.
- **SON_AY_KATKI_MIKTARI**: Total additional contribution payments in the last month (TL).
- **SON_AY_KATKI_ADET**: Number of additional contribution payments in the last month.
- **SON_CEYREK_KATKI_MIKTARI**: Total additional contribution payments in the last quarter (TL).
- **SON_CEYREK_KATKI_ADET**: Number of additional contribution payments in the last quarter.
- **SON_SENE_KATKI_MIKTARI**: Total additional contribution payments in the last year (TL).
- **SON_SENE_KATKI_ADET**: Number of additional contribution payments in the last year.
- **ANAPARA**: Total principal amount invested (TL).
- **GETIRI**: Total return on investment (TL).
- **BU1 - BU24**: Ownership status of BES products 1-24 (Details in a separate document).
- **HU1 - HU19**: Ownership status of Life insurance products 1-19 (Details in a separate document).
- **AKTIF_ILK_POLICE_RG**: Time elapsed since the earliest active policy (months).

Custom Metric Coefficients:

| Product | Coefficient |
|---------|-------------|
| HU06    | 0.0385      |
| HU07    | 0.0328      |
| HU11    | 0.2791      |
| HU12    | 0.1812      |
| HU14    | 0.0113      |
| HU15    | 0.2952      |
| HU19    | 0.1614      |
| UA      | 0.0001      |

## Project Overview

The main objective of this project is to build and optimize predictive models using the given dataset. The models aim to predict various customer behaviors and product usage patterns. The weighted F1 score, which measures the balance between precision and recall, was used as the primary evaluation metric. 

### Key Findings

- The initial weighted F1 score obtained was **0.14**.
- After further optimization and tuning, the final weighted F1 score achieved was **0.026**.

### Notebook Details

The Jupyter Notebook provided in this repository includes the following sections:

1. **Data Preprocessing**:
   - Loading and inspecting the dataset.
   - Handling missing values.
   - Encoding categorical variables.
   - Feature scaling.

2. **Exploratory Data Analysis (EDA)**:
   - Visualizing the distribution of key features.
   - Identifying correlations between features.
   - Understanding the target variable distribution.

3. **Model Building**:
   - Splitting the data into training and testing sets.
   - Implementing various machine learning models (e.g., Logistic Regression, Decision Trees, Random Forest).
   - Hyperparameter tuning using GridSearchCV.
   - Evaluating model performance using the weighted F1 score.

4. **Model Optimization**:
   - Analyzing model performance and identifying areas for improvement.
   - Feature engineering and selection.
   - Advanced hyperparameter tuning.
   - Ensemble methods to improve prediction accuracy.

5. **Results and Conclusion**:
   - Summarizing the findings.
   - Discussing the performance of different models.
   - Providing insights and potential next steps for further improvement.

## Documentation

[Documentation](https://linktodocumentation)

## License

[MIT](https://choosealicense.com/licenses/mit/)
