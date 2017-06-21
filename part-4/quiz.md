# Phase 2 Interview Challenge

These are my answers to Part 4 Quiz Time.

## Part 4: Quiz time!

Copy the questions below into a file `part-4/quiz.md`. Then, write your answer to each question directly below it.

The quiz is worth __50 points__ in total.

_Reminder: you can use the internet to help you answer these questions :)_

- When you run a command in the terminal, where does BASH look for that command?
    A: Bash looks for commands in the default path

- On a UNIX computer, how do you stop a running process?
    A: ^c ('control-c') stops a running process that is in focus (i.e. not running in the background).  Some apps require, like node.js require you hit ^c twice to quit.

- What packages do you have installed via homebrew?
    A: homebrew, postresql, mysql
    NOTE: I just got this machine Thursday, June 15 and am still setting up my environment.  I've used npm for most of my library installations.

- On a UNIX computer, how do you find the process id of a running process?
    A: The command I researched says 'pidof' + 'program_name' will give me the process id.  However, I have not used this command and a quick attempt for this question threw the error 'bash: pidof: command not found'

- In a terminal, what does control-c do?
    A: control-c stops the current process

- In a terminal, what does control-a do?
    A: Ctrl-a goes to the beginning of the command line.

- In a terminal, what does control-e do?
    A: Ctrl-e goes to the end of the command line.

- What keyboard shortcut do you use to split the screen in your editor?
    A: In VS Code Cmd-\ (command+\) splits the editor into an additional pane.

- What keyboard shortcut do you use to split the screen in your terminal?
    A: I use VS Code.  This feature is not available natively.  As a result of this question I found an extension which may add this feature but will not install and test it until after this challenge is completed.

- When a terminal command completes, how can you tell if it was successful or not?
    A: It depends on the command and program.  In general, the absence of an error message and return to the '$' prompt indicates success.  In the case of node.js the running program returns '>' (greater than sign) as a prompt.  In the case of postgreSQL nothing is returned so you're okay.

- What does your `~/.gitconfig` have in it? (paste the whole file here)
    NOTE: I just got this machine Thursday, June 15 and am still setting up my environment.  Unfortunately, wiped the other machine before getting this challenge.
    A: git config --list:
        credential.helper=osxkeychain
        color.ui=auto
        core.repositoryformatversion=0
        core.filemode=true
        core.bare=false
        core.logallrefupdates=true
        core.ignorecase=true
        core.precomposeunicode=true
        remote.origin.url=https://github.com/d2rd/phase-2-challenge.git
        remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
        branch.master.remote=origin
        branch.master.merge=refs/heads/master
    

- Lets say you have the following file structure

  ```
  ~
  └── Projects
      ├── pinterest-for-dogs
      │   ├── README.md
      │   └── package.json
      └── linkedin-for-dancers
          ├── README.md
          └── package.json
  ```

  And you were in the `linkedin-for-dancers` folder. What command would you use to change folders to the `pinterest-for-dogs` folder?
    A:  1) 'cd ..' to navigate to the parent folder 'projects' 
        2) 'cd pinterest-for-dogs' to navigate to the target folder.

- What keyboard shortcut do you use, in your editor, when you want to open a specific file?
    A: For VS Code: 'shift/command/o'.

- What files or folders do you want all git repositories to ignore?
    A: Libraries, supporting files and folders and system files like '.DS_STORE'.

- What is the main difference between `==` and `===` in JavaScript?
    A: '==' matches values by character whereas '===' matches values by character AND datatype.  For example: 
        var 'foo' contains the value '10' as an integer.
        var 'bar' contains the value '10' as a string.

        Therefore '10 == 10' will return true but '10 === 10' will return false.  The second case returns false because 'foo' and 'bar' are not the same data type.

