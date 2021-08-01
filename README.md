# Scrapbook Made Using Android Studio

This is an app that displayed a collage of three famous landmarks images found online and using text to label those images.

all XML codes were written in activity_main.xml source code. 
Next, a constraint layout was used to position and size any pictures or texts flexibly.

Since the goal is to build a collage, the layout was organized using the grid layout. 
The grid layout aligns the elements based on sequence columns and rows. 

Then, three buttons were created and placed in a row. 
The top and the middle buttons had a set boundary using the width of 360 dp and a height of 180 dp. 
However, the height of the last button was changed from 180 dp to 200 dp. 
The purpose of this alteration is to ensure the elimination of any blank spaces at the bottom.

Following the creation of buttons, each button was given the name 
"Golden Gate Bridge," "Statue of Liberty," and "Mount Rushmore" using the tag android:text. 
These will serve as the label for the images of the landmarks in the collage. 
The pictures for the collage were taken from pixabay and saved in a random file. 

Next, the app folder seen in the left column of the android studio was accessed. 
Among the multiple files saved under this folder, a file named "res" was also present. 
The file "res" had another folder named "drawable," 
which displayed an option named "Show in Explorer" when the file gets right-clicked with the cursor. 
When this option is selected, it will open a new window with multiple folders. 
Among them, a folder named "drawable" can be found. 
Here, all the pictures that were initially saved in a random file get copied. 

***It is important to note that these image file names were always saved with a small alphabet letter. 
Otherwise, it would cause an error when the application gets executed. 
Once done, these pictures are called into the xml code using the tag android:background. 
Each of these pictures is called using this tag under their respective buttons.***

However, once that was done, the button's background remained in its default color while displaying only the button's title. 

****This issue was fixed by accessing the "value" folder in the "app" folder. 
There, a folder named "theme" can be found. 
This folder had two XML files named "themes.xml" and "themes.xml (night)." 
In both of these xml files, the code "parent=" Theme.MaterialComponents….."> 
is changed to "parent=" Theme.AppCompat…..">. 
Once that was done, each button displayed the background image and the button's title without any problem.***

Lastly, for aesthetic purposes, the text of the titles of the corresponding buttons was manipulated. 
All the text was placed in the center of the button using the tag android:textAlignment = "center" and 
the color of the text were changed to andoid:textColor= "?android:attr/textColorTertiaryInverse." 
Furthermore, to ensure that the user can easily read the title, the font of the text was increased using the tag android:textSize= "48sp."
