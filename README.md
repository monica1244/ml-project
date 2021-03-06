## Yelp Recommendation And Review Generator
#### Course project for CS 7641: Machine Learning (Prof. Mahdi Roozbahani) @ Georgia Institute of Technology
#### Further implementation details available at: https://monica1244.github.io/dining-sim/

### Overview
In this age of the internet and ease of travel, we are spoilt for choice when it comes to picking a restaurant to dine at. If we can take into account the biases of the user as a prior, we would be able to offer a better selection of restaurants to choose from. Additionally, a person usually goes to restaurants with friends who share similar culinary tastes. Incorporating the user's friends' tastes as additional priors will generate even better recommendations.

We provide a user with a novel and perhaps unusual simulated experience of going to a restaurant, giving a rating and review for the restaurant based on their liking. We chose to use OpenAI’s GPT-2 to generate reviews for restaurants based on the star rating: we generate positive reviews for 5-star ratings and negative reviews for 1-star ratings. For the purpose of this project, the 117M GPT-2 model was fine-tuned using 1,000,000 restaurant reviews using a batch-size of 512. To generate the star rating, we use a standard latent factor model and train the weight values using stochastic gradient descent in a supervised manner. The user's friends who have gone to the same restaurant are added as a separate set of weights.

Through this simulated experience, the user can now decide with greater certainty whether or not to visit a certain restaurant given the probable outcome of going there.

#### Contributors
Kalyani Jagdale @ https://github.com/kalyanijagdale<br>
Malarvizhi Vasudevan @ malar.v1905@gmail.com<br>
Monica Gupta @ https://github.com/monica1244<br>
Sahith Dambekodi @ https://github.com/SND96<br>
Tanvi Bhagwat @ https://www.linkedin.com/in/tanvibhagwat/<br>

#### Datset
Yelp Dataset hosted at: https://www.yelp.com/dataset

This repository is a copy of the original project hosted at the private repository: https://github.gatech.edu/mvasudevan7/ml-project.
