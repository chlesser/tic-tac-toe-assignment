# Tic Tac Toe
This is an implementation of Tic Tac Toe for Graeme Devine's CMPM123 class. It is made with Dear ImGui, and written with C++ in visual studio code, on a windows machine.

## Implementation
This implementation was relatively straightforward, as Graeme had already taken care of the skeleton of the project. As such, I followed this skeleton as closely as I could.

### Methodology
Surprisingly, I hardly relied on any external tools for this project. Almost all of what I needed was already written in the classes (BitHolder, Square, Bit, Game), and that was the extent of my investigation. I disabled Github Copilot for a majority of this assignment, as it hallucinated and was generally unhelpful, but there were times I was writing code and hit tab to autocomplete a for loop or other trivial features.

### Challenges
I had one major code error: for some reason, when I was programming my OwnerAt function, I had the bright idea to use a BitHolder rather than a Bit. I suppose I did this in such a way that resulted in nondetection, and as a result I found myself hunting for the better part of an hour. This compounded with the fact that for some reason, my visual studio code was throwing errors with the debugger, and so I used the old fashioned way - couts.

## AI Implementation
### Unfinished
Originally I was planning on creating a selection screen, but in the process of debugging it got in the way of things. Sadly, I decided to ice those changes.

### Methodology
I went about this by rewatching the beginning of Graeme's lecture on yuja. I attended in person, but wanted to write the function myself. However, working with the functions like gameHasAI() were difficult, so I copied his introduction of minor tweaks around the class to properly setup. I also followed his example of copy pasting the wikipedia entry into code. From here, I largely programmed my own version of the software based on my understanding of the topics. Later, however, in the debugging process I ended up scrapping some of my code and referencing the video. This was foolish, as will be seen in that section.

#### Challenges
The hardest thing for me was wrangling the established functions to work well for me. Once I understood them, the algorithm flowed nicely. The massive bug I had was an error completely shutting down any semblance of AI activity. This was due to my earlier functions (checking for draw and winner) being copied and pasted, but without changing them from referencing the global state. I fixed this in the end, but not before slicing through a good deal of my code.