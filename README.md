# 🎮 Higher or Lower — Followers Game

A simple Python command-line game where you compare two accounts and guess which one has **more followers**.

## 📌 About the Project

In this game, two accounts are displayed one at a time.

You have to choose:

* **1** → Account 1 has more followers
* **2** → Account 2 has more followers

If your answer is correct, your score increases by 1 and the game continues.

If your answer is wrong, the game ends and your final score is displayed.

---

## 🛠️ Technologies Used

* Python 3
* `random` module
* `os` module
* Custom Python modules:

  * `game_art.py`
  * `game_database.py`

---

## 📂 Project Structure

```text
Higher-Lower-Game/
│
├── main.py
├── game_art.py
├── game_database.py
└── README.md
```

### `main.py`

Contains the main game logic, including:

* Displaying account information
* Selecting random accounts
* Comparing follower counts
* Checking the player's answer
* Managing the score
* Clearing the console

### `game_art.py`

Contains the ASCII art used in the game, such as:

* Game logo
* VS symbol

### `game_database.py`

Contains the account information used by the game.

Each account contains information such as:

```python
{
    "name": "Example",
    "follower_count": 100,
    "description": "Example description",
    "country": "Example country"
}
```

---

## ▶️ How to Run

### 1. Install Python

Make sure Python 3 is installed on your computer.

Check your Python version:

```bash
python --version
```

### 2. Download or Clone the Project

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Move into the project folder:

```bash
cd Higher-Lower-Game
```

### 3. Run the Game

```bash
python main.py
```

---

## 🎮 How to Play

When the game starts, you will see two accounts:

```text
Compare 1: Account A
            VS
Compare 2: Account B

Who has more followers? 1 or 2:
```

Enter either:

```text
1
```

or

```text
2
```

### Correct Answer

If your answer is correct:

```text
You are right. Your score is: 1
```

The game continues with another comparison.

### Wrong Answer

If your answer is incorrect:

```text
You are wrong. Your final score is: 3
```

The game ends.

---

## 🧠 Main Functions

### `display_accountinfo()`

Displays the account's name, description, and country.

```python
def display_accountinfo(account):
    name = account["name"]
    description = account["description"]
    country = account["country"]
    return f"{name}, a {description}, from {country}"
```

### `check_answer()`

Checks whether the player's guess is correct by comparing the follower counts.

```python
def check_answer(guess, followers_count_1, followers_count_2):
    if followers_count_1 > followers_count_2:
        return guess == 1
    else:
        return guess == 2
```

---

## ✨ Features

* 🎲 Random account selection
* 👥 Account comparison
* 📊 Follower count comparison
* 🏆 Score tracking
* 🔄 Continuous gameplay
* 🖥️ Console screen clearing
* 🛑 Game ends when the player gives a wrong answer

---

## 🚀 Future Improvements

Possible improvements for this project:

* Add input validation
* Add difficulty levels
* Add a high-score system
* Add more accounts
* Add sound effects
* Add colored terminal output
* Add a replay option
* Create a graphical user interface (GUI)

---

## 📚 What I Learned

Through this project, I practiced:

* Python functions
* `if/else` conditions
* `while` loops
* Lists and dictionaries
* Random selection using `random.choice()`
* Importing custom Python modules
* Working with dictionaries
* User input
* Score tracking
* Basic project organization

---

## 👨‍💻 Author

**Sireesha Koramutla**

A Python learning project created to practice programming fundamentals and build a simple command-line game.
