# project-4
We want to determine if a machine learning model can predict a song track’s danceability (from Spotify sourced data) based on several inputs such as song speed, tempo, valence, duration, etc.

## Required Libraries and Tools

Ensure you have the following libraries installed. These are essential for data processing, model training, and evaluation:

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **tensorflow**: For building and training the neural network model.
- **scikit-learn**: For data preprocessing, model evaluation, and metrics.
- **matplotlib**: For plotting graphs and visualizations.
- **seaborn**: For statistical data visualization.
- **sqlalchemy**: For database interactions.
- **IPython**: For enhanced interactive Python, including display tools.


### Processing:

1. First, download the [main_dataset.csv](resources/main_dataset.csv) from Kaggle as our core data and save into a resources folder.
2. Next, preprocess and clean the data using the [main_dataset_preprocessing.ipynb](./main_dataset_preprocessing.ipynb) file.
3. Then, query the dataset using the [sql_conversion.ipynb](./sql_conversion.ipynb) file.
4. Finally, create the model using the [datamodel_neuralnetwork_karen.ipynb](./datamodel_neuralnetwork_karen.ipynb) file.


### Audio Features

- **Danceability**: Describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

- **Energy**: A measure from 0.0 to 1.0 that represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.

- **Key**: The key the track is in. Integers map to pitches using standard Pitch Class notation (e.g., 0 = C, 1 = C♯/D♭, 2 = D, and so on). If no key is detected, the value is -1.

- **Loudness**: The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing the relative loudness of tracks. Values typically range between -60 and 0 dB.

- **Mode**: Indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.

- **Speechiness**: Detects the presence of spoken words in a track. The closer to 1.0 the attribute value, the more exclusively speech-like the recording (e.g., talk show, audio book, poetry). Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 may contain both music and speech, such as rap music. Values below 0.33 likely represent music and other non-speech-like tracks.

- **Acousticness**: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. A value of 1.0 represents high confidence that the track is acoustic.

- **Instrumentalness**: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater the likelihood that the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks.

- **Liveness**: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 indicates a strong likelihood that the track is live.

- **Valence**: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g., happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g., sad, depressed, angry).

- **Tempo**: The overall estimated tempo of a track in beats per minute (BPM). Tempo is the speed or pace of a given piece and derives directly from the average beat duration.

- **Duration**: The duration of the track in milliseconds.

- **Time Signature**: An estimated time signature. The time signature (meter) specifies how many beats are in each bar (or measure). It ranges from 3 to 7, indicating time signatures of "3/4" to "7/4".



## Results
Our model was able to predict a song's danceability with 81.9% accuracy. 

### Resources
Kaggle, Chat GPT, class resources, etc. \
Dataset: https://www.kaggle.com/datasets/viktoriiashkurenko/278k-spotify-songs?select=main_dataset.csv \
Presentation slides: https://docs.google.com/presentation/d/1kCljK9yE_UL3WgDXqj0c2GfbEvztWu-yVhXjH6NgX-8/edit#slide=id.g35f391192_00
