# cse6432somefunteamname
DESCRIPTION

The objective of this project is to research, design, and implement a Board Game Recommender System where users can input a board game they like and receive the most similar games. The end goal will be to implement a scikit learn k-means clustering model paired with a visualization that allows a user to select a board game that they enjoy and the output will suggest additional similar games the user may be interested in.

This implementation uses a novel dual-layered k-means clustering model to generate general clusters on dimensionality reduced data, where games within each cluster are assigned cosine similarity scores both inside and outside of their respective clusters. This allows the algorithm to easily and accurately recommend closely related games even with sparse input data. The preprocessing that was conducted to generate game similarity significantly speeds up recommendation time, as calculations do not have to be done on the fly, and allows for a seamless user interaction.

The top five game recommendations by similarity score to the selected board game are visualized as a column chart with a color scale that eases interpretation. Users can repeatedly use the system to explore by re-entering a newly recommended game for five additional recommendations.

INSTALLATION

Refer to the requirements.txt for python packages required
R version 4.0.0 or greater is suggested to run the Rmarkdown (.Rmd) for the UI. Current versions of tidyr, dplyr, and plotly should be loaded.

EXECUTION

IF OUTPUT FOLDER NOT POPULATED: Run kmeans.ipynb notebook from end to end to populate the output folder. If output folder is populated move on to step 2
Once the data is loaded into the data folder, KNIT (not run) the .Rmd script so it launches the flexdashboard. This will allow the user to interact with the data and select a game to see what the top 5 most similar games are based on similarity score.
