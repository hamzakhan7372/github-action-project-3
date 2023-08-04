# what is task for!

## Details of the first workflow

In first workflow file we are creating three job for react code; linting, testing and building!

## Details of the second workflow

In second workflow file, we are creating one job for outputting the detials of first workflow! 
In the second workflow file, we use the following shell command:

- `run: echo "${{ toJSON(github)}}"`

run: echo "${{ toJSON(github)}}": This is the run directive, which specifies the shell command to be executed for this step. In this case, the command is echo "${{ toJSON(github)}}".

* echo: This is a shell command used to print the specified text to the console. It is used here to display the output.

* "${{ toJSON(github)}}": This is an interpolated expression. The ${{ ... }} syntax allows you to use context variables and expressions provided by GitHub Actions. In this case, github is a predefined context variable that contains information about the GitHub event that triggered the workflow.

* toJSON(): This is a built-in GitHub Actions function used to convert the github context variable into a JSON-formatted string. It is necessary because the context variable is an object, and echo requires a string as its argument.