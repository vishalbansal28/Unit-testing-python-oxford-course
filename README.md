# Introduction to Unit Testing with Python and GitHub

This project is a repository accompanying the Oxford RSE online course, designed to introduce participants to unit testing with Python and GitHub. It includes instructions for setting up a development environment, cloning the repository, and running tests using pytest

## Getting started

Before starting, make sure that you have

- a [GitHub](http://github.com/) account, and are logged in
- [Git](https://git-scm.com/) installed on your computer
- [Python](https://www.python.org/downloads/) installed on your computer, v3.5 or newer
- a text editor installed on your computer. If you don't have a favourite, we suggest [VS Code](https://code.visualstudio.com/) and the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python).
- Configure GitHub with [SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) so that you can write to your repository.

If you already have Python installed on your computer, you can check which version you have by opening a terminal (on macOS or Linux) or a command prompt (on Windows) and typing

```
python3 --version
```

If you install Python for this course, go to the link above and choose the default option for your operating system.
If you install Python on Windows, make sure you click the "add to path" option during installation.

## Use this repository as a template

Click the green "Use this template" button at the top of this page.
Follow the prompt to give it a name, but otherwise leave the defaults as they are.

On your computer, clone the repository you have just imported:
- Click the green Code button at the top of the page containing your imported version of this repository
- Select SSH and copy the text provided
- From a terminal (on macOS or Linux) or a command prompt (on Windows), run
  ```
  git clone <paste-string-here>
  ```

## Create a virtual environment

From a terminal (on macOS or Linux) or a command prompt (on Windows), change to the directory created by running the git command above.

We recommend creating a virtual environment for this course.
Type
```
python3 -m venv venv
```

On macOS or Linux, activate this environment by running
```
source venv/bin/activate
```

On Windows, activate this environment by running
```
venv\Scripts\activate.bat
```

## Install packages and check everything is working

Run the following commands:
```
pip install --upgrade pip setuptools wheel
pip install -e .
```

You should see a message that ends with `Successfully installed <list of packages>`.

Then run:
```
pytest -v
```

You should see a message that ends with
```
tests/test_models.py::test_everything_works PASSED     [100%]

===================== 1 passed in 0.08s ======================
```



