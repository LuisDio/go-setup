# golang-project

## Golang installation and Setup for ubuntu 16.04

**```$GOROOT/src```**  is the direcory where packages are found such the **Standard Library package** <br/>
If package is not present there, then Go refers to system's environment variable ```GOPATH```.<br>

**```$GOPATH```** is the path to the GO workspace directory which contains all the written source code and ```$GOPATH/src``` is the path to the package within the workspace. Basically this is where you may store store your package. <br/>

You can have as many workspace as you want, as long you keep ```$GOPATH```environment variable pointed to the current working space directory. <br/>


## The Workspace directory structure

A Go workspace directory must have ***three sub directories***. ```src```, ```pkg``` and ```bin```. 

If you want to setup Go workspace, follow this **documentation**. If you are using MacOS, the you can follow this Medium **article** to setup environment variables both temporarily or permanently.<br/>

- src
**src** directory contains GO packages. Any packages installed using ```go get```command will reside here as well.<br/>
In GO, every program is contained in a package. Hence, whenever you will be working with new Go project, you need to create new directory inside $GOPATH/src

- pkg
**pkg** directory contains Go package objects. They are compiled version of original package source code and they have .a file extension (a stands for archived).<br/>
These files contain the compiled package binary code, along with debug symbols and source information. A package object is customized for machine architecture and Go version. These files are created by the Go pack tool while building/installing a package.

- bin
A Go program can either be meant to used as utility inside a package or to perform some operation. We have seen packages and where they reside.<br/>
A Go program which is meant to perform some operation like make a **network request** or **write something to a file** needs to be compiled first, so that your machine can understand the instructions. When you run ```go run hello.go``` command, Go compiler first compiled hello.go file and then executes the resultant binary code.

You can output a binary file from a Go program or package using go build <package-name> (main package) or go build program/path.go command. This will create a binary file in current directory.
