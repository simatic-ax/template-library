# Template for SIMATIC AX `libraries` on GitHub

## What is a library

In computing, a library is a collection of resources that is leveraged during software development to implement an application. Commonly, a library consists of executable code such as compiled functions and classes, or a library can be a collection of source code. This template is tailored for the creation of libraries for PLC applications (executable on a PLCSIM Advanced or real PLC S7-1500).

## Create a project from this "apax-template"

If you want to create a new library inside the GitHub community, please start with using this apax-template by entering the following in the terminal:

```bash
apax create @simatic-ax/library --registry https://npm.pkg.github.com
```

## Folder-structure of this "library" apax-template

```bash
+- template-library
        |     
        +-- .github
        |      |  # GitHub workflows for maintaining the template
        |      |- package-development-workflow.yml
        |      |- package-release-workflow.yml
        |
        +-- template # the content that is going to be installed when using @simatic-ax/app during an apax create
        |      |
        |      +- .github
        |      |   |  # GitHub workflows for maintaining the library
        |      |   |- package-development-workflow.yml
        |      |   |- package-release-workflow.yml
        |      |
        |      +- docs
        |      |   | # the place for additional user-documentation
        |      |   |- MyClass.md
        |      |    
        |      +- snippets
        |      |    | # may contain helpful snippets for using the library
        |      |    |- namespacesupport.json
        |      |    |- usingNamespace.json
        |      |
        |      +- src
        |      |   | # adjust and add library src files here
        |      |   |- myClass.st
        |      |
        |      +- test
        |      |   | # adjust and add test-programs here
        |      |   |- dummy.st
        |      |
        |      | # additional meta-information for GitHub/-workflows
        |      |- .gitattributes
        |      |- .gitignore
        |      |
        |      | # settings file for activating the renovate-bot
        |      |- renovate.json
        |      |
        |      | # adjust the project description file / add apax-scripts
        |      |- apax.yml
        |      |
        |      | # essential git project files, pls. adjust
        |      |- CODEOWNERS
        |      |- README.md
        |      |- LICENSE.md #do not change!
        |
        |- apax.yml # The project manifest identifying this package as a template
```
## Before releasing

Before you release the application example, all checks have to be done:

- [ ] OSS Clearing
- [ ] Patent Clearing
- [ ] ECC (Export control with the [ecc wizzard](https://code-ops.code.siemens.io/ecc-wizard/))
- [ ] License is up to date
- [ ] Codeowner are up to date
- [ ] The Readme.md contains a description:
  - What is this library doing ?
  - How to install the library
  - How to use the library
- [ ] Library has been reviewed
  - Create an Pull-Request for your Main-branch and add community-admins as reviewer

## Release of the library

Successfully releasing your library will trigger the creation of an apax-package of your current repository. Be aware of failing pipelines (GitHub workflows).

## Learn More

See the [documentation on custom templates](https://console.simatic-ax.siemens.io/docs/apax/templates).
