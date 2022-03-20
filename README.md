# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Huy Khiem Nguyen

Time spent: 4 hours spent in total

Link to project: (https://glitch.com/edit/#!/fine-stump-speedwell)

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

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial (change color of the heading, add a strike counter)
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

    GIF1: General features
    
![General features](https://i.imgur.com/Yt156d5.gif)

    GIF2: Three-strike feature
    
![3 strikes](https://i.imgur.com/AP0FPIE.gif)

    GIF3: Speed it up
    
![Speed up](https://i.imgur.com/Doaf0rt.gif)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
    https://www.w3schools.com/js/js_output.asp

    https://www.w3schools.com/js/js_arrays.asp

    https://www.geeksforgeeks.org/difference-between-an-id-and-class-in-html/

    https://stackoverflow.com/questions/30035932/how-do-i-use-this-javascript-variable-in-html

    https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

    For me, the most challenging part of the project was the starting phase. Even though I knew some basic syntax in HTML, CSS, and JavaScript, I had not done any project in those languages before. Therefore, I felt overwhelmed by the project as everything was new to me. Then, I decided to take a small step at a time, and it turned out to be not so hard. In addition, the pre-work instruction broke big features of the project into small steps which really made it easier for me to follow. For example, the idea of making the computer to play clues for the user to repeat was a little tricky. I did not want all the clues to play at the same time, I also needed to keep track of what turn it was to play the proper clue sequence. With the help of the instruction, it became straightforward. To avoid the clues running together, I should use the built-in setTimeout function to delay the calling of the function that plays the next clue. So, the computer would wait for the current clue to finish plus some pause time, and then it would play the next clue. To keep track of the turn, I simply created a variable named progress which acted as an index into the pattern array, so, every time the user correctly guesses the sequence of that turn, the progress variable increases.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

    When I did JavaScript code for the project, I noticed that JavaScript is a dynamically typed language because I did not have to declare the variable with a data type. I learned in school that C++ is a statically typed language, therefore, I believe  C++ is faster than JavaScript as the computer does not need time to figure out what the data type is being used. I know this is a simple web development project, thus, it did not clearly show the advantages of JavaScript in web development, I still wonder if using C++ instead of JavaScript would make web development or at least in backend faster and more efficient.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

    Firstly, I would take a look at some lines of code in the sound synthesis functions that made me confused and search those codes to clearly understand what it did. Secondly, I would definitely add more features to the project. The idea of adding a ticking clock to limit the time the user has to make their guesses sound interesting. I think I would use the setInterval to call a countDown function every second, use clearInterval after the user correctly guesses the sequence of that turn, and call loseGame if the countDown function counts to 0.



## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.loom.com/share/befd53d15a054f3a86ab64d4f11441d9)


## License

    Copyright Huy Khiem Nguyen

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
