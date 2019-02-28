# golang-project

## Golang installation and Setup for ubuntu 16.04

```$GOROOT/src``` is the direcory where packages are found such the **Standard Library package** <br/>
If package is not present there, then Go refers to system's environment variable ```GOPATH```.<br>

```$GOPATH```is the path to the GO workspace directory which contains all the written source code and ```$GOPATH/src``` is the path to the package within the workspace. Basically this is where you may store store your package. <br/>
You can have as many workspace as you want, as long you keep ```$GOPATH```environment variable pointed to the current working space directory. <br/>


## The Workspace directory structure

A Go workspace directory must have ***three sub directories***. ```src```, ```pkg``` and ```bin```. If you want to setup Go workspace, follow this **documentation**. If you are using MacOS, the you can follow this Medium **article** to setup environment variables both temporarily or permanently.<br/>

- src
This directory contains GO packages. Any packages installed using ```go get```command will reside here as well. In GO, every program is contained in a package. Hence, whenever you will be working with new Go project, you need to create new directory inside $GOPATH/src
