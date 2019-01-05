# #100DaysOfCode Log – Hakeem Angulu
## Round 1

The log of round 1 of my #100DaysOfCode challenge. Started on January 1, 2019.

## Log

### R1D1: January 1, 2019

**Today's Progress**: I started development on a Python application that takes the 100 most recent tweets on my timeline, and finds which memes are repeated the most (and thus, the most popular at the time).

**Thoughts**: It feels great to start something new and interesting. We all love memes, and I'd love to get a script out of this that can be run periodically to find out which memes are most popular at different times. It also gets me started on more AI work, with OpenCV and feature matching.

**Key Topics:**:
* Feature matching/AI with OpenCV

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Image Feature Extraction and Matching](https://www.kaggle.com/wesamelshamy/tutorial-image-feature-extraction-and-matching)

### R1D2: January 2, 2019

**Today's Progress**: Continued development on the popular meme application. Performed feature matching on two similar and different images. Next steps are to find a way to reject dissimilar images.

**Thoughts**: It definitely feels good to be getting somewhere with this, but I worry that I'm using blackbox tools. I should focus some more time on understanding the algorithms behind these tools.

**Key Topics:**:
* Feature matching/AI with OpenCV

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Image Feature Extraction and Matching](https://www.kaggle.com/wesamelshamy/tutorial-image-feature-extraction-and-matching)
3. [Similar Image Search With OpenCV](https://medium.com/machine-learning-world/feature-extraction-and-similar-image-search-with-opencv-for-newbies-3c59796bf774)

### R1D3: January 3, 2019

**Today's Progress**: Continued development on the popular meme application. Found a way to compare two images to each other: compare the number of matched key points with BFMatcher to the total number of key points in both images. Next step is to continue testing to find a good threshold for deciding if images are the same.

**Thoughts**: I've understood a lot more of the tools because I spent a good while reading through the documentation. It also feels nice to be so much closer to the goal of deciding similarity.

**Key Topics:**
* Feature matching/AI with OpenCV

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Feature Matching With OpenCV](http://answers.opencv.org/question/877/how-to-match-2-hog-for-object-detection/#882)

### R1D4: January 4, 2019

**Today's Progress**: Continued development on the popular meme application. Worked on using Tweepy to download images from the timeline, ending at the authentication step.

**Thoughts**: Tweepy seems like a good tool for the Twitter API, but there are a few aspects of the implementation that I should clarify in later days, like the class method.

**Key Topics:**
* Twitter API
* Class Methods

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Collecting Twitter Data With Python](https://galeascience.wordpress.com/2016/03/18/collecting-twitter-data-with-python/)
3. [Download the pictures from a Twitter feed using Python](https://miguelmalvarez.com/2015/03/03/download-the-pictures-from-a-twitter-feed-using-python/)
