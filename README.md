# PerfectPitchGame
A game on the Circuit Playground Express Board that tests your pitch.

The basic rundown of this game is a random sequence generator that the player must match to progress forwards. By sifting through C4 major scale using the buttons(the player's range will stay the same through every stage), the user can tap the back of the board to make a selection. The tap only registers if the board is tapped twice in  succession(around a quarter to half a second apart) and with enough force otherwise the selection will not register and a small beep will not play. Each neo pixel on the CPX board correlates to a stage in the game. The player can either guess the correct sequence of notes which will award a green pixel or the wrong sequence which will award a red pixel. There are no redos for each stage. The difficulty of sequences will increase in the following order:
  - 3 single beeps with C4-B4 octive range
  - 3 single beeps with C3-B5 octive range
  - 3 double beeps with C4-B4 octive range
  - 1 triple beep with C3-B5 octive range
 In the case of multiple beeps in a stage, the player will have to make multiple note selections. To do this, the user has to sift through the notes and make a number of note selections corresponding to the given random note sequence played. Only after the required number of selections equals the number of beeps projected will the stage progress.
 
*It should be stated that a short beep will play after the player has tapped the board. This is merely an auditory tool used to signify that a selection has been made, not the random sequence of notes being played. Additionally, the CPX board is to be held in such a way that the micro usb port is facing north of the player. The left button will have the pin D4 marked above it and the right button, D5.

Game Timeline:
  The game starts off by flashing a morse code sequence saying: 'Select Mode: left - hard, right - easy'. The player can make a selection via the slide switch. 5 seconds will be given after the morse code sequence ends for the player to make their mode selection. If the player doesn't want to wait for the intro sequence to finish, either of the buttons on the CPX board can be pressed to skip which will transition immediately to the 5 second wait/ selection period. A starting sequence will commence after the selection has been made. Only after the neo pixels have flashed blue then green will the actual gameplay start. 
 - Easy mode gives the player two advantages, 3 lives before death and an unlimited amount of time to choose the sequences.
 - Hard mode gives the player 1 life before death and ten seconds per stage to make a selection. If the timer runs out, a life will be lost and the game will end.
  
  After the player makes it to the end, a winning sequence will commence followed by the end of the game. If the player loses all of the lives before reaching all 10 neo pixels, a gameover sequence will commence followed by the end of the game. If the player wants to try again, merely press the reset button on the CPX board. This will push the gameplay back to the introductory morse code sequence. All that's left to do is play the game!
 

