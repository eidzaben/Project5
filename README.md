# Project5

## First Step, Organizing the GUI
The first thing I worked on for this project was setting up the GUI. I split the JFrame into two panels, the rightHalf and leftHalf. Then I split the leftHalf into 7 rows of panels. Each of those panels carried out a specific funtion.

## Second Step, Reading in the file
I created a class called readMeso that read in the Mesonet.txt file. I called the read method from this class and set the arrayList that it returned to a local arrayList. This arrayList contained all of the abbreviations, which I needed in order to do what the buttons were meant to do.

## Third Step, Creating the actionListeners
I used the lamda actionListeners for the buttons. Each button had its own actionListener.

### Calculate Hamming Distance Button
For this button I created an object of calcHdClass inside the actionListener. That class counted the frequency of each hamming distance, and returned each of them with a series of getters. The textFields that displayed the frequency of each hamming distance were assigned to the appropriate getters.

## UML 

