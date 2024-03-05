# @simatic-ax.<Library>

## Description

## Install this package

Enter:

```cli
apax add @simatic-ax/<Library>
```

## Namespace

```iec-st
Simatic.Ax.<Library>;
```

## Publish library

> This is only working for public libraries. Public libraries must fulfill the OSS clearing process.

To publish that library on GitHub, the following steps are required

1. Check the apax.yml
1. create the remote repository on GitHub
1. add a remote repository
1. push the repository to the remote repository
1. start the release workflow

### Check the apax.yml

the apax.yml must contain the correct name consisting of organization (e.g. `@simatic-ax`) and project name (e.g `myproject`).

```yml
name: "@simatic-ax/myproject"
```

### create the remote repository on GitHub

Click on https://github.com/organizations/simatic-ax/repositories/new to create a new project.

The `Repository name` must be the same like your project name (e.g `myproject`) 

> don't enter the scope

### add a remote repository to your local repository

```sh
git branch -M main
git remote add origin git@github.com:simatic-ax/<myproject>.git
```


### push the repository to the remote repository

```sh
git branch -M main
git remote add origin git@github.com:simatic-ax/<myproject>.git
```
### start the release workflow

Draft new release

![release](/docs/images/release1.png)

![release](/docs/images/release2.png)

- Choose a tag
- Enter a version regarding semantic versioning (e.g. `0.0.2`)
- Create a new tag
- 
![release](/docs/images/release3.png)

--> Result: The release workflow in GitHub actions starts

## Objects

## Example

<please provide a working example>

## Contribution

Thanks for your interest in contributing. Anybody is free to report bugs, unclear documentation, and other problems regarding this repository in the Issues section or, even better, is free to propose any changes to this repository using Merge Requests.

## License and Legal information

Please read the [Legal information](LICENSE.md)
