Random Image Display Using PHP (RIDUP)


HOW TO USE:
•	Simply extract the zip file to a location in your web server (local used here).
•	Then reference the ‘index.php’ file from the browser.
•	Reloading the webpage also reloads with a new image stored in the image folder.

WHY IT WORKS
This script uses the either of two php randomization functions to create random image display effect after every page reload. 

SOME HTML AND CSS:
The index.php is the RIDUP template - of some sort. Ironically it only contains a single line of php code (that does the main work) embedded in html. Some simple/basic CSS (in the “style.css” file) were used to create a visually appealing interface.

The image to be randomly displayed are stored in an “images” folder/directory where each they are saved serially starting with an integer value (that would be used as the ‘min’ value in the mt_rand() function) and the terminating integer value which is used as the ‘max’ value in mt_rand(). In this RIDUP script, six images were named 1.png, 2.png, 3.png, 4.png, 5.png,6.png.

The mt_rand() function is place in the image (<img>) reference line. Since the images were saved using integer filenames, the function can randomize the filename that are them displayed based on the returned value. 

This can also be done using the php rand() function. Both functions are used in php to generate a random integer in the specified range. Both functions use the same syntax:

rand(min, max) or mt_rand(min, max)
Where min is the lowest value to return and max is the highest value to return.

To generate a random number between 1 and 6 (inclusive), for example, use mt_rand(1, 6) or rand(1, 6).

I used the mt_rand() function in RIDUP because the php documentation states that the mt_rand() function is faster than the rand function. Backward compatibility have been solved (in PHP 7.1.0) by making rand() an alias of mt_rand().

COPYRIGHT: The text and images were all imported from the research of: Singh, B and Ryan, J (2015) Managing Fertilizers to Enhance Soil Health. International Fertilizer-Industry Association (IFA), Paris, France.

	USE. IMPROVE. SHARE.
