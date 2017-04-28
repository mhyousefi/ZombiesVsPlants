# ZombiesVsPlants
A C++ game similar to the game Zombies vs Plants with limited options.

* Zombies are trying to pass accross yout backyard and enter the house (in order to eat your brain, I might add :))). The player can use plants to prevent that from happening.
* There are three types of plants: peashooter, sunflower, and walnut.
* Walnuts are pretty resistent when the zombies reach them while the others are easily eaten!
* There is only one regular type of zombie.

## Requirements
The two files rsdl.h and rsdl.cpp define the UI library used in this game. They use the SDL2 library to offer similar options such as displaying photos, drawing lines, and etc.
Therefore, you need to have the SDL library in your system. 

The /SDL2_Frameworks_Mac directory contains necassary files and info on adding the SDL library on MacOS.

For Linux, the following command can install the library:

    $ sudo apt-get install libsdl2-dev libsdl2-image-dev libsdl2-ttf-dev

## How to use it
Clone the project, move to the cloned directory and try the following commands:

For MacOS:

    $ g++ -o ZombiesVsPlants ZombiesVsPlants.cpp -F/Library/Frameworks rsdl.cpp -framework SDL2 -framework SDL2_image -framework SDL2_ttf
    $ ./ZombiesVsPlants
For Linux:

    $ g++ -o ZombiesVsPlants ZombiesVsPlants.cpp rsdl.cpp -l SDL2 -l SLD2_image -l SDL2_ttf
    $ ./ZombiesVsPlants
    
## Customization
There are two .txt files that specify the game conditions.

1) 1.level.txt: specifies the number of zombie waves, number of zombies per wave, and relative time per wave. 
The current level has three waves each having 3, 8, and 12 zombies with relative durations 4, 7, and 5.

2) savedata.txt: was aimed at saving player name and their current level, though this option was not developed. As of now, it has to be there, but the code will only read it once without taking it into account.

## Side Notes
* This is originally a college course project and I was required to write the code in a single file and avoid object-oriented programing.
* I hope to improve the source code in the future, adding multifile, OO principles, and perhaps new features.
* Anyone is welcomed to fork the project and improve it if interested.
