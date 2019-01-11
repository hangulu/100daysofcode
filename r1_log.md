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

### R1D5: January 5, 2019

**Today's Progress**: Continued development on the popular meme application. Finished function to download all images from the timeline.

**Thoughts**: Got a full understanding of my mistakes from yesterday, the primary of which was following tutorials exactly without investigating what they were doing by double checking the documentation myself. After double checking and re-reading, I understand all the methods I'm using, and I'm in a great place to continue.

**Key Topics:**
* Twitter API
* wget

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Download Files With Python](https://stackabuse.com/download-files-with-python/)
3. [Mining Twitter Data With Python - Part 1](https://marcobonzanini.com/2015/03/02/mining-twitter-data-with-python-part-1/)

### R1D6: January 6, 2019

**Today's Progress**: Almost done with development of the popular meme application. Finished functions that pair the matching and comparing processes of OpenCV to the retrieval processes of Tweepy. Now, functions run the similarity function on all pairs of images downloaded from the timeline.

**Thoughts**: It felt good to complete this section because I required little help from the web (excluding two Stack Overflow checks for removing files with Python and an easier way to generate pairwise permutation). Almost done.

**Key Topics:**
* itertools

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)

### R1D7: January 7, 2019

**Today's Progress**: Done with development of the popular meme application. Running the main script analyzes the timeline, then reports a popular image (if there is one). If not, it reports that all the images are unique (which is a common occurrence when examining timelines of 100 tweets – further development should extend this by running it several times over the course of an hour or something).

**Thoughts**: It feels great to be done! I could continue with this (by making it run several times and looking at longer patterns), but I think I'm about ready to move on.

**Key Topics:**
* collections (Counter)

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)

### R1D8: January 8, 2019

**Today's Progress**: Decided to continue development of the popular meme script. The plan is to build a frontend for it, throw it up on the web, and allow users to see which of their memes they use the most. So far, I've added the ability to specify a user's profile, and I've lowered the threshold for similarity to 0.15.

**Thoughts**: I decided it's better to have a fully-functional product that I can share with the world than a MVP that I can use on my own. This pushes me to think about all stages in the development process, and forces me to build a more diverse skillset.

**Key Topics:**
* Python input
* sys.argv for command-line arguments

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)

### R1D9: January 9, 2019

**Today's Progress**: Worked on the frontend of the popmemes application, using React.

**Thoughts**: This is about my fifth time diving into React, so hopefully it sticks this time. Things are going smoothly so far.

**Key Topics:**
* React forms

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Creating Multistep Forms With React and Semantic UI](https://scotch.io/tutorials/creating-multistep-forms-with-react-and-semantic-ui)

### R1D10: January 10, 2019

**Today's Progress**: Worked on the Django backend of the popmemes application.

**Thoughts**: This is my first time working with Django, and it's much more involved and confusing than Flask. I'll definitely have to spend some time with it before I'm comfortable.

**Key Topics:**
* Django

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)

### R1D11: January 11, 2019

**Today's Progress**: Finished the Django backend of the popmemes application. Next step is to connect it to the React frontend.

**Thoughts**: Most of today was spent studying the basic concepts of backend work, including creating RESTful APIs, CORS, and examining good web development design (reading Steve Yegge's post gave a lot of insight). Now, I have a much better understanding of what the Django REST Framework seeks to do, and I'm very impressed.

**Key Topics:**
* RESTful (Representational State Transfer) API Design
* CORS (Cross-Origin Resource Sharing)

**Link(s) to work**:
1. [Most Popular Meme On The Timeline](https://github.com/hangulu/twitter/tree/master/popmemes)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [REST API Design](https://www.mulesoft.com/resources/api/what-is-rest-api-design)
4. [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
5. [Steve Yegge's Google Platforms Rant](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)
