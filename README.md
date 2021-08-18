# cli-typetest

## Ultimate Goals:

CLI application that tests your typing speed. 
* Can play solo, where you can practice with several options of passages OR race against the clock to type as many random words as possible. 
* Can play multiplayer in a lobby of other players, where everyone's progress is updated realtime and displayed in the terminal (similar to the cars in typeracer)
* Large emphasis on stats, with ability to create a profile OR opt in/out of recording runs
  * Important for when another user wants to try on the same machine

## Solo:
* Create a fancy ascii box
* Highlight the reference text in real time
* Have option to have different settings as parameters
  * Words/chars displayed per line &ndash; `-w, words`
  * Time the player has to type as many words as possible: &ndash; `-t, -time`
  * Length of passages &ndash; `-p, --passage`
    * Short/Medium/Long
    * `-pl, --passagelowercase` for lowercase passages only 
  * Type code &ndash; `-c, --code`
      * Python, JS, Java, C++, C#, C, or Any (from the list)
* Other flags:
  * `-h, --help` &ndash; Show help
  * `-V, --verbose` &ndash; Show settings on start
  * `-i, --input` &ndash; Path to a wordlist file with new line separated words OR new passage

## Multiplayer:
**Will worry about this at a later time**

## Stats:
* Stats at the end of a run:
  * WPM
  * Total keystrokes
  * Correct keystrokes
  * Wrong keystrokes
  * Accuracy
* Simple file to keep track of runs
  * Only for default game (random words)
  * Show averages for most recent 10/25/100 runs
  * Keep running totals of keystrokes (correct, incorrect, total)
  * Keep a PB for WPM

## TODO:
* Create a basic typetest with:
  * ~~Have top 1000 most common words in a text file~~
  * A **good-enough** ascii box
  * Real-time highlighting of reference text
  * Have an end screen that calculates all of the stats