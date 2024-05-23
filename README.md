**RAYTRACER PROJECT**

This was a project created in my fourth semester as part of a Computer Graphics Project. It needs to be run on a specific docker image to function correctly.

Use the docker image found in the following link, and follow the instructions: 
https://github.com/tiperiu/COMP371_dockerimage

Here's what you have to do:
- Clone the this repository
- Clone the docker image
- Start up docker
- go in a command line, navigate to the folder for the docker image and type ./windows/interactive_run.ps1 "*Path to raytracer here*"
- Now that you are in the docker container, navigate to the build folder of the raytracer (./code/build)
- Once in the folder, you can parse a json file by running the raytracer as such: ./raytracer *insert path of the json file name here*
- The json files are normally located in the assets folder.

These are the instructions in order to run the raytracer provided by my professor (credits to Tiberiu Popa) (you can also find this in the code folder):
"
This code is used for three purposes:

1) Build the official course solution
2) Build the student solution 
3) Build a dummy application that showcases some of the codebase.

Each build is controlled by two defines:
COURSE_SOLUTION and STUDENT_SOLUTION.

If none of these variables are defined the dummy code is built. This is the default behaviour.
If COURSE_SOLUTION is defined, the code expects the course solution (this should never be defined)
IF STUDENT_SOLUTION is defined the code expects a student solution is implemented in the src folder. Have a look at the main.cpp file for the expected interface.

You can switch on and off these defines in the CMakeLists.txt file. 


Building the dummy test

1) Create build folder: mkdir build
2) cd build
3) cmake ../
4) make
5) ./raytracer

Building the solution:
1) Uncomment the #add_compile_options(-DSTUDENT_SOLUTION) line in the CMakeLists.txt 
2) Create build folder: mkdir build
3) Create the src folder: mkdir src
3) cd build
3) cmake ../
4) make
5) ./raytracer <filename.json>


Note that some test scenes are provided in the assets folder. You can do a soft link to the assets folder in the build folder for your convenience.
"


