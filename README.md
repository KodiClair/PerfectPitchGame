# PerfectPitchGame
Circuit Playground Express game meant to test your perfect pitch.
The basic flow of the game is the CPX speaker plays a random note, asking the user for a matching response. By sifting through C4 major scale using the buttons, the user can tap the back of the board to make a selection.

/* 
A hand held video game that tests perfect pitch. Have the speaker play a random tone then have the person guess which tone it is.
Cycle through the options with the button to find the pitch. Get three wrong guesses. If all three attempts run out, restart.
To restart, ask in morse code 'try again: left- yes, right- no'. If no, break. Reset button has to be pushed to start from beginning.

Game Main:
- Select game mode
- start actions
- Start game
  - 3 single beeps
  - 3 other octive beeps
  - 3 double beeps
  - 1 triple beep with other octive
  - Cycle through the buttons, each time playing a tone. If you land on the right tone, click on both buttons then move to the next tone.
    The number of tones has to correlate to the number of beeps played. If you have selected the amount of beeps, it will automatically tell
    whether you got it right or wrong. Then, add green or red -> pause -> move to the next.
  - If lost:
    - play mario game over sound and ask to restart or not
  - If won:
    - End actions

*The pixels shift from green to purple/ dark blue given how far you make it

Select Game Mode
Can select between easy and hard mode
'Select Mode(switch): left - hard, right - east'

Start actions
At the start, give a start on what to do in morse code. 'Cycle buttons for correct note.' 
* Allow for skip option in the introduction if either button is pressed.

Easy
- Play tone -> play same tone -> flash green then add green counter on a neo pixel * Plays a nice quick beep when the counter is added
- Play tone -> play different tone -> flash red then add red counter on top of green counter.
- play same different tone two more times -> add two more reds
- Play mario game over sound track
- Pause -> count 3 times, flashing each time from red, yellow, green -> then start
Hard
- Play tone -> play same tone -> flash green then add green counter on a neo pixel * Plays a nice quick beep when the counter is added
- Play tone -> play different tone -> flash red -> Play mario game over sound track
- Play tone -> count down from ten -> red in all spaces -> Flash red -> Play mario game over sound track
- Pause then count 3 times then start

End Actions
10 rounds correlating to the number of neo pixels.
- Given that winning condition is satisfied for either mode, play medieval ceremony trumpet theme or universal studios
- Flash gold in a cool pattern: flash or sparkle
- Restart

*/
