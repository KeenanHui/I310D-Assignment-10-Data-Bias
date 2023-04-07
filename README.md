# I310D-Assignment-10-Data-Bias
Finding bias in Perspective API
This assignment for I310D Introduction to Human Centered Data Science had us looking for bias in the Perspective API toxicity value.

Were were to come up with a hypothesis which, for this assignment, is that the API will have a harder time trying to accurately tell if shorter comments (50 and under words) are toxic compared to longer comments (over 50 words).

Throughout the process, there were some issues with using the API. The most common one was that the API would have a hard time automatically telling what language some text was. The workaround that was implimented was to use try and except (although there must be a better way) to pass any case where the sentence language was not properly found.

My original hypothesis was that Perspective API would have a harder time trying to accurately tell if shorter comments are toxic compared to longer comments. However, after doing analysys, it seems as if that is not the case, and the API has a harder time with comments that are over 50 words in length. The results found that the API accuracy compared was at 70% for comments over 50 words that humans considered toxic and 80% for comments over 50 words that humans considered non-toxic.

I think that there is definitely bias in the API. Personally, I beleive that the API may not be able to put into context the toxic words, and instead puts a toxicity weight to certain words, so comments which have the word will be more likely to be considered toxic (given the threshold of 0.5).

Another reason for bias may also be the smaller sample size used in this test. The larger the sample size, the more accurate the test cases will be.
As I am not compleatly aware of how this model works and am just making an assumption from what the facts I can see, I am curious how this API words. Is it just putting a weight on specific words and finding the toxicity level based on that, or does it take into consideration the context and to what extent it takes context into consideration.
