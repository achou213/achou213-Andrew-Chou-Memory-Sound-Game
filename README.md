# Pre-work - *Memory Game*

"Andrew Chou's Memory and Sound Game" is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Andrew Chou

Time spent: 7.0 hours spent in total

Link to project: https://glitch.com/edit/#!/andrew-memory-game

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![X] http://g.recordit.co/9vJW3RsauE.gif (Full Video: https://recordit.co/9vJW3RsauE)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[- I used this app to learn about Math.random: https://developer.mozilla.org/en-US/docs/web/javascript/reference/global_objects/math/random ]  

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
[The project itself was a challenge for me because it was my first time working with Javascript. However, it was definitely a great way to be 
introduced to the coding language. Throughout the process, I was able to learn aspects and implementations of CSS script and HTML. While working 
on the function that allows the code to generate a new pattern during each commencement of the game, I encountered a slight problem with my for-loop. 
Occasionally, when I started my game, no buttons would play a sound nor light up; in other words, there were times when the newly generated pattern 
would provide a number for the playClueSequence() function that will cause it to return null. At first, I thought I made an error when initializing 
the new buttons, or that I needed to change the provided functions. However, to solve my error, I opened up the console terminal using inspect-element 
and ran the code to observe the processes while my code is running. To my surprise, I noticed that occasionally, my for-loop generated the number 0, 
which the ‘pattern’ array would then include in the list. This is a big error because no buttons were given the index of 0, only from numbers 1 to 6, 
and so, when the code generates a 0 in the pattern, the game does not know which button to play the frequency, and would therefore output a type-null 
error. To fix this, I looked more into the “Math.random” function, using the website provided for me, and changed my function from getRandomInteger() 
to getRandomIntInclusive(); afterwards, I changed the parameters within my new function from (0,7) to (1,6), since my code only contains 6 buttons. 
After this simple change, my code no longer pauses in between sessions, and the function - to generate a new pattern every start of the game - now 
works smoothly.
Additional challenges I encountered was when I attempted to tackle the “additional features” option. I was not able to decorate my buttons with 
images and change the playing sound to an mp3 file, since I do not know the functions of Javascript. While I did spend time researching, I ultimately 
was not able to code the CSS and HTML script correctly. This feature, along with other Javascript applications is something I greatly wish to learn and 
interact with more.]

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
[Upon finishing the assignment, I am even more intrigued in the field of web development and coding website applications. I wish to understand the myriad 
of features and uses of website making. 
The first question I have about web development is how to design a layout of my website where features are organized. Using Youtube.com as an example, 
how would I code my script file, CSS file, and HTML file, in which the search bar is on the top, pictures spread out evenly, and my subscribers on the 
very left? I want to understand more of the implementations of website development to enhance user experience and efficiency, as well as making it appealing 
to clients. 
Furthermore, how would I incorporate animations on my website? Many web pages utilize this function to make their site more organized and unique; they provide 
appealing animations to enhance the delivery of their message. For example, when you scroll through Apple.com, the transitions are very smooth and appealing. 
This not only captures users’ attention, but a good website design also demonstrates proficiency in your skills and the amount of effort you put in. I believe 
this function can be implemented in the CSS file, which is why I am very interested in learning more regarding this topic. 
The final question I have is how to properly utilize website APIs and which file  (index.html, script.js, style.css) would I incorporate the code in. APIs are 
an essential aspect of website building; it not only widens the uses of your website, but also allows users to communicate between other sites and retrieve 
necessary information for their own benefit. While I understand how to implement APIs using Python and C++, I am still unfamiliar with Javascript and wish to 
know more. ]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
[If I had additional hours and the necessary Javascript skills to work on the project, I would definitely spend them finishing the additional features, such as changing the buttons into pictures, replacing the 
buzzer sound with other sounds, as well as making a timer. Although I spent a number of time referencing online web sources, it was ultimately very difficult for me to incorporate them into my code; I believe 
this is an aspect of CSS I need to work on and learn more about. Also, I would spend this time understand more about the javascript library and what other features are available. 
Furthermore, while doing the “3-lives” additional feature, I tried to display the current number of lives on the page. However, I did not know how to display a changing variable, and so, I was not able to implement 
this function. When I looked up my inquiries, I didn’t understand how to change my script.html file where it displays a variable instead of just words. If I had more time and knowledge in Javascript, I would definitely 
able to design my website to my wanting and add additional design features that improve user experience. 
Lastly, to relate back to my interest in animations, I would definitely research how to enhance my website through the use of animations and graphic illustrations. Currently, my website is very bland and static; in order 
for users to continue using it, the design and features are very important. Therefore, I would spend my time trying to add small transitions or animations when a button is clicked, when you win, or when you lose. Even tho 
these are simple features, they add dynamic and color to the website as a whole. ]

## License

    Copyright Andrew Chou

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.