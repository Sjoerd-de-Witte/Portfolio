# Portfolio

## Datacamp
![image](https://user-images.githubusercontent.com/120015853/213521634-464dedbe-4458-4ee2-bc8c-e9cf36be9165.png)
![image](https://user-images.githubusercontent.com/120015853/213521705-06b65c44-a0ef-4c54-8185-2b59ca9fae62.png)
![image](https://user-images.githubusercontent.com/120015853/213521772-867505a7-c536-458f-91ec-2336baedebbf.png)
![image](https://user-images.githubusercontent.com/120015853/213521882-16770441-f3ec-4516-9dfd-a6f60ba2dff7.png)
![image](https://user-images.githubusercontent.com/120015853/213521990-071d8d15-e157-4b85-a65c-12a23a510af8.png)
![image](https://user-images.githubusercontent.com/120015853/213522093-23018356-0baf-4b5d-870c-743df444f9f3.png)
![image](https://user-images.githubusercontent.com/120015853/213522198-f01bca37-6f37-41d5-aed8-f18ab3d39bb8.png)
![image](https://user-images.githubusercontent.com/120015853/213524020-8d886a22-693f-45a3-b379-1dc74ba35904.png)
![image](https://user-images.githubusercontent.com/120015853/213524085-a2933412-affb-4d7d-ae69-6afbf88d35a6.png)
![image](https://user-images.githubusercontent.com/120015853/213524190-714b2187-4837-421e-b090-d05ad0c5ed3a.png)
![image](https://user-images.githubusercontent.com/120015853/213524283-c6702829-72cf-4cb2-b367-e984557953e7.png)
![image](https://user-images.githubusercontent.com/120015853/213524344-777dcd26-f810-42f2-acc4-120f915f75b4.png)
![image](https://user-images.githubusercontent.com/120015853/213524433-4c55ee06-690e-4fdc-9196-92b6eb178ca3.png)
![image](https://user-images.githubusercontent.com/120015853/213524512-7451ca92-7968-4111-9b1b-3a9a1bf1dff2.png)
![image](https://user-images.githubusercontent.com/120015853/213524593-7f1c6318-efbe-43ed-b59f-9b365ca67e75.png)


## Research Project

## Predictive Analytics

XGBoost is een machine learning-techniek die vaak wordt gebruikt voor verschillende soorten problemen. Het is een ensemble-techniek die gebruik maakt van beslissingsbomen. Een belangrijk kenmerk van beslissingsbomen is dat ze goed zijn in het afhandelen van non-lineaire relaties tussen variabelen. Dit maakt ze geschikt voor het voorspellen van tijdsreeksen, aangezien veel tijdsreeksen niet-lineaire patronen bevatten. Een studie uit 2016 (Friedman, et al.) toonde aan dat beslissingsbomen geschikt zijn voor het voorspellen van tijdsreeksen en dat ze presteerden beter dan lineaire modellen. Een studie uit 2018 (Chen, et al.) toonde aan dat gradient boosting algoritmen zoals XGBoost presteerden beter dan andere technieken zoals RandomForest voor tijdsreeksvoorspellingen. Er zijn ook verschillende studies die de prestaties van XGBoost voor specifieke toepassingen hebben onderzocht, zoals het voorspellen van energieverbruik (Zhang, et al., 2017) en verkeersintensiteiten (Li, et al., 2018). Beide studies concludeerden dat XGBoost de beste prestaties leverde in vergelijking met andere populaire technieken. 

In de eerste notebook heb ik voor een huisje het energieverbriuk per dag proberen te voorspellen met behulp van XGBoost. Ik heb hier gekozen om de hyperparameters voor dit huisje te finetunen met GridSearchCV. Deze notebook is mee gericht op de kwalitatieve analyse. <br>
[XGBoost met hyperparameter tuning](xgboost1.ipynb) <br>
In de tweede notebook heb ik voor alle huisjes het energie verbruik per dag geprobeerd te voorspellen met XGBoost, omdat het finetunenen van de parameters best wel veel tijd kost en het resultaat niet heel veel verschilt heb ik hier geen hyperparameters getuned. Deze notebook is meer gericht om de kwantatitatieve analyse. <br>
[XGBoost met loop over elk huisje](xgboost2.ipynb)

In deze notebook heb ik gekeken naar de RandomForestClassifier, omdat deze een hoog accuracy had bij de lazypredict, een library die alle classifier modellen op een probleem toepast. Ik heb gekeken hoeveel het model beter werdt op het moment dat we de hyperparameters gingen finetunen. <br>
[RandomForestClassifier met hyperparameter finetuning](rfr.ipynb)

## Domain Knowledge
Voor het Energieproject had ik de taak gekregen om te proberen een oplossing te vinden met behulp van XGBoost. Daarom ben ik eerst aan de slag gegaan om te begrijpen hoe dit machine learning model in elkaar zit. Ik heb hiervan een verslag gemaakt voor mezelf, maar ook voor de rest van mijn groepje om te begrijpen waar ik mee bezig was.

[XGBoost](XgBoost.pdf)

## Data Preprocessing
- interpoleren
## Communucation

### Gegeven presentaties

Ik heb de eerste externe presentatie over het Foodboost project gegeven samen met Job. Verder heb ik de derde externe presentatie over het Energie project samen met Job en Senna gegeven. Tot slot heb ik ook nog een handvol interne presentaties gegeven.

### Verslag

Voor het verslag heb ik de taak op mij genomen om hoofstuk Data, de methode, resulataten en analyse resultaten voor XGBoost te schrijven.
