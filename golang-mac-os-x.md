# Golang on Mac OS X

Install Golang:
```
brew update
brew install golang
```

Setup Go workspace:
```
mkdir $HOME/go
cd $HOME/go
mkdir bin pkg src 
```

Setup Go environment:
```
vi ~/.bash_profile
export GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin
```

Create, build, and run a Go project:
```
mkdir $GOPATH/src/github.com/<username>/myapp
touch $GOPATH/src/github.com/<username>/myapp/myapp.go
go install
myapp
```

Make your program runnable from CLI:
* Create an executable file: `go build myapp.go`
* Copy this file to a directory on your system path: `cp myapp /usr/local/bin`
* Run on CLI: `myapp --list`

Import a Go package: `go get -u github.com/urfave/cli`

Generate a program documentation for package fmt: `godoc fmt`

