# Taskaty

A simple command line interface app for task management.

## Installation

* Clone this repository then run:

* Create a virtual environment:

```
python -m venv venv
```

Or

```
python3 -m venv venv
```

If you are on Ubuntu, make sure that `python3-venv` is installed:

```
sudo apt install python3-venv
```  

* Ativate the virtual environment:

- On Windows:

```
venv\Scripts\activate
```
- On Linux and macos:

```
source venv/bin/activate
```

* Run the following command to install the app:
```
pip install -e .
```

You will be able to run the app from the command line or terminal using the `taskaty` command.

## Usage

### Add a task
To add a task use the option `add`.

```
taskaty add "Add search bar compoent to the UI"
```

`add` option has the following optional arguments. :

`-d, --description`: add a short description to the task.

`-s, --start_date`: determine the starting date of the task. Not using this argument or leaving it empty will assign the date of the current day as the starting day. Use isoformat string "YYYY-MM-DD".

`-e, --end_date`: determine the ending date of the task. Use isoformat string "YYYY-MM-DD".

`--done`: Determine whether the task is checked as done or not. ("False" or "True").

### List tasks

To list the unfinished tasks use:

```
taskaty list
```

`list` option has the following optional argumen:

`-a, --all`: List all the tasks.

### Check a task

To check a task as finished use:

```
taskaty check -t <task_number>
```

### Remove a task

To remove a task use:

```
taskaty remove -t <task_number>
```

If task number is not specified, last task would be removed.

### Remove all tasks

To remove all tasks use:

```
taskaty reset
```
