# Portfolio Sjoerd de Witte

## Datacamp

* Introduction to Python 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524593-7f1c6318-efbe-43ed-b59f-9b365ca67e75.png"/>
  </details>
  
* Intermediate python
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524512-7451ca92-7968-4111-9b1b-3a9a1bf1dff2.png"/>
  </details>
  
* Python Data Science Toolbox(part 1)
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524433-4c55ee06-690e-4fdc-9196-92b6eb178ca3.png"/>
  </details> 

* Python Data Science Toolbox(part 2)
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524344-777dcd26-f810-42f2-acc4-120f915f75b4.png"/>
  </details> 

* Statistical Thinking in Python (part 1)   
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524283-c6702829-72cf-4cb2-b367-e984557953e7.png"/>
  </details> 
  
* Machine Learning with scikit-learn 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524190-714b2187-4837-421e-b090-d05ad0c5ed3a.png"/>
  </details> 
  
* Linear Classifiers in Python 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524085-a2933412-affb-4d7d-ae69-6afbf88d35a6.png"/>
  </details> 
 
* Introduction to Data Visualization with Matplotlib  
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213524020-8d886a22-693f-45a3-b379-1dc74ba35904.png"/>
  </details> 

* Model Validation in Python 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213522198-f01bca37-6f37-41d5-aed8-f18ab3d39bb8.png"/>
  </details> 

* Data Manipulation with pandas
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213522093-23018356-0baf-4b5d-870c-743df444f9f3.png"/>
  </details> 
  
* Exploratory Data Analysis in Python 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213521990-071d8d15-e157-4b85-a65c-12a23a510af8.png"/>
  </details> 

* Cleaning Data in Python 
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213521882-16770441-f3ec-4516-9dfd-a6f60ba2dff7.png"/>
  </details> 

* Machine learning for Time Series Data in Python
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213521772-867505a7-c536-458f-91ec-2336baedebbf.png"/>
  </details> 

* Time Series Analysis in Python
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213521634-464dedbe-4458-4ee2-bc8c-e9cf36be9165.png"/>
  </details> 

* Joining Data with Pandas
  <details>
  <summary>Certificaat</summary>
  <img src = "https://user-images.githubusercontent.com/120015853/213521705-06b65c44-a0ef-4c54-8185-2b59ca9fae62.png"/>
  </details>



## Predictive Analytics
Hieronder staan een aantal van de modellen die ik tijdens deze minor heb gemaakt.

### XGBoost
XGBoost is een Machine Learning-techniek die vaak wordt gebruikt voor verschillende soorten problemen. Het is een ensemble-techniek die gebruik maakt van beslissingsbomen. Een belangrijk kenmerk van beslissingsbomen is dat ze goed zijn in het afhandelen van non-lineaire relaties tussen variabelen. Dit maakt ze geschikt voor het voorspellen van tijdreeksen, aangezien veel tijdreeksen niet-lineaire patronen bevatten.  

Een studie uit 2019 toonde aan dat XGBoost geschikt kan zijn voor tijdreeks voorspellingen (Abbasi, R. A., Javaid, N., Ghuman, M. N. J., Khan, Z. A., & Ur Rehman, S, 2019).  

In de eerste notebook heb ik voor een huisje het energieverbriuk per dag proberen te voorspellen met behulp van XGBoost. Ik heb hier gekozen om de hyperparameters voor dit huisje te finetunen met GridSearchCV. Deze notebook is mee gericht op de kwalitatieve analyse. <br>
* [XGBoost met hyperparameter tuning](xgboost1.ipynb) <br>

In de tweede notebook heb ik voor alle huisjes het energie verbruik per dag geprobeerd te voorspellen met XGBoost, omdat het finetunenen van de parameters best wel veel tijd kost en het resultaat niet heel veel verschilt heb ik hier geen hyperparameters getuned. Deze notebook is meer gericht om de kwantatitatieve analyse. <br>
* [XGBoost met loop over elk huisje](xgboost2.ipynb)<br>

Vergeleken met de andere modellen die door mijn groepsgenoten (LSTM- en SVR-modellen) zijn gemaakt scoorde XGBoost slechter zowel met een lagere R2-score als een groter RMSE-waarde. Dat is ook niet verassend, want de meeste huisjes hadden een negatieve R2-score. 

### RandomForestClasssifier

In deze notebook heb ik gekeken naar de RandomForestClassifier, omdat deze een hoog accuracy had bij de lazypredict, een library die alle classifier modellen op een probleem toepast. Ik heb gekeken hoeveel het model beter werdt op het moment dat we de hyperparameters gingen finetunen. <br>

* [RandomForestClassifier met hyperparameter finetuning](rfr.ipynb)

Vergeleken met modellen die mijn groepsgenoten hadden gemaakt was RandomForest een goed model, het scoorde op alle onderdelen, accuracy, precision en recall, het hoogst.


## Data Preprocessing

Ik heb eerst de data geimporteerd en bekeken. Het eerste wat opviel was dat alle tijdstippen van de metingen waren genoteerd als timestamps, omdat dit niet makkelijk leesbaar is heb ik deze eerst omgezet naar datetimes en dubbele metingen eruit gehaald. Door naar de data van verschillende huisjes te kijken viel op dat er niet altijd om de 5 minuten was gemeten, zoals eigenlijk de bedoeling was. Soms ontbraken er hele dagen of dagdelen, daarom heb ik vervolgens de data geinterpoleerd.

De belangrijkste data voor ons waren die van de smartmeter en in het bijzonder de energy_in en energy_out, de energie de het huis van het net opneemt en afgeeft. En de data van de solarpanels en in het bijzonder de energy_out, de hoeveelheid energie die de zonnepanelen opwekken. Met deze data is namelijk het totale verbruik van een huis te berekenen.

Verder was het interessant om te zien dat als er gekeken werd naar de correlatie tussen smartmeter_energy_out en solar_energy_out, dat het bijna een op een liep. Dat betekent, dat de energie die wordt opgewekt door de zonnepanelen nauwelijks wordt gebruikt door het huis en bijna allemaal wordt teruggelevert aan het net, dit is een goed argument waarom een batterij in het huis nuttig zou kunnen zijn.

In deze notebook heb ik een huisje geanalyseerd.

* [Data voorbereiding met interpolatie](Sjoerd_interpoleren.ipynb)<br>

Later heeft Senna dit als loop voor alle huisjes gemaakt en hebben we gekeken naar de grafieken van energieverbruik naar bijzonderheden/uitschieters in deze grafiek.

Tot slot bij het voorbereiden voor de data van een machine learning model heb ik ook nog wat visualitaties gemaakt van de data.

* [Data voorbereiding voor ML model](Dataxgboost.ipynb)<br>

## Communucation

### Gegeven presentaties

Ik heb de eerste externe presentatie over het Foodboost project gegeven samen met Job. Verder heb ik de derde externe presentatie over het Energie project samen met Job en Senna gegeven. Tot slot heb ik ook nog een handvol interne presentaties gegeven. <br>
* [FoodBoost prestatie](FoodBoostEindpresentatie.pptx)<br>
* [Energie 2de presentatie](Energy2.pptx)

### Verslag

Voor het verslag heb ik de taak op mij genomen om hoofstuk Data, de methode, resulataten en analyse resultaten voor XGBoost te schrijven.

## Bronnen

Abbasi, R., Javaid, N., Ghuman, M., Khan, Z., & Ur Rehman, S. (2019, maart). Short term load forecasting using XGBoost. Springer, pp. 1120-1131. Opgeroepen op januari 19, 2023 
