# Python Quiz Game
A simple python game built with python
## Table of contents
  - [Table of contents](#table-of-contents)
  - [Features](#features)
  - [Project Structure](#project-structure)
  - [Requirements](#requirements)
  - [Installation](#installation)
  - [Environment Setup](#environment-setup)
  - [Usage](#usage)
  - [Examole Output](#examole-output)
  - [Roadmap](#roadmap)
  - [Contributing](#contributing)
  - [License](#license)
  - [Author](#author)


## Features
- Quiz System
    - Asks the player multiple questions
    - Checks the answers automatically
    - Calculates the final score
- Result storage
    - Saves quiz results in `results.txt`
- Admin mode
    - Asks for the admin password
    - checks if the password is correct
    - Keeps the private information outside the main python file
    - Loads the password from `.env`

## Project Structure
```text
python-quiz-game/
│   main.py
│   question.py
│   requirements.txt
│   .env.example
│   .gitignor
│   README.md
```

### File description
- `main.py` - Main file used to run quiz game
- `question.py` - Stores questions and answers
- `requirements.txt` - lists the python packages needed for the project
- `.env.example` - Shows the environment variables needed by the projects
- `.gitignore` - Tells git which files and folders should not be tracked 
- `README.md` - contains the project documantion

## Requirements
Before running, make sure you have:

- `python3`
- `python-dotenv`

## Installation
1. open a terminal in the project folder.
2. check that python is installed.
```bash
python--version
```
3. install the python packages:
```bash
pip install -r requirements.txt
```

## Environment Setup
1. create a `.env` file from `env.example`:
```bash
cp .env.example .env
```
2. open the new `.env` file
3.  replace the example value with your own password
```text
QUIZ_ADMIN_PASSWORD = your_password_here
```
4. save the new file
> Do not commit your `.env` file because it may contain private information



## Usage
1. open a terminal in the project folder
2. run the quiz game 
 ```bash
python main.py
```
3. choose `yes` or `no` for admin mode 
4. if you choose `yes` or `no` , enter the password from your `.env` file
5. enter your name
6. answer the questions
7. see yor final score and messages
8. your result is saved in `result.txt`

## Examole Output
```text
do you want to open admin mode? yes/no: no

what is your name?alex
welcome

what language are we using?python
correct

what command starts a git?git init
correct

what command shows git status?git status
correct

your score is:  3 out of 3
excellent job alex
```

## Roadmap
- [x] add multiple quiz questions
- [x] calculate the final score
- [x] save results to a file
- [x] add admine mode
- [ ] add more quiz questions
- [ ] add difficultly questions
- [ ] add a timer

## Contributing

## License

## Author
create by [hamta](https://github.com/hamta-fallahyan)