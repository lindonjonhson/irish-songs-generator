# irish-songs-generator

This project is a poetry/song generator through the use of Recurring Neural Networks, made with the support of the Tensorflow team.

They have a series of videos on NLP that can be seen [here](https://www.youtube.com/watch?v=fNxaJsNG3-s&list=PLQY2H8rRoyvzDbLUZkbudP-MFQZwNmU4S&index=1).

Instead of a dataset, in this project we used the lyrics of irish songs compiled in one large txt file.

At first we had to use the tokenizer to transform each line in a sequence, after that we had to create all the possible ngrams of that phrase until it is completed.

This is important as it will create a dataset with all the different word configurations, which our model will use to create the next verses of our song/poem.

Once the ngrams were made, we had to pad the sequences so they had all the same size, and most importantly, one-hot encode the labels for the model.

After that, we just had to run the data through the model and once it ready, we could give our phrase to the model and ask it to finish the song for us.

Feel free to take a look at the code and make any changes to it.
