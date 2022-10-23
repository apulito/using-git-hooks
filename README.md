## Git Hooks

Each Git repository has a local `.git/hooks` folder with a script for each possible hook, they are in the form `hook_type.example`. We can modify these scripts as needed and Git will run them when such events occur.


## Sharing

To share them with the entire development team we can create a folder inside the repository, at the root level, which would allow you to include the files in the version control flow.

Create a ".githooks" folder where to put all the hooks. Then change the hooks directory using the core.hooksPath configuration variable: `$ git config core.hooksPath .githooks`