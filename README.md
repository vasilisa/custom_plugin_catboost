# DATAIKU Plugin for custom Python model

## Why: 
Custom scikit-learn compatible ML model could be wrapped up into a plugin. 
This allows to: 
- Use all visual ML capabilities inside Dataiku
- Use hyperparameter optimisation which is not accessible if you create a custom Python model in the lab directly 

## Example with Catboost model 
**Prerequisites**
- you need to create a ```code-env``` with catboost and make it available as part of your lab running environment in Dataiku
- No need to create a special code environment within the plugin

**Steps to create a plugin**: 

1. Go to Administration -> Plugins -> Plugin Development
2. Initiate a new component 

<img width="855" alt="Screenshot 2023-07-13 at 15 10 09" src="https://github.com/vasilisa/custom_plugin_catboost/assets/2486429/efb4df1d-3c63-42ac-8693-d10c59458d44">

2. Select "Prediction Algorithm" component 
<img width="734" alt="Screenshot 2023-07-13 at 15 09 56" src="https://github.com/vasilisa/custom_plugin_catboost/assets/2486429/dc828eb5-00e8-419b-a55a-c6a90ef9f845">

3. Fill in the ```algo.py``` and ```algo.json files```
4. Fill in ```plugin.json``` with the plugin description information 

### More information on plugin development tutorials [here](https://knowledge.dataiku.com/latest/plugins/development/index.html)
### Git with developed and approved by Dataiku plugins [here](https://github.com/dataiku/dataiku-contrib)
### For more advanced custom model development as a plugin see Generalizied Linear Model plugin git [here](https://github.com/dataiku/dss-plugin-generalized-linear-models)
