# Building & Developing

I have been working on this using Ubuntu and VSCode, this is how I set it up.

VSCode can be downloaded free from https://code.visualstudio.com/docs/setup/linux 



### Installing Python
* `sudo apt install python3-all-venv`
* `sudo apt install pipx`

### Setting up VSCode
* Install Python VSCode extension from the marketplace.
* Create a virtual environment in VSCode (.venv folder) and activate it.

From the built-in terminal we can setup the dependencies needed:

* `pip install PySide6`
* `pip install vdf`
* `pipx install auto-py-to-exe`

It is important to run these commands from the built-in terminal or it will likely fail. 

### Debugging

Now we can make changes to the code and run them by pressing **F5**.
Breakpoints can be set, changes can be made and tested with ease.


### Compiling for Linux

From the built-in terminal we can generate an executable using auto-py-to-exe 

`auto-py-to-exe -c ./build-linux.json`
