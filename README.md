# PIF Engine

This file contains the description and documentation of PIF, an open-source tool to write "physiological interactive fiction". Soon to be published at https://chi2020.acm.org/: Frey, J., Ostrin, G., Grabli, M., & Cauchard, J. R. (2020). Physiologically-Driven Storytelling: Concept and Software Tool. In CHI '20.

## Getting Started

Below are instructions for installing and deploying PIF

### Prerequisites

- Unity Version 2019.3.X or higher
- .NET Framework 4.5+

We also recommend installing the latest version of Visual Studios

### Installing

###### PIF.Unity

1) Download and install the latest version of Unity Hub
2) Clone the PIF.Unity, found at 
>https://github.com/PIF-engine/PIF.Unity.git
3) Add the cloned directory to your Projects manager in Unity Hub
4) Load the Project in Unity, wait for import to finish

###### PIF.Director

1) Clone the PIF.Director, found at 
>https://github.com/PIF-engine/PIF.Director.git
2) Open the Director solution in Visual Studios 2018+
3) Build the project
4) Move liblsl32.dll to the directory of the build project
   -NOTE: Director will hard crash if liblsl32.dll is not found. Should this occur, check to make sure the DLL is located in the correct location


## Testing the System

1) Run the PIF Unity engine inside the Unity Play Window, picking the FOVE Scene if you have a FOVE connected, or the PIF Camera scene if not
2) Run the Director and press Connect to Stream

If all works fine, the Director should be connected to the Unity Engine. The Unity engine will be sending samples to the Director. Press the Advance Story button to control the flow of the story in engine. Pressing the Send Var Update button will force any var to change its CurrentValue to the typed NewValue. Last Var Recieved displays the last variable based communication that the Unity Engine sent to the Director.
