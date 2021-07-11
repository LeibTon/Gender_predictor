# Gender_predictor
Using LSTM to predict gender(M/F) of Hindu Names.

## Data:

All names have been extracted from [hindunames.net](hindunames.net) using web scraping.  
Total Number of Boy Names: 2966  
Toatal Number of Girl Names: 1596  

## Model:

Bidrectional LSTM have been used to learn features of characters that made up name. Below is a brief description of the model:
![Model](/model.png)

All the data is used to train the model, so there is no validation dataset. Hence can check is the model is overfitting. Accuracy achieved after 100 epochs is 90.47%.  

### Testing

```
Ap is a Male name. | Prediction: 0.68927544
Arjun is a Male name. | Prediction: 0.9617493
Ananya is a Female name. | Prediction: 0.4445054
Sonam is a Male name. | Prediction: 0.90388197
Sohal is a Male name. | Prediction: 0.93381894
Anshita is a Female name. | Prediction: 0.020775735
Amisha is a Female name. | Prediction: 0.04405147
Salman is a Male name. | Prediction: 0.94363177
Jagdish is a Male name. | Prediction: 0.99922925
Aditya is a Male name. | Prediction: 0.9266465
Archit is a Male name. | Prediction: 0.9564622
Bidhan is a Male name. | Prediction: 0.9251536
Azhar is a Male name. | Prediction: 0.98485863
Jesicca is a Female name. | Prediction: 0.057892382
Johnny is a Male name. | Prediction: 0.8201932
Ram is a Male name. | Prediction: 0.7771222
Lakhan is a Male name. | Prediction: 0.9541757
```

## Files:

- [Saving Names.ipynb]("/Saving Names.ipynb"): Used to extract names from hindunames.net  
Libraries: requests, re

- [Gender_Predictor.ipynb](/Gender_Predictor.ipynb): Data Preprocessing, Model, Training, Testing.  
Libraries: tensorflow, numpy

Link to Original Colab Notebook: [Notebook](https://colab.research.google.com/drive/1jcFV2MSkdxemjAK5beGt13RganAH-Q0S?usp=sharing)



