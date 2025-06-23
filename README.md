# TennisPredictionModel


Trained on this dataset: https://www.gigasheet.com/sample-data/atp-tennis-2000-2024

This includes matches from 2000 to 2024, however until 2006, there was no ATP ranking points data so I truncated the data to only include matches from 2006 to 2024.

It is currently producing 63% accuracy, compared to %50 accuracy from guess work, is pretty decent. I wanted to aim for 75-80% using rolling averages and potentially an ELO ranking system, but the early stages of me testing rolling averages has shown minimal improvements.

This data set doesn't include data from the 2024 Australian Open, so when testing the model on a few First Round games, I saw some pretty promising results. I aim to have the model run on the entire tournament and see if it correctly predicts that Jannik Sinner would win. 

I also wanted to highlight some model bias at this current stage of testing. I am currenlty calculating rolling averages in the past 8 matches for only Player_1. This gives more detailed information to the model about how Player_1 is preforming in the past, while no information about Player_2's past preformance data is shown. 
