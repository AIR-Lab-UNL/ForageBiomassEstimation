# ForageBiomassEstimation
Codes and example data for forage biomass estimation with Random Forest Regression

There were two steps:

    S1: Training a Random Forest Regression based forage biomass estimation model
        Code file: "S1_RF_forage_biomass.ipynb"
        Data needed: "Modeling_data_example.csv" under the folder "S1_RandomForest_estimation"
            Notes: This CSV file includes only 20 data points from our project, provided as an example to demonstrate the reproducibility of our code. The full dataset cannot be shared due to confidentiality policies. AlThough this example won't present the same results shown in our paper, we highly ensure it provides enough details for the complete reproducibility of study; readers can construct a dataset in the same format using their own ground sampling data and drone remotely sensed VIs, and use our codes to train their own forage biomass estimation model.
        Output: two pretained forage biomass estimation models, respectively for "livebiomass" and "totalbiomass", under the folder "S1_RandomForest_estimation"

    S2: Applying the pretrained forage biomass etimation model to UAV images to create esimated forage biomass maps
        Code file: "S2_UAV-estimated forage biomass map generation.ipynb"
            Notes: This code file uses the pretained livebiomass estimation model as an example, to predict livebiomass on June 28, 2021.
        Data needed: (1) The pretained livebiomass estimation model file, "Livebiomass_RF_model.joblib" under the folder "S1_RandomForest_estimation";
                     (2) The UAV maps of the predictor variables collected on June 28, 2021.
        Output: A map of predicted livebiomass estimation on June 28, 2021. 


