# Apax Template Package

## What is a template

See the [documentation on custom templates](https://axciteme.siemens.com/docs/apax/templates).

## How to use it

1. If not done, login to the GitHub registry

    More information you'll find [here](https://github.com/simatic-ax/.sharedstuff/blob/main/doc/personalaccesstoken.md)

1. Create a new library project from template from CLI

      ```sh
      apax create @simatic-ax/library --registry https://npm.pkg.github.com
      ```
      and follow the dialog

      alternatively:

      ```sh
      apax create @simatic-ax/library --registry https://npm.pkg.github.com <Workspace Name>
      ```

## Create own templates on GitHub

If this template is not suitable for you, you can create your own user spcific templates. This describes, how a template for GitHub is created. For other Git provider it might be similar, but each Git provider has its own specific properies.

1. Select your target path. In this example, it is shown with the Windows Explorer

   ![selPath](docs/images/explorer.png)

1. Open a console by entering `cmd` in the address text box
   
   ![openConsole](docs/images/console.png)
   
   Result: A command line window will be opened

1. Create a new, empty template workspace by entering:

   ```sh
   apax create template template-userspecific
   ```

   > **Important:** It's very important, that the name of the template package starts with `template-` < template-name >


1. Open the template workspace with:

   ```sh
   axcode template-userspecific
   ```

   Result:
   AX Coder is opened and you an see the following workspace structure which consists of:

      ![WSstruct](docs/images/template-structure.png)

   1. The apax.yml `(1)` which is the description for the template package
   
   1. The apax.yml in the template folder `(2)` wich belongs to the workspace, which will be created, when you create a workspace from tis template.
   
   > The template-folder `(2)` is the folder, which comtains all files and folders for the workspace to be created from this template. 
   > For example, it can contain:
   > - your individual apax.yml with scrips, variables or common used dependencies
   > - src- and test-folder with example files
   > - a README.md
   > - a docs folder for further documentation

1. Modify the default apax.yml `(1)`

   The default apax.yml is not suitable to publish your package on a GitHub registry

   Default apax.yml

   ```yml
   name: "template-userspecific"
   version: 0.0.0
   type: generic
   ```

   1. Scope of the templateon GitHub
   
      For GitHub it's important, that the scope is part of the name section. On GitHub, the name of [GitHub organisation](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations) is also the scope.

      If your organisation is `simatic-ax`, then the name section in the apax yml must look like:
      
      ```yml
      name: "@simatic-ax/template-userspecific"
      ```

   1. Define the content for the template
   
      In the file section, in the apax.yml, you can define, what generally will be shipped in a package. For templates, at minimum, the template folder must be shipped. This can be done, by adding the follwoing lines to tha apax.yml

      ```yml
      files:
      - 'template'
      ```

   1. 



1. sdklöfös
 
   ösöslkfjsds

3. sdfsdfwd
   
   sdfsdfs

## Learn More

See the [documentation on custom templates](https://axciteme.siemens.com/docs/apax/templates).
