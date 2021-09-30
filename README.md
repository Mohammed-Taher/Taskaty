# Taskaty

A simple command line interface app for task management.

## Installation

Clone this repository then run:

```
pip install -e .
```

You will be able to run the app from the command line using the `taskaty` command.

## Usage

To add a task use the option `add`.

```
taskaty add "Add search bar compoent to the UI"
```

`add` option has the following optional arguments:

`-d, --description`: add a short description to the task.

`-s, --start_date`: determine the starting date of the task. Not using this argument or leaving it empty will assign the date of the current day as the starting day.

`-e, --end_date`: determine the ending date of the task.

`--done`: Determine whether the task is checked as done or not.
