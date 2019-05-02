# Project5

## First Step, Organizing the GUI
The first thing I worked on for this project was setting up the GUI. I split the JFrame into two panels, the rightHalf and leftHalf. Then I split the leftHalf into 7 rows of panels. Each of those panels carried out a specific funtion.

## Second Step, Reading in the file
I created a class called readMeso that read in the Mesonet.txt file. I called the read method from this class and set the arrayList that it returned to a local arrayList. This arrayList contained all of the abbreviations, which I needed in order to do what the buttons were meant to do.

## Third Step, Creating the actionListeners
I used the lamda actionListeners for the buttons. Each button had its own actionListener.

### Calculate Hamming Distance Button
For this button I created an object of calcHdClass inside the actionListener. That class counted each hamming distance and incremented the appropriate distance counter using a switch case. Then the class returned each of them with a series of getters. The textFields that displayed the frequency of each hamming distance were assigned to the appropriate getters.

### Show Stations Button
The show stations action listener created an object of the showStation class. Then it retrieved the the cities that matched the desired hamming distance and displayed them in a JTextArea. I added a scrolling feature to the JTextArea in order for it to display line by line.

### Add Station Button
This button first determines if the text in the textfield next to it is already part of the arrayList. If it's not, then that word is added to the arrayList and the JComboBox.

## Free zone
For the free zone I added feature that allows the user to type a character into a text field. Then when they click the button, the frequency of that letter in the list of city abbreviations is calculated. I calculated it by using an enhanced for loop to go through the cities, and then nesting another for loop to go through each of those characters. If any of those characters matches the given character, count is incremented. Finally the count is returned and displayed.

## UML 
![Project 5 UML](https://user-images.githubusercontent.com/47228130/57079944-10e88680-6cb7-11e9-89ca-e316d87ea126.png)
