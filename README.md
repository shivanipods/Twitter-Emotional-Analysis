# Emotional Analysis from Twitter Data

## Overview
This is supposed to be an application which would us determine the 48 granular emotions of a person. <More to come>

### Components of the *twitter* directory
1. _credentials_twitter.py: This file contains the various auth keys, etc. required to enable streaming the twitter data. (Majorly for execfile in Python terminal purposes)

2. _twitter_streaming.py: This is the file which is complete with auth values too and streams twitter feeds into the **twitter_data** file).

3. _twitter_data.txt: This is the raw twitter stream data, collected via the file 2.

4. _preprocess.py_: This file takes in the raw twitter stream and strips it clean to only store the respective Tweet ID, Text, Hashtags, and Location information into a structured csv file called **twitter_texts.csv**

5. _twitter_texts.csv: This is the output file from file 4 which has the respective Tweet ID, Text, Hastags, and Location information. It will later be fed into the LDA classifier algorithm to generate emotion topics.

6. _lda_train.py: This is the core working file for the LDA classifier and takes in the structred tweets to predict emotional topics. **I am still working on it**

7. _stopmild_: These are the stop words I stripped off the tweet data, to make it less noisy, these need to be rechecked for not removing negation words, which might be helpful in emotional analysis.  

### Results so Far
The LDA classifier gives very random results, a lot of the same is due to the extensive usage of punctuations etc in raw twitter data. Need to improve this more.

#### Disclaimer : All the file names in the code have been hardcoded to direct to my local file locations.
This needs to be fixed in the end, to maintain code ethics and make code more elegant. <TODO: Assign a variable for 'Users/pods/Documents/CMU/twitter/' in the code>
