# @simatic-ax/apax-package-name-d7b4b031

## Description

*please insert a description of the library*

## Getting started

Install with Apax:

> If not yet done login to the GitHub registry first.
> More information you'll find [here](https://github.com/simatic-ax/.github/blob/main/docs/personalaccesstoken.md)

```cli
apax add @simatic-ax/apax-package-name-d7b4b031
```

Add the namespace in your ST code:

```iec-st
Using apax-package-name-d7b4b031;
```

## Library functionality

| Classes | Description         |
|---------|---------------------|
| *xyz*     | *description for xyz* |

| Functions   | Description             |
|-------------|-------------------------|
| *xyz*       | *description for *xyz** |

| Function Blocks | Description           |
|-----------------|-----------------------|
| *xyz*           | *description for xyz* |

## Folder structure
```bash
apax-package-name-d7b4b031
    |
    +- .github
    |   |  # GitHub workflows for maintaining the library
    |   |- package-development-workflow.yml
    |   |- package-release-workflow.yml
    |
    +- docs
    |   | # the place for additional user-documentation
    |   |- MyClass.md
    |    
    +- snippets
    |    | # may contain helpful snippets for using the library
    |    |- namespacesupport.json
    |    |- usingNamespace.json
    |
    +- src
    |   | # adjust and add library src files here
    |   |- myClass.st
    |
    +- test
    |   | # adjust and add test-programs here
    |   |- dummy.st
    |
    | # additional meta-information for GitHub/-workflows
    |- .gitattributes
    |- .gitignore
    |
    | # settings file for activating the renovate-bot
    |- renovate.json
    |
    | # adjust the project description file / add apax-scripts
    |- apax.yml
    |
    | # essential git project files, pls. adjust
    |- CODEOWNERS
    |- README.md
    |- LICENSE.md #do not change!
```

## Contribution

Thanks for your interest in contributing. Anybody is free to report bugs, unclear documentation, and other problems regarding this repository in the Issues section or, even better, is free to propose any changes to this repository using a pull request.

## License and Legal information

Please read the [Legal information](LICENSE.md)
