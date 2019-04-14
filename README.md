# Quizbot

## About

This is a bot for Discord which can run quizzes in your text channel. It uses the [Open Trivia DB API](https://opentdb.com/api_config.php) to gather questions based on user input and mediates the question and answer process in Discord. [Discord.py](https://github.com/Rapptz/discord.py) is used to interact with Discord.

## Usage

* `!quiz` - Broadcast bot instructions to the current text channel.
* `!quiz Categories` - Broadcast a list of categories to the current text channel.
* `!quiz <N> <Difficulty> <Category>` - Performs the main fetch of quiz questions then begins the process of quizzing in the current text channel.
    * `N` - Number of questions to fetch. N must be between 1 and 10 (inclusive).
    * `Difficulty` - Difficulty of questions to fetch. Difficulty must be one of 
        * `Easy`
        * `Medium`
        * `Hard`
        * `Any` - This returns questions from a mixture of difficulties
    * `Category` - Category of questions to fetch. Category must be one of the possible categories provided by the API, which can be found by typing `!quiz Categories`, or `Any` which returns questions from a mixture of categories 