# WSQ_hackathon
A Recommender model that helps to match Job seekers to possibly new roles by 
comparing their similarity coefficient with the next nearest neighbour

The model's permise works based on given OCEAN personality type, ( https://en.wikipedia.org/wiki/Big_Five_personality_traits ),
it will match one jobseeker another individual with the top 3 closest similarity score, and suggest to the person, the 3 closest
job roles and industry, that the person could consider looking at, as in today's market, jobs are consistently changing, and with
a large enough dataset, a person may discover a new industry or a profession, that they might not have considered previously, due to
lack of information

This leads to the first weakness of the model, which is that it requires a large pool of samples in order to be effective, however, after 
the critical mass point, we believe that the model would grow more accurate

Recommender systems are not new, they have been used by places such as netflix and amazon, to recommend similar products to consumers, 
but we considered this as a new use case

< For implemtation > 
The dataset would be collected by a workforce counselor, or in an ideal situation, would be automatically collected via an online
game that derives the score,  currently, we are using an anonymized dataset to run the simulation


The DF.csv file contains the data we used to train the model with (extraversion,	independ,	selfcontrol,	anxiety,	novator),
continuous variables were scaled with standard_scalar from scikit-learn, so that no one numeric factor would have a larger effect on the
model, and cosine similarity distance measure was used

Once the model is trained, a new individual can enter his details via "RecommenderLanding.html" , with flask running as the webserver,
and the flask webserver will return the top 3 professions and industries that the person could try to explore


** Note : Spectre 0.5.3 was used as the CSS library to add some romance to the project and jazz it up a little

Appreciate the effort for reading this =)
