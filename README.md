# Controlled-Chaos
Max4Live Euclidian Rhythm Generator

A polyrhythmic MIDI generator based on Euclidian mathematics. The intention is to create an arpeggiator-type device that allows users to generator new, expressive rhythms easily with just a few knob turns. Traditional Euclidian generators are often cumbersome and require fine-tuning dozens of parameters, which restricts their purpose to studio environments. By introducing elements of creative randomization, this device removes these challenges whilst still providing the full benefits of Euclidian-style Rhythms.

Video Demonstration Available Here:
https://www.julianlenz.com/controlledchaos

## Architecture

Euclidian Rhythms are broken down into 3 defining numbers:
Played Hits / Total Beats / Phase Offset
For example, a pattern of (4/16/1) would result in:
0 X 0 0 0 X 0 0 0 X 0 0 0 X 0 0 

The device's primary mode is polyphonic - each note played by the user will generate a different rhythm. For example, while holding C3 it plays (12/15/4), but when the user adds a G4 (whilst holding the first note) it could trigger at (9/17/2). 

## Controls
Density: The overall number of notes to be generated per sequence (i.e. a higher density may result in 14/16 notes triggering, whereas lower could yield 3/16)
Chaos: The similarity between each rhythm (only valid with Arpeggiator turned OFF). A value of 0 results in monophonic rhythm generation on all notes
Humanity: Adds slight delays and velocity randomization

Rhythm: The sub-division of beats. If set to 'sixteenth' then a Euclidian 'Total Beat' value of 9 results in 9 16ths.
Arp: When enabled, rhythm generation becomes monophonic. Instead of playing polyphonic patterns of multiple notes, it will instead randomly arpeggiate between the played notes within the singular rhythm. 
Note Reset: Will reset the rhythms to their starting position every time a new note is played. 
