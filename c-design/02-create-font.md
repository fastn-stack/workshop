# Create a fonts

## Prerequisites: 

- Install Python 

## Steps:

- Use the 
[font-template](https://github.com/fastn-stack/font-template) to create the repository.
![](/c-design/static/font-template.png)

- Explore Google font: https://fonts.google.com/

- Select the sizes of the font that is provided or the 
selected google font

- Copy the URL, for eg: https://fonts.googleapis.com/css2?family=Croissant+One&display=swap

- Paste the URL in the new tab

- Select all and copy the generated data

- Clone [google-font-to-fastn](https://github.com/fastn-stack/google-font-to-fastn) repository into your local

- Open the cloned repo through a text editor

- Open the `font.txt` file and paste the generated data

- Open the `read_google_font.py` file and search for 
`package_name` field and change the `package_name` with your 
font repository package name 
(eg: fastn-community.github.io/lato-font)

- Also search for `repo` field and change the value with the 
alias name (eg: lato-font)

- Open the terminal


- Run the `python request` command that is mentioned in the 
[create-font-package](https://fastn.com/create-font-package/) URL .ie. `python3 -m pip install requests`


- Once the installation is successful, go back to the 
`create-font-package` URL and scroll down and copy the 
`read_google_font.py` code and execute it in the terminal ie. 
`python3 read_google_font.py`

- Open the `FASTN.ftd` file and copy the `--fastn.font` sections 

- Now, open the `FASTN.ftd` of the font repository you created 
using the font-template

- Paste the copied `--fastn.font` sections there and Commit the 
changes.

- Now, open the `custom.ftd` file and replace <font-name> with 
the selected font name

- Copy the `static` folder that was created in the 
`google-font-to-fastn` repository when you executed the command 
and paste it in your repository.

- Go to `Settings>Pages` and select `gh-pages` from the `Build 
and deployment` section

- You have successfully created your custom font

- You can move to 
[create typography](/c-design/02-create-typography.md)