# HangMan
The Hangman game is a game of guessing. There are two players, where one decides on a word, and other one has to try the word by taking guesses as to what letters it contains. The game ends either when a maximum number of mistakes has been made, or when the player has found all the letters of the word.

An user chooses to be either the admin or the player. The person who acts as the admin does not have to do anything apart from choosing their role, as their device is merely used to run automatic checking on the player's guesses. The player actively, participates in the game by making guesses. The communication between the devices is made through SMS-messaging.

Steps followed:-

- The model, which handle the game mechanics, and takes care of encoding and decoding messages between the devices.
- The layout of the various activities: adding buttons, text fields, and listeners for each of them, and changing their colors and backgrounds.
- Message passing between two emulators or real devices to allow the admin and player to communicate, by using the Android class for broadcasts.

- Adding a database to keep record of categories and words with hints under each category. With sqlite created a database, and a helper class to aid in using the database.
- Making a contact picker for both admin and player so that each of them can select the number of the person they wish to play with.
- Adding options to allow the player to add new word in the database, and to notify the other player of changes in the database.
- Creating a database with all the numbers each device has already played with as an alternative to picking a number from the contacts. The database can store numbers multiple times but only returns them once.
- Finally, verifying the absence of bugs in the code and making minor modifications.
