# Project 2 Readme Team Melvin

## 1. Team Name:
Melvin

## 2. Team members' names and netids:
Melvin Pineda Miguel - MPINEDAM

## 3. Overall project attempted, with sub-projects:
Program 2: K-Tape Turing Machine

## 4. Overall success of the project:
Successful or so I hope. My inputs generated were in-depth, my program analyzed them well. I was able to run it multiple times, see patterns, and I made a script to automate and save it all.

## 5. Approximately total time (in hours) to complete:
Didn't track it exactly but somewhere from 3.5-4 hours. The longest part was making the Turing Machine itself, but automating it with my run script took a lot longer than expected.

## 6. Link to GitHub repository:
[https://github.com/TAPMelvin/Project2](https://github.com/TAPMelvin/Project2)

## 7. List of included files:

| File/folder Name            | File Contents and Use |
| ----------------------------| --------------------- |
| **Code Files**              |                       |
| generateTMInput.py          | Generates random Turing Machine input data for simulation |
| simulateTuringMachine.py    | Runs the simulation on input data and writes the result to an output file |
| runTMSimulation.py          | Automates the entire process, assigns filenames, and manages file cleanup. Handles input/output naming for each run |
| **Test Files**              |                       |
| TMInputs.txt                | Initial input file created by generateTMInput.py |
| TMInputs1.txt               | Generated input file, used for the Turing machine simulation |
| TMInputs2.txt               | Generated input file, used for the Turing machine simulation |
| TMInputs3.txt               | Generated input file, used for the Turing machine simulation |
| TMInputs4.txt               | Generated input file, used for the Turing machine simulation |
| TMInputs5.txt               | Generated input file, used for the Turing machine simulation |
| **Output Files**            |                       |
| TMOutputs1.txt              | Output file for simulation results corresponding to TMInputs1.txt |
| TMOutputs2.txt              | Output file for simulation results corresponding to TMInputs2.txt |
| TMOutputs3.txt              | Output file for simulation results corresponding to TMInputs3.txt |
| TMOutputs4.txt              | Output file for simulation results corresponding to TMInputs4.txt |
| TMOutputs5.txt              | Output file for simulation results corresponding to TMInputs5.txt |

## 8. Programming languages used, and associated libraries:
- **Python**:
    - **Subprocess**: To execute scripts in the directory.
    - **Os**: Used for file existence checks and deleting files.
    - **Sys**: For argument parsing.

## 9. Key data structures:
- **Lists**: Store Turing Machine tapes and dynamically manipulate their symbols.
- **Dictionaries**: Map states and transitions for fast lookups.
- **Strings**: Represent input symbols, states, and transitions for parsing and formatting.
- **Integers**: Track tape head positions, step counts, and file sequence numbers.
- **File Objects**: Manage input/output data for persistent simulation records.

## 10. General operation of code:
- **generateTMInput.py**: Generates input data for the Turing machine.
- **simulateTuringMachine.py**: Parses inputs and generates simulation output.
- **runTMSimulation.py**: Automates both input generation and simulation, saves results with new filenames, and performs cleanup.

## 11. What test cases you used/added, why you used them, what did they tell you about the correctness of your code:
I used test cases with varying input sizes and edge cases, such as multiple tapes and transitions, to make sure that the Turing Machine simulator handled different configurations correctly. These test cases confirmed that the program can process many inputs (at least 250 at a time), follow transitions accurately, and properly handle both successful simulations and invalid transitions.

## 12. How you managed the code development:
I followed the structure I used for project one. First, I thought about what inputs would be needed and what I wanted them to look like. Then I wrote **generateTMInput.py**. Afterward, I focused on creating the actual Turing Machine, which took the longest. I made sure the logic was correct by referencing the textbook. Finally, I made everything run automatically, assigning file names and cleaning up unnecessary files.

## 13. Detailed discussion of results:
To determine the correctness of my program, I used a variety of test cases, including edge cases, typical inputs, and intentionally invalid configurations, to ensure all expected behaviors were handled properly. For example, I tested scenarios with minimal inputs, random sequences, and cases where no valid transitions could be found. By looking at the output traces in the simulation, I verified that states transitioned as expected and the correct messages, such as "Reached final state" or "No matching transition found," were printed for each input. The degree of nondeterminism varied across test cases, with some requiring multiple possible transitions at certain states, while others followed a single deterministic path. These traces confirmed the program’s ability to handle both deterministic and nondeterministic transitions while still producing consistent and accurate results as seen with the different input and outputs. If needed, **runTMSimulation.py** will produce more data.

## 14. How team was organized:
Solo

## 15. What you might do differently if you did the project again:
If I were to do the project again, I would improve the efficiency of the transition matching process by optimizing how transitions are searched and applied. Additionally, I would implement more detailed logging to track each step of the simulation for easier debugging and testing.

## 16. Any additional material:
None
