# Tinder Autoliker 80%/20% likes/dislikes (customizable)
The script automatically likes 80% of the profiles and dislikes 20% at random intervals between 1 and 4 seconds (also customizable).

## How this code works
1. The script starts by defining two variables: "liking" which indicates whether the script is currently liking/disliking profiles, and "likingInterval" which will hold the identifier of the interval timer.

2. A function "getRandomDelay()" is defined which generates a random delay between 1 and 4 seconds (represented in milliseconds).

3. A function "likeOrDislike()" is defined. This function:
   - Fetches all buttons on the page.
   - Loops through these buttons to find the 'like' and 'dislike' buttons by their class names.
   - Randomly decides (with an 80% chance) to either 'like' or 'dislike' a profile by programmatically clicking the appropriate button.
   - Logs the action and the delay time to the console.

4. A function "controlLiking()" is defined. This function:
   - Checks if the script is currently liking/disliking profiles.
   - If it is, the function clears the interval timer to stop the liking/disliking process and updates the control button text to "♥ START".
   - If it isn't, the function sets up an interval timer to periodically (at random intervals between 1 and 4 seconds) 'like' or 'dislike' profiles and updates the control button text to "♥ STOP".

5. A control button is created with the initial text "♥ START", and given a fixed position in the top-right corner of the page.

6. Hover event listeners are added to the control button to change its background color when the mouse pointer is over it.

7. A click event listener is added to the control button to start or stop the liking/disliking process when the button is clicked.

8. A helper function "darkenColor()" is defined to darken a given color by a specified amount.

9. Finally, the control button is appended to the body of the page, making it visible and interactive for the user.

## To install this script, follow these steps:

1. Install the Tampermonkey extension for your browser. You can do this by visiting the official Tampermonkey website or the extension/add-on store for your browser and following the installation instructions.

2. Once Tampermonkey is installed, click on the Tampermonkey icon in your browser toolbar and select "Create a new script...".

3. In the script editor that opens, delete any pre-existing code.

4. Copy the provided Tinder Auto Liker script and paste it into the Tampermonkey script editor.

5. Click the "File" button, then click "Save" to save the script.

6. The script should now be installed and enabled. You can check this by clicking on the Tampermonkey icon in your browser toolbar and ensuring that the script is listed under "Enabled scripts".

7. Finally, visit https://tinder.com/app/recs. The script should automatically run on this page, and you should see the "♥ START" button in the top-right corner of the page.

Note: This script will only work when visiting the Tinder web application in a browser where the Tampermonkey extension is installed and enabled. Furthermore, it's important to be aware that the use of such scripts may violate the terms of service of the website and could result in your account being banned or suspended. Always use scripts responsibly and ethically.
