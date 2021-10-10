### Contributing

Let's get ready to contribute.

Contributions are welcome and appreciated!

### Git Workflow to contribute to an Open Source Project:

- Fork this repository: Click on "Fork" and choose a suitable GitHub account for the fork eg. your personal Github account.

- Clone your own project fork into your development machine and cd into that directory.

    ```
    $ git clone https://github.com/yourusername/Spot-the-difference.git

    ```

- Create a new branch in the project for the specific fixes that you want to contribute (name it after either a bugfix, a tracker issue, a documentation section, etc) and switch to it.

    ```
    $ git checkout -b <branch name>

    ```
    This automatically creates the branch and switches to it.

- Use your favourite editor to make changes to the files in your local repository. Any changes you make will only affect the branch you have created.

- Add the changes to the staging area and then commit changes to the branch.

    ```
    $ git add <file name>
    $ git commit -m "your commit message"

    ```

- Push your changes to your forked repository

    ```
    $ git push origin <branch name>

    ```

    This pushes your changes to the &lt;branch name&gt; branch of the "origin" (which is your fork on GitHub).

- From the GitHub forked Repository open a pull request by click "Pull Requests"->"New Pull Request"

### Resource

- Find Git CheatSheet and a good commit message resources under Git folder.
- Commit messages are a key part of your project history, so it's always a good practice to write descriptive commit message.
- Also, there is GitKraken CheatSheet for your reference.