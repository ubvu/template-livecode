# Livecode repository

## For learners

This repository keeps track of the code being written by the instructor.
Use it to catch up or as a reference when running into errors.

The folder structure is a good starting point when creating a project yourself.

## For instructors

Use [gitautopush](https://pypi.org/project/gitautopush/) to automatically push your livecode to this repository.

### Prerequisites

- Python and pip installed
- Git installed
- GitHub account added to the repository as a Contributor 

### Installation and usage

- in a first terminal window `git clone` this repository to create a tracked working directory
- if you already cloned this repository a while ago, `git pull` to avoid conflicts
- in a second terminal window, install gitautopush with `pip install gitautopush`
- in this second terminal window, start observing the folder with the command: `gitautopush --sleep <INT> /path/to/my/repo/folder`. `<INT>` is the amount of time (in seconds) between attempts to synchronise the code in the local repository with the remote
- save the files in the working directory often and regularly (or automatically)
- double check in the second terminal window if gitautopush automatically pushes your changes to the repository: in case of failure, the errors `git` throws should be inside the message of gitautopush  
- once you finish your lesson, close gitautopush in the second terminal window with <kbd>Ctrl</kbd>+<kbd>C</kbd> or close the terminal window altogether

### Troubleshooting

- ValueError: A `git status` command didn't work, are you sure this is a git repository?
    - It might be occuring when there are already some changes to be staged once you launch `gitautopush`. First, run `gitautopush`, then start creating files or making changes to the existing ones. 
    - Another thing to try is to first commit and push one file manually to the repository, once you have done that and no changes are staged run `gitautopush`


