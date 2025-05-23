# Assignment-3-Simple-Tweet-solution

Download Here: [Assignment 3: Simple Tweet solution](https://jarviscodinghub.com/assignment/assignment-3-simple-tweet-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Let’s make our own simple twitter…
A “tweet” is a special object that is the fundamental building block of Twitter.
If you are curious about the composition of a tweet you can familiarize yourself with the developer
pages available here:
https://developer.twitter.com/en/docs/tweets/data-dictionary/overview/tweet-object
You can see that the tweet is quite a complex object, which is why we would focus instead on a much
simpler version called “Simple Tweet”. It is a good start for us to create a simple twitter application.
A simple tweet will be composed of the following:
id int; which uniquely identifies the simple tweet
created_at char[51]; that would store the UTC time and date.
Note that UTC is the coordinated universal time, which is a common standard on the
Internet.
text char[141]; allow up to 140 characters.
user char[21]; the user name of the person who posted the tweet
You are asked to create a structure definition for a simple tweet called “tweet”. You will then need to
create a simple application with the following menu functionality:
1. Create a new tweet
2. Search tweets
3. Display tweets
4. Save tweets to file
5. Load tweets from file
6. Exit
When the user first starts the program he/she is prompted to enter his/her user name.
The menu is then displayed.
1. Create a new tweet
This option will automatically generate the next highest value for an id, the locate date/time for the
created_at in UTC, and prompt the user for the tweet’s text.
The new record is stored at the next available location in the array. If the array has reached capacity
then no new records may be added.
2. Search tweets
This option will search all tweets’ text for occurrences of a certain keyword string entered form the user.
It will search the text of each tweet, then display all the tweets that contained this keyword.
3. Display tweets
This option will display to the console screen all the tweets.
4. Save tweets to file
This option will save all the tweets to a file. The user is promoted for the filename. A simple status is
generated accounting to the number of records saved. Use a sequential text file.
5. Load tweets from file
This option will retrieve all the tweets stored in the file. The filename is provided by the user. The loaded
records will replace all existing records. Note that any new record added at this point will have to have
the next available id as per the new records (i.e. the next max value).
You will be graded as follows:
1. Struct definition setup [5pts]
2. Array setup in main to store the tweets up to MAX_TWEETS (do not use any global variables) [1
pts]
3. The user login [2 pts]
4. The main menu interactivity [2pts]
5. Each of the 5 menu items in a separate function [5 pts each = 25 pts]
6. Correct compilation, output (shown in the script file) [5 pts]
Refer to the script file attached with this assignment for reference on the output formatting and
examining a sample run. I am also providing the a.out file for sample runs and testing.
Total points: 40 pts
Submit your .c file, .txt (script) file, and the saved tweet file.
Sample steps to create the script file:
cp twitter.c twitter.bak
script tweets.txt
cat twitter.txt
cc twitter.c
./a.out
cat tweets.txt
exit


