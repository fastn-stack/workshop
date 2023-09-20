# Create a fonts

This workshop will help you create your fastn fonts.

## Prerequisites: 

- Install [Python](https://www.python.org/downloads/) 

- Also, if you do not have `pip` installed, follow the reference URL to install: https://packaging.python.org/en/latest/tutorials/installing-packages/

## Steps:

- Clone [google-font-to-fastn](https://github.com/fastn-stack/google-font-to-fastn) repository into your local machine
![](/c-design/static/google-font-to-fastn-repo.png)

- Open the cloned repo through a text editor (eg Sublime Text)

- Explore the [Google fonts](https://fonts.google.com/) and 
choose the font you want to create in `fastn` (eg: lato)
![](/c-design/static/google-font-lato.png)

- Select all the styles of the font that you want to have in 
your font package
![](/c-design/static/selected-lato-styles.png)

- Copy the URL, for eg: https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap
![](/c-design/static/copy-lato-url.png)

- Paste the URL in the new tab and copy the content of the 
entire page
![](/c-design/static/display-content.png)

- In the cloned `google-font-to-fastn` repo, open the `font.txt`
file and replace the content of this file with the copied 
content
![](/c-design/static/font-txt.png)

- Use the 
[font-template](https://github.com/fastn-stack/font-template) 
to create the font repository
![](/c-design/static/font-template.png)

> Naming convention: Use the google-font name (eg: Lato) and 
append it with `-font`. 
(eg: lato-font, make sure the name is in lowercase)

- Copy the the font repostory package name from the `FASTN.ftd` 
file
![](/c-design/static/package-name-in-FASTN.png)

- In the cloned `google-font-to-fastn` repo, open the 
`read_google_font.py` file

- Search for `package_name` variable and change the value with 
your font repository package name.
Also, search for `repo` variable and change the value with the 
alias name (eg: lato-font) 

![](/c-design/static/package-name-in-py.png)

- Open the terminal and navigate to the directory of the cloned 
`google-font-to-fastn` repo
![](/c-design/static/navigate-to-directory.png)

- Run the `python request` command 
```
python3 -m pip install requests
```
Note: If the python version is above 3 then this command will 
work, else you can use `python -m pip install requests`

- Once the installation is successful, run the 
`read_google_font.py` script: 
```
python3 read_google_font.py
```
![](/c-design/static/run-py-script.png)

(This script will generate `FASTN.ftd` and `static` folder in 
the `google-font-to-fastn` repository)

![](/c-design/static/FASTN-and-static.png)

- Open the `FASTN.ftd` file and copy the all `--fastn.font` 
sections
![](/c-design/static/copy-fastn-font.png)

- Now, open the `FASTN.ftd` of the font repository you created 
using the font-template

- Paste the copied `--fastn.font` sections there and Commit the 
changes
![](/c-design/static/paste-fastn-font.png)

- Now, open the `custom.ftd` file and replace <font-name> with 
the selected font name (eg: Lato)
![](/c-design/static/replace-font-name.png)

- Copy the `static` folder that was created in the 
`google-font-to-fastn` repository when you executed the command 
and paste it in your repository
![](/c-design/static/added-static-folder.png)

- You have successfully created your custom font

- Go to `Settings>Pages` and select `gh-pages` from the `Build 
and deployment` section
![](/c-design/static/lato-gf-pages.png)

- This will generate your live URL once the workflow `Page Build and Deployment` executes successfully

- Open the URL and you will see the output

- You can move to 
[create typography](/c-design/02-create-typography.md)