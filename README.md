## Git Hooks

Each Git repository has a local `.git/hooks` folder with a script for each possible hook, they are in the form `hook_type.example`. We can modify these scripts as needed and Git will run them when such events occur. In this example the pre commit hook has been customized to manage the branch naming.

## Sharing across the team

Let's create a folder inside the repository, at the root level, to include it in the version control flow. In this way you can share hooks with the entire development team.

So, create a ".githooks" folder where to put all the hooks. Then change the hooks directory using the core.hooksPath configuration variable to point to the new folder: `$ git config core.hooksPath .githooks`