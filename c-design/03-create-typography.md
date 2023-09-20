# Create a typography

- Use the [typography-template](https://github.com/fastn-stack/typography-template) to create the repository.

- Open the `FASTN.ftd`, replace the default dependency of 
`fifthtry.github.io/inter-font` with the font package name you created in the `create-font` workshop module

- Commit the changes

- Open the `index.ftd` and import the `assets` of same package and give the alias as <font-name>-assets

Example:
```
-- import: fifthtry.github.io/inter-font/assets as lato-assets
```
Here lato-assets is the alias

- Now update the value of all the instances of `font-family` field by replacing `inter-assets` with the `alias` you gave (eg lato-alias)

- Also, replace the `Inter` value with the font you are using 
(eg Lato)

- Commit the changes

- Go to `Settings>Pages` and select `gh-pages` from the `Build 
and deployment` section

- This will generate your live URL once the workflow `Page Build and Deployment` executes successfully

- Open the URL and you will see the output