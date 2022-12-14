# ml_finalproject
Plant Recommendation Engine from the Missouri Botanical Garden plant database

Project Description

As a practicing landscape architect, I’m interested in the ways that data analysis and visualization can strengthen the profession. The concepts introduced so far in the course makes me think machine learning can help make certain aspects of the job easier. A lot of developing selecting plant material comes with experience and seeing what works in the field. However, I've noticed that landscape architects tend to stick to a particular palette, and are sometimes hesitant to try new plants.

After scraping the Missouri Botanical Garden plant database (see pfch_finalproject repo), I created a plant recommendation engine that uses cosine similarity to identify similar plants and return the top 5 most similar plants. Hopefully this will inspire people to expand and experiment with new plants they didn't think to use.

This project uses Python in Jupyter Notebook, and I have included the scraping results as a CSV.

As someone new to Python and machine learning, I struggled with cleaning and formatting my data properly for the cosine similarity. This required encoding and normalizing all of the categorical feastures, in order to do a pairwise comparison of vectors. It was also my first time working with accessing information via an index and a matrix, which became challenging when writing the actual function to return the results. After finally being able to write a function to return the top 5 similar results, I realized that it was a little unhelpful for inspiring someone to use new plants since it would just recommend different varieties of the same plant. As a result, the function now filters results that share the same common name, so it gives completely unique results. While this may not be the best way to filter out similar plants, becuase now it recommends plants that may not even be the same type of plant as the target plants, the results it returns are still interesting becuase the features are mathematically similar.

Some basic next steps in this project might be to figure out the best way to fill NA values in the dataframe and try different models to see if the results make a little more sense. I think something else that might be useful is to also filter the results by plant type, but the model as is is quite thought provoking.

Future goals for this project are to scrape the rest of the text data from the Missouri Botanical Garden plant pages, parse, and extract additional features from those paragraphs. This would add more complexity to the dataframe, but hopefully make the analysis more accurate to someone who is familiar with plants. Ultimately, I still have a dream to create a machine learning model that will predict the survival of a plant in a given location, and will be working to compile data on this, so please reach out if you would like to collaborate!
