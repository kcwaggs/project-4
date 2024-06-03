# project-4
We want to determine if a machine learning model can predict a song track’s danceability (from Spotify sourced data) based on several inputs such as song speed, tempo, valence, duration, etc.

## Folders/Files
We used the main_dataset.csv as our core data from kaggle. \
To preprocess and clean the data, we did this in the test.ipynb file. \
To query the dataset we utilized the sql.ipynb file. \
To create the model, this was done in the datamodel_neuralnetwork_karen.ipynb file. \

## Notes 
Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable. \
Our team also attempted to model for a song's popularity, and were unable to create a model that could predict popularity with meaningful predictability. \


## Results
Our model was able to predict a song's danceability with 81.9% accuracy. 

### Resources
Kaggle, Chat GPT, class resources, etc. \
Dataset: https://www.kaggle.com/datasets/viktoriiashkurenko/278k-spotify-songs?select=main_dataset.csv \
Presentation slides: https://docs.google.com/presentation/d/1kCljK9yE_UL3WgDXqj0c2GfbEvztWu-yVhXjH6NgX-8/edit#slide=id.g35f391192_00