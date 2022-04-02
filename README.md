# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Kelly Henry

Time spent: **10** hours spent in total

Link to project: (https://glitch.com/edit/#!/righteous-probable-caraway?path=index.html%3A1%3A0)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

Start and Stop normal game

![](https://i.imgur.com/9xxwb0G.gif)

Start game and get incorrect choices 3 times

![](https://i.imgur.com/So0G1Lw.gif)

Win game 

![](https://i.imgur.com/KRNmguK.gif)



## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
- https://www.w3schools.com/
- https://www.geeksforgeeks.org

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

A challenged I encountered in creating this submission was adding more chances for the user. I knew I needed to create a global variable to count the mistakes made by the user but I had to figure out where to increase the variable and where to end the game. To overcome this challenge, before I wrote anything into my code I broke down what I needed so I could get an algorithm. First I needed to check if what the user clicked was correct( if(pattern[guessCounter] == btn)), if it was my global variable (mistake) is left alone. Else, the mistake variable was increased. This process should continue however before progress++ and playClueSequence() is called I needed to check if mistake = 4 before. If it did, then the loseGame() function is called and the game ends. After I figured out step by step what I needed to do, one at a time I implemented each step. First I made my variable and set it to false. When the game starts, it is set to true so the counter starts. From there I went into the guess() function so I could add my conditional statements to keep track of wrong guesses and end the game. The key to solving this problem was to break down what I had to do and know exactly what each function does so I could add features to the right place. In the end, I was able to figure it out and to ensure everything was correct and I printed the mistakes counter to the console so I could keep track of it. Whenever I have trouble, I figure out exactly what I need to do before I add anything to my code. 

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
 
After completing this submission some questions I have is what is the best way to organize all the functions in the javascript file. I was able to navigate through all the functions, but I couldn't help wonder if there was a way to improve the organization. In addition, I was wondering if any other coding languages could be used to increase the functionality of our webpage like JQuery so it would make the javascript file easier to read and more efficient. Lastly, a question I have after completing my submission is how can I make the program faster and more efficient. When I go on to make larger web pages with multiple files a key part is making everything fast but still functional. With web development, I would like to explore how to implement this within our web pages. 
 
4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a couple of more hours, I would add a couple of features to improve the user interface. The first thing I would add is a tracker on the game page so the user can keep track of how many lives they have. In addition, I would also add a progress bar so the user could know when the game was almost over and how far along they are. Also, if I had more time, I would have two buttons that say "Easy" and "Difficult." The easy version would have a basic pattern with only five buttons but the difficult version would implement a timer, additional buttons, and a longer song pattern. Lastly, after the game finishes, I would add a button that allows the user to give input on the game, so I can always improve the site. I would add a getElementById function in my javascript file so I could implement this feature. Overall, the changes I would add would work on improving the user interface and creating more options. While adding changes, however, I want to make the website simple and easy enough for the user to understand. 


## Interview Recording URL Link

[My 5-minute Interview Recording](https://drive.google.com/drive/folders/1Uz_iKonopCb_Vi8bwJxFSWM3ExoAonC6?usp=sharing)


## License

    Copyright [Kelly Henry]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
