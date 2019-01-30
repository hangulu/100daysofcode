# #100DaysOfCode Log – Hakeem Angulu
## Round 1

The log of round 1 of my #100DaysOfCode challenge. Started on January 1, 2019.

## Log

### R1D1: January 1, 2019

**Today's Progress**: I started development on a Python application that takes the 100 most recent tweets on my timeline, and finds which memes are repeated the most (and thus, the most popular at the time).

**Thoughts**: It feels great to start something new and interesting. We all love memes, and I'd love to get a script out of this that can be run periodically to find out which memes are most popular at different times. It also gets me started on more AI work, with OpenCV and feature matching.

**Key Topics:**:
* Feature matching/AI with OpenCV

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Image Feature Extraction and Matching](https://www.kaggle.com/wesamelshamy/tutorial-image-feature-extraction-and-matching)

### R1D2: January 2, 2019

**Today's Progress**: Continued development on the popular meme application. Performed feature matching on two similar and different images. Next steps are to find a way to reject dissimilar images.

**Thoughts**: It definitely feels good to be getting somewhere with this, but I worry that I'm using blackbox tools. I should focus some more time on understanding the algorithms behind these tools.

**Key Topics:**:
* Feature matching/AI with OpenCV

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Image Feature Extraction and Matching](https://www.kaggle.com/wesamelshamy/tutorial-image-feature-extraction-and-matching)
3. [Similar Image Search With OpenCV](https://medium.com/machine-learning-world/feature-extraction-and-similar-image-search-with-opencv-for-newbies-3c59796bf774)

### R1D3: January 3, 2019

**Today's Progress**: Continued development on the popular meme application. Found a way to compare two images to each other: compare the number of matched key points with BFMatcher to the total number of key points in both images. Next step is to continue testing to find a good threshold for deciding if images are the same.

**Thoughts**: I've understood a lot more of the tools because I spent a good while reading through the documentation. It also feels nice to be so much closer to the goal of deciding similarity.

**Key Topics:**
* Feature matching/AI with OpenCV

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Feature Matching With OpenCV](http://answers.opencv.org/question/877/how-to-match-2-hog-for-object-detection/#882)

### R1D4: January 4, 2019

**Today's Progress**: Continued development on the popular meme application. Worked on using Tweepy to download images from the timeline, ending at the authentication step.

**Thoughts**: Tweepy seems like a good tool for the Twitter API, but there are a few aspects of the implementation that I should clarify in later days, like the class method.

**Key Topics:**
* Twitter API
* Class Methods

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Collecting Twitter Data With Python](https://galeascience.wordpress.com/2016/03/18/collecting-twitter-data-with-python/)
3. [Download the pictures from a Twitter feed using Python](https://miguelmalvarez.com/2015/03/03/download-the-pictures-from-a-twitter-feed-using-python/)

### R1D5: January 5, 2019

**Today's Progress**: Continued development on the popular meme application. Finished function to download all images from the timeline.

**Thoughts**: Got a full understanding of my mistakes from yesterday, the primary of which was following tutorials exactly without investigating what they were doing by double checking the documentation myself. After double checking and re-reading, I understand all the methods I'm using, and I'm in a great place to continue.

**Key Topics:**
* Twitter API
* wget

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Download Files With Python](https://stackabuse.com/download-files-with-python/)
3. [Mining Twitter Data With Python - Part 1](https://marcobonzanini.com/2015/03/02/mining-twitter-data-with-python-part-1/)

### R1D6: January 6, 2019

**Today's Progress**: Almost done with development of the popular meme application. Finished functions that pair the matching and comparing processes of OpenCV to the retrieval processes of Tweepy. Now, functions run the similarity function on all pairs of images downloaded from the timeline.

**Thoughts**: It felt good to complete this section because I required little help from the web (excluding two Stack Overflow checks for removing files with Python and an easier way to generate pairwise permutation). Almost done.

**Key Topics:**
* itertools

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)

### R1D7: January 7, 2019

**Today's Progress**: Done with development of the popular meme application. Running the main script analyzes the timeline, then reports a popular image (if there is one). If not, it reports that all the images are unique (which is a common occurrence when examining timelines of 100 tweets – further development should extend this by running it several times over the course of an hour or something).

**Thoughts**: It feels great to be done! I could continue with this (by making it run several times and looking at longer patterns), but I think I'm about ready to move on.

**Key Topics:**
* collections (Counter)

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)

### R1D8: January 8, 2019

**Today's Progress**: Decided to continue development of the popular meme script. The plan is to build a frontend for it, throw it up on the web, and allow users to see which of their memes they use the most. So far, I've added the ability to specify a user's profile, and I've lowered the threshold for similarity to 0.15.

**Thoughts**: I decided it's better to have a fully-functional product that I can share with the world than a MVP that I can use on my own. This pushes me to think about all stages in the development process, and forces me to build a more diverse skillset.

**Key Topics:**
* Python input
* sys.argv for command-line arguments

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)

### R1D9: January 9, 2019

**Today's Progress**: Worked on the frontend of the popmemes application, using React.

**Thoughts**: This is about my fifth time diving into React, so hopefully it sticks this time. Things are going smoothly so far.

**Key Topics:**
* React forms

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Creating Multistep Forms With React and Semantic UI](https://scotch.io/tutorials/creating-multistep-forms-with-react-and-semantic-ui)

### R1D10: January 10, 2019

**Today's Progress**: Worked on the Django backend of the popmemes application.

**Thoughts**: This is my first time working with Django, and it's much more involved and confusing than Flask. I'll definitely have to spend some time with it before I'm comfortable.

**Key Topics:**
* Django

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)

### R1D11: January 11, 2019

**Today's Progress**: Finished the Django backend of the popmemes application. Next step is to connect it to the React frontend.

**Thoughts**: Most of today was spent studying the basic concepts of backend work, including creating RESTful APIs, CORS, and examining good web development design (reading Steve Yegge's post gave a lot of insight). Now, I have a much better understanding of what the Django REST Framework seeks to do, and I'm very impressed.

**Key Topics:**
* RESTful (Representational State Transfer) API Design
* CORS (Cross-Origin Resource Sharing)

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [REST API Design](https://www.mulesoft.com/resources/api/what-is-rest-api-design)
4. [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)
5. [Steve Yegge's Google Platforms Rant](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)

### R1D12: January 12, 2019

**Today's Progress**: Worked on connecting the Django backend to the React frontend. Took a break from the coding to learn about decorators and Python's syntactic sugar in depth.

**Thoughts**: Today was mostly spent understanding core concepts of Python that I had used before, but hadn't fully understood, mostly notably: decorators. I loved being able to dive into the language of the authors of Python through PEPs, understanding most of what they expressed.

**Key Topics:**
* Decorators
* Syntactic Sugar

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [PEP 318: Decorators for Functions and Methods](https://www.python.org/dev/peps/pep-0318/#background)
4. [Primer on Python Decorators](https://realpython.com/primer-on-python-decorators/)
5. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)

### R1D13: January 13, 2019

**Today's Progress**: Worked on connecting the Django backend to the React frontend. Not much progress made in actually finishing the app; the Django REST Framework has gotten a little confusing as I try to veer away from tutorials.

**Thoughts**: Today was a bit frustrating as I delve deeper into the Django weeds - it makes me miss Flask. However, I'm confident that tomorrow will be good for solidifying some of the confusing  concepts (ViewSets and Routers).

**Key Topics:**
* DRF ViewSets
* DRF Routers

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)
4. [Importing Modules From Parent Folder](https://stackoverflow.com/questions/714063/importing-modules-from-parent-folder)
5. [ViewSets in DRF](https://www.django-rest-framework.org/api-guide/viewsets/)
6. [Routers in DRF](https://www.django-rest-framework.org/api-guide/routers/)

### R1D14: January 14, 2019

**Today's Progress**: Fixed many errors that I was encountering after changing the database schema and deviating from tutorials. The main issue is that not all the information stored in the database is submitted through the form.

**Thoughts**: I am now understanding DRF more fully, and I can feel myself becoming more comfortable sorting through the errors. I feel closer to the finish line.

**Key Topics:**
* Axios
* MVC

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)
4. [Axios](https://www.npmjs.com/package/axios)
5. [MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)

### R1D15: January 15, 2019

**Today's Progress**: Worked more on the logic of the rendering in JavaScript.  A few errors relating to the importing of my own modules are arising, however.

**Thoughts**: I'm learning a lot of JS (the hard way), which is exciting. I have a better understanding of 'this', functions, and promise chaining. I'm worried about a few errors I'm encountering, but I'm optimistic.

**Key Topics:**
* Promise Chaining
* MVC

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Build A Todo Application Using Django and React](https://scotch.io/tutorials/build-a-to-do-application-using-django-and-react)
3. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)
4. [Promise Chaining](https://javascript.info/promise-chaining)
5. [Understanding the “this” Keyword in JavaScript](https://medium.com/quick-code/understanding-the-this-keyword-in-javascript-cb76d4c7c5e8)

### R1D16: January 16, 2019

**Today's Progress**: Worked out most of the errors that I was worried about, but now encountering errors when posting to the API. Almost finished though.

**Thoughts**: A little frustrated that I'm not finished yet, but I'm confident that I will be soon, and I'm learning a lot on the way.

**Key Topics:**
* Alerts

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)

### R1D17: January 17, 2019

**Today's Progress**: Identified the cause of another error: relative file paths in the matcher function. Worked this out, but limited by the Twitter API.

**Thoughts**: The Twitter API's rate limiting is a major bottleneck of both the development process and production. It seems as if we can only make meaningful requests once every 15 minutes, which is frustrating. Looking forward to finishing this and moving on.

**Key Topics:**
* Rate Limiting

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)

### R1D18: January 18, 2019

**Today's Progress**: Worked some more on using axios to connect the backend to the frontend by adding a file specifically for axios functions. Also changed from class-based views to function-based views.

**Thoughts**: Feeling a bit slow, but I hope the project will be done soon. Regardless, the important thing is that I'm learning a lot, and in the best way that one can learn: by trying out different things myself.

**Key Topics:**
* Class-Based Views vs. Function-Based Views
* Axios

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)
3. [Class-Based Views vs. Function-Based Views](https://simpleisbetterthancomplex.com/article/2017/03/21/class-based-views-vs-function-based-views.html)

### R1D19: January 19, 2019

**Today's Progress**: The API is now working flawlessly for all GET requests (both full lists of users and details for individuals). It was broken a bit  after switching from class-based to function-based views. Now, all is more  seamless, and I'm ready to move on to focusing on POST requests and the frontend. Also fixed a lot in the JavaScript, with a focus on the Form component and the ImageServices file for Axios.

**Thoughts**: Got a lot accomplished today, so I'm feeling good. Inching closer to the finish line. I decided to focus on ensuring that the product works well and I understand every bit of it, no matter how long it takes me.

**Key Topics:**
* Axios

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)

### R1D20: January 20, 2019

**Today's Progress**: Worked some more on the API and the frontend. POSTing now works fully with the frontend, but GETting is proving difficult.

**Thoughts**: Got a lot accomplished today, so I'm feeling good. Inching closer to the finish line. I decided to focus on ensuring that the product works well and I understand every bit of it, no matter how long it takes me. Got some more concrete work done, and I now understand more about HTTP requests.

**Key Topics:**
* HTTP Requests

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)

### R1D21: January 21, 2019

**Today's Progress**: Both POSTing and GETting now work seamlessly with the frontend. The project is basically finished, and now returns alerts with the correct information (the username, the most popular image, and the frequency of that image). The last step is to display the image and run tests.

**Thoughts**: Basically finished, and I'm feeling excellent. The app is looking good and is working well. Most importantly, I have a much stronger grasp of JavaScript and React than when I started.

**Key Topics:**
* Template Literals
* Binding
* Conditional Rendering
* Component Data Storage

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [How to build a modern web application...with Django and React](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04)
3. [Template Literals in JS](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)
4. [Binding in JS](https://alistapart.com/article/getoutbindingsituations)
5. [Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)
6. [Where To Hold React Component Data](https://medium.freecodecamp.org/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00)

### R1D22: January 22, 2019

**Today's Progress**: Finished with the popular image application. I've separated the repository into its own, cleaned up the directory, and tested it (as much as I could given the Twitter API rate limiting).

**Thoughts**: It feels so good to be finished! There were many obstacles, but I pushed through. Now, I have a much stronger understanding of React, JavaScript, and OpenCV than I did before I started.

**Key Topics:**
* Component Data Storage

**Links to work and references**:
1. [Most Popular Image On The Timeline](https://github.com/hangulu/popimg)
2. [Where To Hold React Component Data](https://medium.freecodecamp.org/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00)

### R1D23: January 23, 2019

**Today's Progress**: My next application will be a Java backend that allows one to post a new tweet to an existing thread. Today, I installed Java on my system, and started a few tutorials to remind myself what coding in Java is like.

**Thoughts**: I'm glad that I'm getting started on something new. I'll be coding in Java all summer, so I think I'll dedicate at least my next two projects to really learning that language, and the thread thing is an excellent start (because I'll be using it every day for this).

**Key Topics:**
* Java

**Links to work and references**:
1. [Java Tutorial](https://www.tutorialspoint.com/java/java_overview.htm)
2. [Learn Java in One Day and Learn It Well](https://www.amazon.com/Java-Beginners-Hands-Project-Project-ebook/dp/B01LZOCVN9/ref=sr_1_3?s=books&ie=UTF8&qid=1548245450&sr=1-3)
3. [Effective Java](https://www.amazon.com/Effective-Java-Joshua-Bloch/dp/0134685997)

### R1D23: January 24, 2019

**Today's Progress**: Finished chapters 1-2 of *Learn Java in One Day and Learn It Well.*

**Thoughts**: A little slower than previous days, but it feels good to dive back into the syntax of Java.

**Key Topics:**
* Packages
* Comments
* The main() method

**Links to work and references**:
1. [Learn Java in One Day and Learn It Well](https://www.amazon.com/Java-Beginners-Hands-Project-Project-ebook/dp/B01LZOCVN9/ref=sr_1_3?s=books&ie=UTF8&qid=1548245450&sr=1-3)
