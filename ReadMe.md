# Tic Tac Toe
This is an implementation of Tic Tac Toe for Grame Devine's CMPM123 class. It is made with Dear ImGui, and written with C++ in visual studio code, on a windows machine.

## Implementation
This implementation was relatively straightforward, as Grame had already taken care of the skeleton of the project. As such, I followed this skeleton as closely as I could.

### Methodology
Surprisingly, I hardly relied on any external tools for this project. Almost all of what I needed was already written in the classes (BitHolder, Square, Bit, Game), and that was the extent of my investigation. I disabled Github Copilot for a majority of this assignment, as it hallucinated and was generally unhelpful, but there were times I was writing code and hit tab to autocomplete a for loop or other trivial features.

### Challenges
I had one major code error: for some reason, when I was programming my OwnerAt function, I had the bright idea to use a BitHolder rather than a Bit. I suppose I did this in such a way that resulted in nondetection, and as a result I found myself hunting for the better part of an hour. This compounded with the fact that for some reason, my visual studio code was throwing errors with the debugger, and so I used the old fashioned way - couts.

## Extra
