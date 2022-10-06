## SCR project setup
# Create a python environment
To have a seperate environment for this project it is recommended to have a seperate environment of all the packages that are used. 

[Venv creation online tutorial](https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments)

First of all create a virtual environment for all the python packages
- navigate to the project location
- open the terminal in that location
- enter the command to create the virtual environment
```sh
python -m venv "venv_name"
```
# Package installation
Now that you have created the virtual environment you need to download all the packages that are required for the project to work as intended.
- First step open Pycharm
- On the bottom right corner there is a selection for your python interpreter

![img.png](img.png)
- Click "add interpreter..."![img_2.png](img_2.png)
- Select "Existing environment"![img_4.png](img_4.png)
- Then by clicking the three dots you have to navigate to the previously created virtual environment location and select the python.exe file that is located in Scripts folder
![img_5.png](img_5.png)
- Now on the bottom right side of Pycharm it should be showing the version of python that you are running and the environment name in brackets

Now that we have set up our Pycharm to use the required virtual environment, we can work on installing the packages for the project.

- At the bottom of Pycharm open the tab called "Terminal"
- There it should show that the environment is activated (in this example it is called venv) ![img_6.png](img_6.png)
- Now we need to open the project location where the "requirements.txt" file is located with the command "cd"
```sh
cd "project location"
```
for the cd command you need to give the full path of the project location e.g., "C:\Users\Username\Desktop\Projects\projectname>"<br/>
next use the install command to install all the packages to your virtual environment
```sh
pip install -r requirements.txt
```
Wait for the packages to install and now your virtual environment is set up!

# Set up global environment variables
Variables that are created outside of a function are known as global variables.
The project uses Global environment variables so that we can easily change what URL and login credentials

- open the Start menu enter "environment"
- click "Edit the system environment variables" ![img_7.png](img_7.png)
- click "Environment variables" ![img_8.png](img_8.png)
- when the new window opens click "New..." on the top part of the window ![img_10.png](img_10.png)
- enter the name and value(that are required and keep repeating this step until you create all of the required variables)
- close the windows by pressing OK in the bottom right corner of the window

**Every time you enter a new global variable please restart Pycharm**

Now you have set up the global environment variables! <br />
**name = variable** <br />
SCR_WEBSITE_LOCATION = https://staging-usshortcodes.com/scr <br />
SCR_API_LOCATION = https://staging-usshortcodes.com/scr <br />
SCR_USER_CREDENTIALS = testUser/test_user_1 <br />
SCR_CARRIER_CREDENTIALS = testUser2/test_user_2 <br />
<br />
HEADLESS_MODE = (True or False) <br />
HEADLESS_MODE - is a setting that lets you chose if you want the browser to open when running tests (True = opens browser, False = runs tests without opening a browser)


