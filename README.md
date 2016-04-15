# go-chat

## Setup Local Development
1. Make a directory as a workspace for all you go projects. I chose ~/Documents/Development/go
2. Create three directories under this workspace. The directories are bin, pkg, and src.
3. Create a directory under src called 'github.com'
4. Create a directory under githuh.com called 'mebobby2', or whatever your github name is.
5. Open up ~/.bash_profile
6. Add this line to it: export GOPATH=/Users/bobbylei/Documents/Development/go
7. Then add this line after it: export PATH=$PATH:$GOPATH/bin. This line enables you to run your go executable programs from the command line just by entering their name, without worrying where they are located on the hard disk.
8. source ~/.bash_profile
9. Git clone this repo into the directory ~/Documents/Development/go/src/github.com/mebobby2

## Compiling
1. First you need to install gorilla websocket library because go-chat depends on it: go get github.com/gorilla/websocket. This command can be run anywhere on the terminal and installs the library to the directory ~/Documents/Development/go/src/github.com/gorilla/websocket
2. Build the chat client: go install github.com/mebobby2/go-chat. This creates an executable in the directory  ~/Documents/Development/go/bin
3. Run the chat client by typing this anywhere in the terminal: go-chat
4. Open two browsers at: http://127.0.0.1:8080, and chat away


