**Readme** -
For part 1:
Install the necessary modules using the following commands in a anaconda environment. Run the script to get the regression results <br>

%pip install pandas <br>
%pip install matplotlib <br>
%pip install seaborn <br>
%pip install pandas-profiling <br>
%pip install scikit-learn <br>
%pip install lightgbm <br>
%pip install catboost <br>
%pip install scikit-optimize <br>
%pip install ipywidgets <br>

For part 2:
To run the script, you will need the following:
1. './twitter_files_v3/entities.pkl' - Dictionary of entities generated in module 2, also provided in the zip file
2. './twitter_files_v3/prediction_data.pkl' - Prediction data generated in module 2, also provided in the zip file
3. './glove/glove.6B.100d.txt' - Glove embeddings

For each task - **you need to provide 4 inputs** - 
1. **entity** (from the list of entities),
2. **pred_type** (game_day (predicts in last 10 min), reg_day (predicts for entire day))
3. **task_type** (from "sentiment", "summary", "keywords")
3. **date** (format %Y-%m-%d for reg_day; %Y-%m-%d %H:%M:%S for game day)

The 3 task types are: 
1. 'sentiment': returns the sentiment of the set of tweets for a given entity for the given day or in last 10 min if prediction type is game_day.
2. 'summary': returns list of 4 tweets which summarize the tweets for a given entity for the given day or in last 10 min if prediction type is game_day.
3. 'keywords': returns list of 10 key phrases that appear in context of a given entity for the given day or in last 10 min if prediction type is game_day.
