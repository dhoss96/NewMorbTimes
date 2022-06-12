# New Morb Times!

As they say in the Oscar Winning movie "Morbius", its Morbin Time!


## The What

What this bot does is it reads in tweets from the New York Times on Twitter.
Then using natural language processing and changes the words to be "Morbed" 
and then replies to that tweet in question with the new "Morbed" tweet.

For example:

> No one knows for sure why dolphins are being spotted more frequently
> in and around New York Harbor. To better understand, scientists set up
> underwater microphones to track the feeding noises of the newly
> prevalent marine mammals.

Becomes: 

> No morbe morbs for sure why dolphins are being spotted more frequently
> in and around New York Harbor. To morbter understand, scientists morb
> up underwater microphones to track the feeding noises of the newly
> prevalent marine mammals.


## The How

This project uses the Natural Language Toolkit [NLTK](https://www.nltk.org/index.html) to best find out how to combine a word with 'Morbius'.

It accesses the Twitter API through [Tweepy](https://docs.tweepy.org/en/stable/) to grab tweets from the NYT twitter and reply to it with the "Morbed" tweet.



## The Why

Im going to level with you. The entire reason i did this project was because i heard the phrase "Its morbin time" and thought,
"Hey I could make a really bad joke about this and the New York Times" and then i spent the better part of a weekend learning Natural Language Processing to make this meme a reality.

## Usages

Although this entire project was based off of a bad joke, there is still quite a bit one could learn from this.
This project provides a good example of Natural Language Processing in an easy to understand way.

It also provides a good example of how to use Tweepy with the Twitter v2 API, as all of the documentation i found on Tweepy was either for the v1.1 API(which you cannot use for reading user tweets) or was missing required fields for calling the API.

A Major issue I ran into with Tweepy that was not documented anywhere I found on official tweepy docs, was that you **NEED** `user_auth=True` to be added to any client.getSomething calls for tweepy. Otherwise even if you provide the correct authentication, you will still get a '401 unauthorized'