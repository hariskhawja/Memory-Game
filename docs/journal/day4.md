# Journal - Day 4
Date: Thursday, December 1, 2022

- Aritro, Byron, and Haris were able to resolve all programming and wiring errors related to the memory game circuitry
- Although the game did work, it became apparent that the 75HC595 was very buggy and was adament in oftentimes failing to supply power to the 7 segment display
- The 75HC595 was also consistent in failing to present the correct levels within the game
- More wire stripping was taken place as majority of all voltage and ground wires had been completed
- Though in theory the game was working (TinkerCAD), the physical circuit built was inconsistent due to the 75HC595 IC, thus a collaborative reflection took place to determine the team's direction or next steps with the project:
    - One such option was to attempt to refine the 75HC595 and reduce failures
    - Another option was to utilize the Arduino's other I/O pins, since there was enough to power each segment of the 7 segment display
    - Finally, the third option was to utilize another more powerful integrated circuit: the CD4511 or the 7 segment decoder
- Aritro, Byron, and Haris selected the third option since it seemed to significantly increases chances of success of the project
- The team began to research and implement the CD4511 into the circuit

## Pictures of TinkerCAD Circuitry with CD4511
![tinkerCAD circuit](/media/diagrams/tDay4.jpg)

## Video of the Nearly Completed Physical Circuitry


## What is a 7 segment decoder?
The 7 segment decoder is an integrated circuit who's purpose is to use certain binary patterns to encode decimal values from 0-9 with 4-bits. Similar to the shift register, the 7 segment decoder drastically reduces the number of I/O pins used by the Arduino to control the 7 segment display. In simple terms, to reflect the correct numerical values, this IC records each segment of the display with an encoding digit on each of its pins. 

The IC has 16 pins in total: 4 of which are used as input pins and 7 used as output pins (for each corresponding segment of the display). This 7:4 ratio in terms of I/O pins reveals its ability to enhance circuit performance by reducing total tools used to complete a given task.

![source](https://www.javatpoint.com/bcd-to-seven-segment-decoder)