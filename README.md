# InstaSPOT: **your next travel destination in an instant** :round_pushpin: #
### SOEN471 Winter 2022 Big Data Analytics Project by Team 8 ###

Name  | ID
------------- | -------------
Alvaro Tolosa  | 40020196
Chelsie Ng  | 40071692
Johnny On | 40137434
Misheelt Munkhjargal | 40196482

## Summary

<div align="justify">

  <h4> How can Instagram choose our next travel destination? </h4>
    <p> These days, social media has become a powerful tool that drives trends and popularity to a great extent. Instagram alone
    currently has over one billion active users. There is a great potential for increasing reach, popularity, and engagement
    by optimizing this market. Travel posts on Instagram allow users to discover new destinations worldwide through their
    stunning visuals and scenery. Which brings up the following research questions: How can Instagram choose our next travel 
    destination? Can we effectively recommend locations on Instagram based on user interests? Our goal is to leverage this market 
    by developing a tool that identifies main preferences based on user interests, empowering users to discover new and exciting 
    travel destinations. Our model will recommend new landmarks by extracting key features from a dataset of Instagram posts and 
    user input on preference and interest. </p>

  <h4> Dataset description </h4>
    <p> Our dataset comes from Proceedings of The Web Conference (WWW 20), ACM, 2020, provided by Seungbae Kim. This dataset
    classified influencers into nine categories related to beauty, family, fashion, fitness, food, interior, pet, travel,
    and others. This dataset contains 300 posts per influencer, so there are over 10 million Instagram posts where each
    influencer is categorized based on their post metadata. Each post metadata file is in JSON format and contains details
    like caption, user tags, hashtags, timestamp, sponsorship, likes, comments, etc. Given this massive amount of data,
    preprocessing was required to extract relevant information. Considering only the metadata of travel influencers, we came
    to around 70,000 post metadata. We also extracted pertinent fields such as post id, location name, location id,
    hashtags, number of likes, and the list of users who commented whether they liked the post or not. With these specific
    features, we can map whether a location is a hotspot or not. </p>

  <h4> Model Design & Algorithms </h4>
    <p> As such, users can find compelling travel destinations in a large corpus of posts using a recommendation system. A
    recommendation system can provide suggestions users might not have initially thought to look for themselves. We will
    recommend locations that cater to user interests through a content-based filtering approach. We will be using the
    Pearson correlation coefficient algorithm to recommend hotspots locations to users based on other similar spots the user
    has liked. We will also use the collaborative filtering approach to address and compare some of the limitations of
    content-based filtering by detecting similarities between users and travel destinations simultaneously. We will be using
    the Latent Factor algorithm with Stochastic gradient descent to optimize our recommendations. </p>

  <p> With such features, we wish to create a recommendation system for potential travel destinations to allow users to be
  exposed to information about a particular location as much as possible based on their interests. </p>
</div>
  
## Acknowledgements

- [Instagram Influencer Dataset](https://sites.google.com/site/sbkimcv/dataset)
