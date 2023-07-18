# Readme.md
Hockey Team Check-In App

The Hockey Team Check-in App is a simple web application that allows players to check-in or check-out for games. Players can enter their names and indicate their attendance status for each game. The app uses HTML, CSS, and JavaScript to create an interactive and user-friendly interface.


Features:

Players can check-in for games by entering their names and clicking the "Check-in" button.
Players can check-out by unchecking the checkboxes next to their names.
The app dynamically updates the player list to reflect real-time check-in and check-out status.
Player data is saved to local storage, ensuring that the check-in status persists even if the page is reloaded.


How to Use:

Clone or download this repository to your local machine.
Open the index.html file in your web browser.
Enter your name in the input field and click the "Check-in" button to check-in for a game.
To check-out, uncheck the checkbox next to your name.
Player data is automatically saved to local storage.


Functions Explanation:

saveToLocalStorage(): This function is responsible for saving the player data to local storage. It is called whenever a player checks-in or checks-out for a game to persist their attendance status.

checkInPlayer(event): This function handles the form submission when a player wants to check-in for a game. It extracts the player name from the input field and checks if the player is already in the player list. If the player exists, it toggles their attendance status (check-in/check-out). If the player is not in the list, it adds a new player with the check-in status. The form input is then cleared, and the player list is updated to reflect the changes.

updatePlayerList(): This function updates the player list displayed on the web page. It dynamically generates HTML elements for each player in the players array and displays them as a list with checkboxes next to each player's name.

toggleAttendance(name): This function is called when a player's attendance status is toggled using the checkbox. It finds the player in the players array based on the provided name and toggles their attendance status (check-in/check-out). The updated player list is then saved to local storage.

playerForm.addEventListener('submit', checkInPlayer): This line of code adds an event listener to the player form. It listens for form submissions (when the "Check-in" button is clicked), and when triggered, it calls the checkInPlayer function to handle the check-in process.


Technologies Used:

HTML
CSS
JavaScript
